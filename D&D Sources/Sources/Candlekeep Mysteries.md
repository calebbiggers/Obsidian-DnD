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

![[Candlekeep-Mysteries-Banner.jpg|banner]]