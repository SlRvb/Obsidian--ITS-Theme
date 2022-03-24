
# Callouts

Type | Description |
---|---|
`[!infobox]` | Wikipedia-like infoboxes
`[!captions]` | Displays text around image in the style of a caption
`[!kanban]` | Displays a (functionally limited) kanban board
`[!grid]` | Best type of image grid for internally linked images
`[!masonry]` | Best type of image grid for externally linked images
`[!recite]` | A D&D styled popout 
`[!metadata]` | Styled callout that colors \*\*bold\*\* words, table headers, and inline dataview keys blue


#### Adjustments
```
> [!callout-type adjustment]

> [!kanban nt]
> [!kanban no-title]
> [!caption left]
```

| Abbr. | Full Title | Description|
|---|---|---|
| `no-t` | `no-title` | Hides callout title
| `n-th` |`no-table-header` | Hides table header in callouts

---
> **Yaml css classes** to style different on per page basis

| cssclass | Description |
|---|---|
| `alt-co` | Alternate Callout Styling, use callout color as background color
| `co-ttl-ctr` | Center callout titles

> **Callouts uses the same [parameters](Image-Positions#sizing) as the images for resizing (width-wise) and [moving it](Image-Positions#leftrightcenter).**