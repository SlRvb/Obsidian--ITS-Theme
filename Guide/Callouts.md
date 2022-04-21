
# Callouts
[Get Callout Snippet](https://github.com/SlRvb/Obsidian--ITS-Theme/blob/main/S%20-%20Callouts.css)

Type | Description |
---|---|
`[!infobox]` | Wikipedia-like infoboxes
`[!captions]` | Displays text around image in the style of a caption
`[!kanban]` | Displays a (functionally limited) kanban board: [How to](Callouts#Kanban)
`[!grid]` | Best type of image grid for internally linked images
`[!masonry]` | Best type of image grid for externally linked images
`[!recite]` | A D&D styled popout 
`[!metadata]` | Styled callout that colors \*\*bold\*\* words, table headers, and inline dataview keys blue
`[!cards]` | Style images and dataview tables like notion's gallery view: [How to](Callouts#Cards)
`[!table]` | Prevent table from wrapping

#### Adjustments
```
> [!callout-type|adjustment adjustment2]

> [!kanban|nt]
> [!kanban|no-title]
> [!caption|left]
```

| Abbr. | Full Title | Description|
|---|---|---|
| `no-t` | `no-title` | Hides callout title
| `n-th` |`no-table-header` | Hides table header in callouts
| `2`, `4` | | Change number of columns for [[#Cards]]

> **Callouts uses the same [parameters](Image-Positions#sizing) as the images for resizing (width-wise) and [moving it](Image-Positions#leftrightcenter).**


---

> **Yaml css classes** to style different on per page basis

| cssclass | Description |
|---|---|
| `alt-co` | Alternate Callout Styling, use callout color as background color
| `co-ttl-ctr` | Center callout titles

# Formatting

## Infoboxes
```md
> [!infobox]+
> # Name
> ![[Image.png|cover hsmall]]
> ###### Stats
> Type |  Stat |
> ---|---|
> Test | Testing |
> Test | Testing |
> Test | Testing |
> Test | Testing |
```

```md
> [!infobox|left]+
> # Name
> ![[Image.png|cover hsmall]]
> ###### Stats
> Type |  Stat |
> ---|---|
> Test | Testing |
> Test | Testing |
> Test | Testing |
> Test | Testing |
```

## Kanban
```md
> [!kanban]+
> - [[Link|Lane 1 Title]]
> 	- ![[Image.png]]
> 	- [[Link|Card]]
> - [[Link|Lane 2 Title]]
> 	![[Image without background card styling.png]]
> 	- [[Link|Card]]
```

## Cards
> Might want to install the [Image Adjustments ](Image-Positions) snippet to control the images sizing

- Blank Line `>` separated
- `**Bold**` syntax will center text and and a background color (no background color for dataview tables)

**External and Internal Images:**
```md
> [!cards]
> **[[Link]]**
> ![Image link|sban htiny ctr](https://images.unsplash.com/photo-1574375927938-d5a98e8ffe85?ixlib=rb-1.2.1&q=85&fm=jpg&crop=entropy&cs=srgb&w=1200)
> 
> **[[Link]]**
> ![[Image Link.png|sban htiny ctr]]
```

**Add More Columns:**
```md
> [!cards|4]
> **[[Link]]**
> ![Image link|sban htiny ctr](https://images.unsplash.com/photo-1574375927938-d5a98e8ffe85?ixlib=rb-1.2.1&q=85&fm=jpg&crop=entropy&cs=srgb&w=1200)
> 
> **[[Link]]**
> ![[Image Link.png|sban htiny ctr]]
> 
> **[[Link]]**
> ![Image link|sban htiny ctr](https://images.unsplash.com/photo-1574375927938-d5a98e8ffe85?ixlib=rb-1.2.1&q=85&fm=jpg&crop=entropy&cs=srgb&w=1200)
> 
> **[[Link]]**
> ![[Image Link.png|sban htiny ctr]]
```

**Style Dataview Table:**
```md
> [!cards|dataview]
> ```dataview
> TABLE WITHOUT ID
> 	"![|sban cover hmicro](" + image + ")" as Image,
> 	"**"+ file.link + "**" AS "Column Name",
> FROM "folder"
> SORT file.name
> LIMIT 10
> ```
```
