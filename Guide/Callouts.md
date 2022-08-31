
# Callouts
> **[Get Callout Snippet](https://github.com/SlRvb/Obsidian--ITS-Theme/blob/main/Snippets/S%20-%20Callouts.css)**

---

| Type | Description |
| --- | --- |
| `[!infobox]` | Wikipedia-like infoboxes: [How to Format](Callouts.md#infoboxes) |
| `[!captions]` | Displays text around image in the style of a caption |
| `[!kanban]` | Displays a (functionally limited) kanban board: [How to Format](Callouts.md#kanban) |
| `[!grid]` | Display images in a grid/masonry style: [How to Format](Callouts.md#image-grid) |
| `[!recite]` | A D&D styled popout |
| `[!metadata]` | Styled callout that colors \*\*bold\*\* words, table headers, and inline dataview keys blue |
| `[!cards]` | Style images and dataview tables like notion's gallery view: [How to Format](Callouts.md#cards) |
| `[!table]` | Prevent table from wrapping |
| `[!aside]` | Add asides to the side of notes |
| `[!timeline]` | Style callout as a vertical Timeline [How to Format](Callouts.md#timeline) |
| `[!column]` | Style inner callouts as columns: [How to Format](Callouts.md#column) |

# Adjustments
**Format Syntax:**
```
> [!callout-type|adjustment adjustment2]

> [!kanban|n-t]
> [!kanban|no-title txt-c]
> [!caption|left]
```

---

> **Callouts uses the same [parameters](Image-Positions.md#sizing) as the images for resizing (width-wise) and [moving it](Image-Positions.md#leftrightcenter).**

| Abbr. | Full Title | Description |
| --- | --- | --- |
| `no-t` | `no-title` | Hides callout title |
| `s-t` | `show-title` |  |
| `n-th` | `no-table-header` | Hides table header in callouts |
| `no-i` | `no-icon` | Hide callout icon |
| `txt-c` | `text-Center` | Center callout text |
| `ttl-c` | `title-Center` | Center callout title text |
| `embed` |  | Remove callout padding to expand embed |
| `nmg` | `no-margin` | Remove callout margins |
| `clean` |  | Remove callout Styling |
| `alt-co` |  | Alternate Callout styling for individual callouts |
| `alt-line` |  | Minimalistic callout style with only title underlined |
| `dim` |  | Dim collapsible (`+`/`-`) callouts unless hovered and opened |
| `dim-hvr` |  | Dim callout unless hovered |
| `collapse` |  | Remove all padding and margins for ultra compact look |
| `t-w` | `table-wide` | Widen table to edges of callout |
| `tbl-cln` | `table-clean` | Remove most table styling: lines, background colors |

---

> **Yaml css classes** to style different on per page basis

| cssclass | Description |
|---|---|
| `alt-co` | Alternate Callout Styling, use callout color as background color
| `co-ttl-ctr` | Center callout titles

## Colors

| Abbr. | Full Title | Description |
| --- | --- | --- |
| `c-` | `color-` | Change callout title/border color |
| `bg-` | `background-` | Change callout background color |
| `bg-c-` | `background-color-` | Change callout title and background color |

- **Colors:**
	- purple
	- blue
	- green
	- red
	- pink
	- orange
	- yellow
	- gray

**Syntax:**
```markdown
> [!recite|color-blue]

> [!recite|background-blue]

> [!recite|background-color-blue]
```

```markdown
> [!recite|c-purple]

> [!recite|bg-purple]

> [!recite|bg-c-purple]
```

# Formatting

## Infoboxes
```markdown
> [!infobox]
> # Name
> ![[Image.png|cover hsmall]]
> ###### Stats
> | Type |  Stat |
> |---|---|
> | Test | Testing |
> | Test | Testing |
> | Test | Testing |
> | Test | Testing |
```

```markdown
> [!infobox]+ Collapsible Infobox
> # Name
> ![[Image.png|cover hsmall]]
> ###### Stats
> | Type |  Stat |
> |---|---|
> | Test | Testing |
> | Test | Testing |
> | Test | Testing |
> | Test | Testing |
```

```markdown
> [!infobox|left]
> # Name
> ![[Image.png|cover hsmall]]
> ###### Stats
> | Type |  Stat |
> |---|---|
> | Test | Testing |
> | Test | Testing |
> | Test | Testing |
> | Test | Testing |
```

## Image Grid
| | |
| --- | --- |
| `[!grid]` | Best type for **internally linked** images |
| <code>[!grid\|masonry]</code> | Best type for **externally linked** images |

```markdown
> [!grid]
> ![[Internal Image.png]]
> ![[Internal Image 2.png]]
>
> ![[Internal Image 3 on New Row.png]]


> [!grid|masonry]
> ![External Image 1](https://www.dmuth.org/wp-content/uploads/2021/03/obsidian-logo.png)
> ![External Image 2](https://www.dmuth.org/wp-content/uploads/2021/03/obsidian-logo.png)
> 
> ![External Image 3 on New Row](https://www.dmuth.org/wp-content/uploads/2021/03/obsidian-logo.png)
```


## Kanban
```markdown
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
```markdown
> [!cards]
> **[[Link]]**
> ![Image link|sban htiny ctr](https://images.unsplash.com/photo-1574375927938-d5a98e8ffe85?ixlib=rb-1.2.1&q=85&fm=jpg&crop=entropy&cs=srgb&w=1200)
> 
> **[[Link]]**
> ![[Image Link.png|sban htiny ctr]]
```

**Add More Columns:**
```markdown
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
````markdown
> [!cards|dataview]
> ```dataview
> TABLE WITHOUT ID
> 	"![|sban cover hmicro](" + image + ")" as Image,
> 	"**"+ file.link + "**" AS "Column Name",
> FROM "folder"
> SORT file.name
> LIMIT 10
> ```
````

## Column
| Adjustment | Description |
| --- | --- |
| `flex` | Wrap column on smaller width screens |
| `3`, `4` | Add more columns; Default is 2 |
| `dataview` | Styles dataview LISTs into columns <br>(column numbers work with this as well) |

```markdown
> [!column]
>> [!info] Column 1
>> - Use another callout for columns
>
>> [!note] Column 2
>> Need that singular blockquote `>` as separation between columns
```

```markdown
> [!column|flex 3]
>> [!info|no-t] 
>> Column 1
>
>> [!important]+ Current Topics
>> Column 2
```

````markdown
> [!column|dataview 3] 3 Columns for Dataview List
> ```dataview
> LIST
> FROM ""
> LIMIT 20
> ```
````

## Timeline
| Adjustment | Description |
| --- | --- |
| `t-l` | Timeline callout left side |
| `t-r` | Timeline callout right side |
| | |
| `t-1` to `t-10` | Add some spacing above the timeline callout to simulate how close events are in time |

```markdown
> [!timeline|t-l] **Title** _Subtitle_
> Left aligned timeline piece

> [!timeline|t-r t-4] **Title** *Subtitle*
> Right aligned timeline piece

> [!timeline|t-r t-10] **Title** *Subtitle*
> Spaced timeline piece
```

## Asides
| Adjustment | Description |
| --- | --- |
| `show-title` | Brings back callout title for Asides |
| `clean` | Remove Aside styling |
| `tufte` | Tufte Aside styling (WIP, somewhat buggy) |
| `left` | Move aside left |
| `right` | Move aside right |

```markdown
> [!aside|clean right]
> Removes styling from aside

> [!aside|tufte]+ 
> Tufte styled aside callout

> [!aside|tufte title]
> Show callout title for asides
```

