---
tags:
  - Source
icon: LiBookMarked
---
# Items
```dataview
LIST
FROM #Item 
WHERE contains(sources, link(this.file.name))
SORT file.name ASCENDING
```

![[Lost-Mine-Of-Phandelver-Banner.jpg|banner]]