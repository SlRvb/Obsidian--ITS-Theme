# CSS Classes
> CSS Classes to add in the frontmatter/yaml to change the way a page looks.

**Example:**
```
---
cssclass: table, t-c, no-m
---
```

Classes | Description
---|---|
`no-m` | Fully hide Frontmatter on just that page
`justified` | Justifies text
`readable` | Set readable line width to just that page when readable line width is off
`writing` | Centers Headings, justifies text, auto sets readable line width
`poem` | Centers text
`kanban` | Turn lists into kanban-like boards
`k-o` | Adds border and bullet to sub list of a kanban list
`table` | First column has a darker background and text is bolded
`t-c` | Center tables
`t-w` | Table expands to fill the whole width of the file
`hc` | Center headings
`hcl` | Center headings with a line on each side
`illusion` | Apply [Illusion Theme](https://github.com/ZaherAlMajed/Illusion-Theme.md) inspired styling to headings
`dvl` | Stylize Dataview Lists to be more spaced out and have a background
`s-li` | Space out lists
`img-grid` | Apply [image grid](Image-Positions#image%20grid) to all pictures on page

## Ids 

`<s id="#col"></s>`

Classes | Description
---|---|
`#col` | Show/Create a color block
`#font` | Showcase a font in huge sized text
`#vid` | 16:9 aspect ratio for videos. Used before an iframe:<br>`<div id=vid><iframe></iframe></div>`

**Examples:**
![](https://i.imgur.com/FHYhFcR.png)
![](https://i.imgur.com/3cSv8c3.png)