---
tags:
  - Source
banner: "[[Van-Richtens-Guide-To-Ravenloft-Banner.jpg]]"
banner_lock: true
banner_y: 0.3
type: Source
icon: LiBookMarked
---
# Items
```dataview
LIST
FROM #Item 
WHERE contains(sources, link(this.file.name))
SORT file.name ASCENDING
```

![[Van-Richtens-Guide-To-Ravenloft-Banner.jpg|banner]]