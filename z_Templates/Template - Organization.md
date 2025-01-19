---
tags:
  - Organization
aliases: 
type: 
pronounced: 
hq: 
location: 
leaders: 
associated_religion: 
alignment: 
banner: "[[Group-Banner.webp]]"
banner_lock: true
icon: LiUsers
---
> [!infobox-wiki]+ `=this.file.name`
> **Pronounced:**  "`=this.pronounced`"
> ![[PlaceholderImage.png]]
> ##### Basic Information
> 
> | | |
> |---|---|
> | **Aliases** | `$= !dv.current().aliases ? "None" : dv.current().aliases.join(", ")` |
> | **Leaders** | `$= !dv.current().leaders ? "None" : dv.current().leaders.join(", ")` |
> | **Type** | `=this.type` |
> | **Base of Operations** | `$= !this.hq ? "None" : dv.current().hq` |
> | **Associated Religion** | `$= !this.associated_religion ? "None" : dv.current().associated_religion` |
> | **Alignment** | `=this.alignment` |
> 

> [!quote]+  Read to the Players
TBD

# Background
## Characters
```dataview
LIST
FROM #NPC 
WHERE contains(groups,link(this.file.name))
SORT file.name ASCENDING
```
## Points of Interest
```dataview
LIST
FROM #Location 
WHERE contains(groups,link(this.file.name))
SORT file.name ASCENDING
```
## Shops & Services
```dataview
LIST
FROM #Shop or #Service
WHERE contains(groups,link(this.file.name))
SORT file.name ASCENDING
```



![[Group-Banner.webp|banner]]