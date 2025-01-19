---
tags:
  - Source
banner: 
banner_lock: true
banner_y: 0
type: Source
icon: LiBookMarked
---
# Classes
```dataview
LIST
FROM #Class
WHERE contains(sources, link(this.file.name))
SORT file.name ASCENDING
```
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
# Spells
```dataview
LIST
FROM #Spell
WHERE contains(sources, link(this.file.name))
SORT file.name ASCENDING
```
# Feats
```dataview
LIST
FROM #Feat
WHERE contains(sources, link(this.file.name))
SORT file.name ASCENDING
```