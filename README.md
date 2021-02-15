# ITS Theme
*By SlRvb*

Theme for my Obsidian Story Vault: ***In The Shadows.***


# Features
- Dark and Light mode compatible
- Colored Graph
- Squared Edges
- **Heading:**
    - **Underline**: spans across the page depending on the heading
    - **Font:** Calisto MT
    - **Embeded:** Embedded files have smaller headers and are 1 color
- Custom Horizontal line
    - *Credit:* [TriDiamond](https://forum.obsidian.md/t/meta-post-common-css-hacks/1978/223)
- Tag Pills (Rectangular)
- Metadata minimal style
- Checkboxes
    - *Credit:* [Kepano: Nicer Checkboxes](https://forum.obsidian.md/t/nicer-checkboxes/2238)
- **Images:**
    - Images Centered
    - **Zoom:** images enlarges upon clicking and holding it 
        - *Credit:* [Kepano: Image Zoom Click Hold To Expand Images](https://forum.obsidian.md/t/image-zoom-click-hold-to-expand-images/5164)
    - **Gallery/Masonry:** Side by side images.
        - Put `cssclass: img-grid` into frontmatter/YAML, separate by adding spaces
        - *Credit*: [Kepano: Display side by side image grid (CSS snippet)](https://forum.obsidian.md/t/display-side-by-side-image-grid-css-snippet/9359)
- **\<i>\</i>** for images or other files attributions
    - Adds a different color to text within it to differentiate it from other text
    - Centered to match image centering
- **Blockquotes**
    - Soft background
    - Wider blockquote
    - Quotation marks added top right corner
- **Popover**
    - Larger Popover
    - Images fit within the popover window
    - Images are cropped in popover window
- **Line Relationships**
    - Bullet Points
        - *Credit:* [Lizardmenfromspace](https://forum.obsidian.md/t/meta-post-common-css-hacks/1978/2)
    - Outline Pane
    - Folder Navigation
    - Tag Pane 
        - *Note: Dot appears at bottom left corner. If it's too annoying add this snippet:*
        - ```.tag-container .tree-item-children {border-left: 0px;}```
- **Folder Navigation Icons**
    - Credit: [Deathau](https://forum.obsidian.md/t/meta-post-common-css-hacks/1978/109)
- **Text Wrapping**
    - Outline Pane
    - Tag Pane
    - File Explorer Sidebar
    - Embed Titles
    - Query Titles

*Folder Icons based on Folder Title not included, use this to add your own icons:*
```
.nav-folder-title[data-path="<Folder name here>"] .nav-folder-title-content::before {
  content: "<Emoji here> ";
  font-size:1.3em;
}
```

# Preview

## Darkmode

![](Darkmode.png)

**Features**
![](Darkmode-Features.png)
**Edit Mode**
![](Darkmode-Editing.png)

## Lightmode

![](Lightmode.png)

**Features**
![](Lightmode-Features.png)
**Edit Mode**
![](Lightmode-Editing.png)
