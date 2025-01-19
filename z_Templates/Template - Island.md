---
tags:
  - Island
aliases:
type: Island
pronounced:
plane:
themes:
terrain:
location:
rulers:
leaders:
gov_type:
religions:
banner: "[[Island-Banner-2.png]]"
banner_lock: true
ocean:
---
![[Island-Banner-2.png|banner]]
> [!island-wiki]+ `=this.file.name`
> **Pronounced:**  "`=this.pronounced`"
> ![[PlaceholderImage.png]]
> ##### Info
>  |
> ---|---|
> **Aliases** | `$= !dv.current().aliases ? "None" : dv.current().aliases.join(", ")` |
> **Themes** | `$= !dv.current().themes ? "None" : dv.current.themes.join(", ")` |
> **Location** | `$= !dv.current().location ? "N/A" : dv.current().location` |
> **Plane** | `=this.plane` |
> **Terrain** | `$= !dv.current().terrain ? "N/A" : dv.current.terrain().join(", ")` |
> ##### Politics
>  |
> ---|---|
> **Rulers** | `$= !dv.current().rulers ? "N/A" : dv.current().rulers.join(", ")` |
> **Leaders** | `$= !dv.current().leaders ? "None" : dv.current().leaders.join(", ")` |
> **Govt Type** | `$= !dv.current().gov_type ? "None" : dv.current().gov_type` |
> **Religions** | `$= !dv.current().religions ? "None" : dv.current().religions.join(", ")` |
# **`=this.file.name`**
> [!info|overview]+ Overview
TBD

## History
-
## Politics & Relationships
-
## Current Events
-
## Plot Hooks
-
## Hidden Details
-
## General Notes

## Settlements & Cities
 [[+Settlement Database|📝Create New Settlement/City]]
```dataview
LIST
FROM #Settlement or #City
WHERE location=link(this.file.name)
SORT file.name ASCENDING
```
## Locations & Landmarks
[[+Location Database| 📝Add New Location/Landmark]]
```dataview
LIST
FROM #Location 
WHERE location=link(this.file.name)
SORT file.name ASCENDING
```
##  Groups & Organization
[[+Organization Dataabase| 📝Add New Group/Organization]]
```dataview
LIST
FROM #Organization 
WHERE location=link(this.file.name) OR hq=link(this.file.name)
SORT file.name ASCENDING
```