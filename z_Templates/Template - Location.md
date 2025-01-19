---
tags:
  - Location
aliases: 
type: 
pronounced: 
owners: 
location: 
groups: 
banner: "[[Location-Banner.jpg]]"
banner_lock: true
banner_y: 0
icon: LiMapPin
---
> [!place-wiki]+ `=this.file.name`
> **Pronounced:**  "`=this.pronounced`"
> ![[PlaceholderImage.png]]
> ##### Info
>  |
> ---|---|
> **Aliases** | `$= !dv.current().aliases ? "None" : dv.current().aliases.join(", ")` |
> **Type** | `=this.type` |
> **Owner(s)** | `$= !dv.current().owners ? "N/A" : dv.current().owners.join(", ")` |
> **Location** | `=this.location` |
> **Group(s)** | `$= !dv.current().groups ? "N/A" : dv.current().groups.join(", ") ` |
# Description
> [!quote]+ Read to Players
TBD
# Background

# Shops
```dataview
LIST
FROM #Shop or #Service
WHERE location=link(this.file.name)
SORT file.name ASCENDING
```
# Points of Interest
```dataview
LIST
FROM #Location 
WHERE location=link(this.file.name)
SORT file.name ASCENDING
```
# Groups
```dataview
LIST 
FROM #Organization 
WHERE location=link(this.file.name) or hq=link(this.file.name)
SORT file.name ASCENDING 
```
# Characters
```dataview
LIST
FROM #NPC 
WHERE location=link(this.file.name) or home=link(this.file.name)
SORT file.name ASCENDING
```


![[Location-Banner.jpg|banner]]