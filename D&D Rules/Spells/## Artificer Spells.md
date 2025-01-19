## Cantrips
```dataview
LIST
FROM #Spell
WHERE contains(classes, "Artificer")
GROUP BY level
SORT file.name ASCENDING 
```
## Level 1
```dataview
LIST
FROM #Spell and #Artificer and #Lvl1
SORT file.name ASCENDING
```
## Level 2
```dataview
LIST
FROM #Spell and #Artificer and #Lvl2
SORT file.name ASCENDING
```
## Level 3
```dataview
LIST
FROM #Spell and #Artificer and #Lvl3
SORT file.name ASCENDING
```
## Level 4
```dataview
LIST
FROM #Spell and #Artificer and #Lvl4
SORT file.name ASCENDING
```
## Level 5
```dataview
LIST
FROM #Spell and #Artificer and #Lvl5
SORT file.name ASCENDING
```