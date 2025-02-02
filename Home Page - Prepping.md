---
tags:
  - Dashboard
icon: LiHome
---

# Home Page - Prepping

## To Do List

```tasks
( not done ) AND NOT ( path includes z_Templates )
Short
```

## Buttons

```meta-bind-button
label: New Item
icon: ""
hidden: false
class: ""
tooltip: ""
id: item
style: primary
actions:
  - type: templaterCreateNote
    templateFile: z_Templates/Template - Item.md
    folderPath: Homebrew/Wondrous Items
    fileName: Untitled
    openNote: true

```

## Useful Links

- [Chat GPT Site](https://chatgpt.com/)
- [D&D Beyond Campaign](https://www.dndbeyond.com/campaigns/4438888)
- [Ledger+](https://ledger.thegriffonssaddlebag.com/)
- [Item Cards Doc](https://docs.google.com/presentation/d/14xa7q2X1g3ze7Fm3ygqxDmSD6wNtIJqBtLxIf08fnSg/edit)
- [Generators](https://watabou.github.io/#)
- [Statblock Generator](https://tetra-cube.com/dnd/dnd-statblock.html)

## Last Updated

 ```dataview
TABLE WITHOUT ID
link(file.name) as "Name", tags as "Tags", type as "Type", file.mtime as "Last Edited"
WHERE !contains(file.folder, "z")
SORT file.mtime DESC
LIMIT 10
```

![[Island-Banner-2.png|banner]]
