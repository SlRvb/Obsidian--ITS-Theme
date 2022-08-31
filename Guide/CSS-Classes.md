# CSS Classes
> CSS Classes to add in the frontmatter/yaml to change the way a page looks.

**Example:**
```
---
cssclass: table, t-c, no-m
---
```

| Classes | Description |
| --- | --- |
| `no-m` | Fully hide Frontmatter on just that page |
| `justified` | Justifies text |
| `readable` | Set readable line width to just that page when readable line width is off |
| `writing` | Centers Headings, justifies text, auto sets readable line width |
| `poem` | Centers text |
| `dvl` | Stylize Dataview Lists to be more spaced out and have a background |
| `dvl-c` | Style Dataview Tables and Lists as cards/like a Notion gallery |
| `alt-co` | Style all callouts with background as the callout color |
| `hr-tog` | Remove horizontal line icons |
| `img-grid` | Apply [image grid](Image-Positions#image%20grid) to all pictures on page |

<!--`alt-line` | Style all callouts with only an underline under the title-->

#### Headers/Headings

| Classes | Description | 
|---|---|
| `hc` | Center headings
| `hcl` | Center headings with a line on each side
| `illusion` | Apply [Illusion Theme](https://github.com/ZaherAlMajed/Illusion-Theme.md) inspired styling to headings
| `h-line` | Remove all header underlines from note
| `sphd-und-#` | Numbers(#) 1-6 will hide all underlines for specific header levels <br>`sphd-und-3`, `sphd-und-1`

#### Lists

| Classes | Description | 
|---|---|
| `kanban` | Turn lists into kanban-like boards
| `k-o` | Adds border and bullet to sub list of a kanban list
| `s-li` | Space out lists
| `bul-li-neon` | Neon glow style for list lines
| `bl-c` | Bullets are only one color on page (Accent2 coloring)

#### Tables

| Classes | Description | 
|---|---|
| `table` | First column has a darker background and text is bolded
| `t-c` | Center tables
| `t-w` | Table expands to fill the whole width of the file
| `tbl-nalt` | Remove alternating row coloring from tables
| `tbl-b` | Add border lines to table

#### Tags

| Classes | Description | 
|---|---|
| `tag-notion` | Notion styled tags (rounded rectangle)
| `tag-bubble` | Round/pill style tags
| `tag-outline` | Outline style tags, no background color, it's now the tag line color
| `tag-text` | Tags are only colored text, no background color

# Ids 

`<s id="#col"></s>`

Classes | Description
---|---|
`#col` | Show/Create a color block
`#font` | Showcase a font in huge sized text
`#vid` | 16:9 aspect ratio for videos. Used before an iframe:<br>`<div id=vid><iframe></iframe></div>`

**Examples:**
![](https://i.imgur.com/FHYhFcR.png)
![](https://i.imgur.com/3cSv8c3.png)
