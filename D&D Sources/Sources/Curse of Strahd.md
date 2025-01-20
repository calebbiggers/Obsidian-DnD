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

![[Curse-Of-Strahd-Banner.jpg|banner]]