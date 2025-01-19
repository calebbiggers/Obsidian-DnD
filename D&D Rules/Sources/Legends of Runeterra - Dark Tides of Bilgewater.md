---
tags:
  - Source
icon: LiBookMarked
---
# Subclasses
```dataview
LIST
FROM #Subclass 
WHERE contains(sources, link(this.file.name))
SORT file.name ASCENDING
```
# Items
```dataview
LIST
FROM #Item 
WHERE contains(sources, link(this.file.name))
SORT file.name ASCENDING
```

![[Legends-Of-Runeterra-Dark-Tides-Of-Bilgewater-Banner.jpg|banner]]