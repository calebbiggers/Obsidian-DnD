---
tags:
  - City
aliases: 
pronounced: 
type: Settlement
population: 
themes: 
kingdom: 
terrain: 
location: 
rulers: 
leaders: 
gov_type: 
exports: 
religions: 
banner: "[[Settlement-Banner.jpg]]"
imports: 
defences: 
banner_lock: true
icon: LiBuilding2
banner_y: 0.8
image: "[[PlaceholderImage.png]]"
---
> [!place-wiki]+ `=this.file.name`
> **Pronounced:**  "`=this.pronounced`"
> `$= dv.paragraph(dv.func.embed(dv.current().image))`
> ##### Info
>  |
> ---|---|
> **Alias** | `$= !dv.current().aliases ? "None" : dv.current().aliases.join(", ")` |
> **Type** | `=this.type` |
> **Population** | `$=  !dv.current().population ? "Unknown" : String(dv.current().population)` |
> **Themes** | `$= !dv.current().themes ? "None" : dv.current().themes.join(", ")` |
> **Kingdom** | `=this.kingdom` |
> **Terrain** | `$= !dv.current().terrain ? "None" : dv.current().terrain.join(", ")` |
> **Location** | `=this.location` |
> ##### Politics
>  |
> ---|---|
> **Rulers** | `$= !dv.current().rulers ? "N/A" : dv.current().rulers.join(", ")` |
> **Leaders** | `$= !dv.current().leaders ? "None" : dv.current().leaders.join(", ")` |
> **Govt Type** | `=this.gov_type` |
> **Defenses** | `$= !dv.current().defences ? "None" : dv.current().defences.join(", ")` |
> **Religions** | `$= !dv.current().religions ? "None" : dv.current().religions.join(", ")` |
> ##### Commerce
>  |
> ---|---|
> **Imports** | `$= !dv.current().imports ? "None" : dv.current().imports.join(", ")` |
> **Exports** | `$= !dv.current().exports ? "None" : dv.current().exports.join(", ")` |
# Description
>[!quote] Read To Players
>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras vulputate iaculis dui, ut aliquet velit. Vivamus eu ornare sem. Quisque tincidunt, leo ac malesuada lobortis, dui nisl varius nunc, fermentum tincidunt velit nulla et ipsum. In mi nulla, hendrerit ac augue vel, porta porta urna. Nunc congue pretium eros, eu euismod arcu efficitur eget. Aliquam molestie neque in felis mollis, at accumsan enim tempus. Fusce rhoncus sollicitudin mauris, eget posuere risus tristique sagittis. Maecenas gravida dui dui, sit amet accumsan ipsum maximus vel. In tincidunt, elit nec tempor hendrerit, dui metus pulvinar ipsum, fringilla malesuada erat ex vitae mi. Sed non ullamcorper tellus, ac consectetur nunc. Sed lacus urna, accumsan quis nunc quis, scelerisque rutrum ipsum.
# Background
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras vulputate iaculis dui, ut aliquet velit. Vivamus eu ornare sem. Quisque tincidunt, leo ac malesuada lobortis, dui nisl varius nunc, fermentum tincidunt velit nulla et ipsum. In mi nulla, hendrerit ac augue vel, porta porta urna. Nunc congue pretium eros, eu euismod arcu efficitur eget. Aliquam molestie neque in felis mollis, at accumsan enim tempus. Fusce rhoncus sollicitudin mauris, eget posuere risus tristique sagittis. Maecenas gravida dui dui, sit amet accumsan ipsum maximus vel. In tincidunt, elit nec tempor hendrerit, dui metus pulvinar ipsum, fringilla malesuada erat ex vitae mi. Sed non ullamcorper tellus, ac consectetur nunc. Sed lacus urna, accumsan quis nunc quis, scelerisque rutrum ipsum.
# Notes
- Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras vulputate iaculis dui, ut aliquet velit. Vivamus eu ornare sem. Quisque tincidunt, leo ac malesuada lobortis, dui nisl varius nunc, 
- Sed non ullamcorper tellus, ac consectetur nunc. Sed lacus urna, accumsan quis nunc quis, scelerisque rutrum ipsum.


# Districts
```dataview
TABLE WITHOUT ID
link(file.name) as "Name"
FROM #District
WHERE location=link(this.file.name)
SORT file.name ASCENDING
```
# Shops
```dataview
TABLE WITHOUT ID
link(file.name) as "Name", type as "Type", owners as "Owners"
FROM #Shop or #Service
WHERE location=link(this.file.name)
SORT file.name ASCENDING
```
# Points of Interest
```dataview
TABLE WITHOUT ID
link(file.name) as "Name", type as "Type"
FROM #Location 
WHERE location=link(this.file.name)
SORT file.name ASCENDING
```
# Groups
```dataview
TABLE WITHOUT ID
link(file.name) as "Name", type as "Type", leaders as "Leaders"
FROM #Organization 
WHERE location=link(this.file.name) or  hq=link(this.file.name)
SORT file.name ASCENDING 
```
## Characters
```dataview
TABLE WITHOUT ID
link(file.name) as "Name", occupations as "Occupations", location as "Location"
FROM #NPC or #PC or #Random-NPC
WHERE location=link(this.file.name) or home=link(this.file.name)
SORT file.name ASCENDING
```

![[Settlement-Banner.jpg|banner]]