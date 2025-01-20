---
tags:
  - Source
banner: "[[Taldorei-Campaign-Setting-Reborn-Banner.jpg]]"
banner_lock: true
banner_y: 0
type: Source
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
# Spells
```dataview
LIST
FROM #Spell
WHERE contains(sources, link(this.file.name))
SORT file.name ASCENDING
```

![[Taldorei-Campaign-Setting-Reborn-Banner.jpg|banner]]