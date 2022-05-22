
# Callouts
> **[Get Callout Snippet](https://github.com/SlRvb/Obsidian--ITS-Theme/blob/main/S%20-%20Callouts.css)**

---

Type | Description |
---|---|
`[!infobox]` | Wikipedia-like infoboxes
`[!captions]` | Displays text around image in the style of a caption
`[!kanban]` | Displays a (functionally limited) kanban board: [How to Format](Callouts#Kanban.md)
`[!grid]` | Best type of image grid for internally linked images
`[!masonry]` | Best type of image grid for externally linked images
`[!recite]` | A D&D styled popout 
`[!metadata]` | Styled callout that colors \*\*bold\*\* words, table headers, and inline dataview keys blue
`[!cards]` | Style images and dataview tables like notion's gallery view: [How to Format](Callouts#Cards.md)
`[!table]` | Prevent table from wrapping
`[!aside]` | Add asides to the side of notes
`[!timeline]` | Style callout as a vertical Timeline [How to Format](Callouts#Timeline.md)
`[!column]` | Style inner callouts as columns: [How to Format](Callouts#Column.md)

#### Adjustments
**Format Syntax:**
```
> [!callout-type|adjustment adjustment2]

> [!kanban|nt]
> [!kanban|no-title txt-c]
> [!caption|left]
```

---

> **Callouts uses the same [parameters](Image-Positions#sizing) as the images for resizing (width-wise) and [moving it](Image-Positions#leftrightcenter).**

| Abbr. | Full Title | Description|
|---|---|---|
| `no-t` | `no-title` | Hides callout title
| `n-th` | `no-table-header` | Hides table header in callouts
| `no-i` | `no-icon` | Hide callout icon
| `txt-c` | | Center callout text
| `embed` | | Remove callout padding to expand embed
| `nmg` | `no-margin` | Remove callout margins
| `clean` | | Remove callout Styling
| `alt-co` | | Alternate Callout styling for individual callouts
| `alt-line` | | Minimalistic callout style with only title underlined |

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
> Might want to install the [Image Adjustments snippet](https://github.com/SlRvb/Obsidian--ITS-Theme/blob/main/S%20-%20Images%20Adjustments.css) to control the images sizing

- Blank Line `>` separated
- `**Bold**` syntax will center text and and a background color (no background color for dataview tables)

| Adjustment | Description |
| --- | --- |
| `2`, `4`, `5` | Change number of columns; 3 is default |
| `dataview` | Style dataview table and lists as cards |
| `dvl` | Style dataview list

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

## Column
| Adjustment | Description |
| --- | --- |
| `flex` | Wrap column on smaller width screens
| `3`, `4` | Add more columns; Default is 2

```yaml
> [!columns|flex 3]
>> [!info|no-t] 
>> Column 1
>
>> [!important]+ Current Topics
>> Column 2
```

## Timeline
| Adjustment | Description |
| --- | --- |
| `t-l` | Timeline callout left side |
| `t-r` | Timeline callout right side |


```yaml
> [!timeline|t-l] **Title** _Subtitle_
> Left aligned timeline piece

> [!timeline|t-r] **Title** *Subtitle*
> Right aligned timeline piece
```

## Asides
| Adjustment | Description |
| --- | --- |
| `title` | Brings back callout title for Asides |
| `clean` | Remove Aside styling |
| `tufte` | Tufte Aside styling (WIP, somewhat buggy) |
| `left` | Move aside left |
| `right` | Move aside right |

```md
> [!aside|clean right]
> Removes styling from aside

> [!aside|tufte]+ 
> Tufte styled aside callout

> [!aside|tufte title]
> Show callout title for asides
```