---
tags:
  - Source
banner: "[[Unearthed-Arcana-Banner.jpg]]"
banner_lock: true
banner_y: 0
type: Source
icon: LiBookMarked
---
# Spells
```dataview
LIST
FROM #Spell
WHERE contains(sources, link(this.file.name))
SORT file.name ASCENDING
```

![[Unearthed-Arcana-Banner.jpg|banner]]