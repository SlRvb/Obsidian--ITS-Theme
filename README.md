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
    - **Image Positions:** Move images to either left, right, center, change types, etc.
        - Inspired by: [Lithou's Image Flags](https://github.com/Lithou/Sandbox/blob/main/.obsidian/snippets/pub-Image%20Flags.css)
        - *If you use lithou's snippet, this feature does conflict with it.*
- **\<i>\</i>** for images or other files attributions
    - Adds a different color to text within it to differentiate it from other text
    - Centered to match image centering
    - Adding: `alt="left"` and `alt="right"` within it will push the attribute to left and right of the screen.
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
- Embeds simplified

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

# Image Positions
**Clear**
`![[image.png|clear]]`: `clear` will allow that image to sit below another image if it's on the same side instead of sitting in the middle of the page.

**Cover** (Mostly for Complex Version)
`![[image.png|cover]]`: `cover` will allow for the resizing of the image to maintain aspect ratio and avoid stretching.

**Sizing** (Mostly for Complex Version)
`![[image.png|<>+<>|200]]`: Place the `|<numbers>` sizing at the *end* of the image line and it will shrink the image to that size.

## Simplified Version
**Left/Right**
`![[image.png|left]]`. `left` will move the image to the left.
`![[image.png|right]`. `right` will move the image to the right.

**Banner**
`![[image.png|banner]]`. `banner` will crop the image height-wise while setting the width to cover the entire page.

**Portrait**
`![[image.png|portrait]]`. `portrait` will crop the image width-wise while setting the height to a standard of about 400px.

**Profile**
*Not fully working unless you use the `pc` property.*
Profile will round the borders of the image to create a round image. 


## Complex Version
**Left/Right**
`![[image.png|locl]]`. `locl` will move the image to the left.
`![[image.png|locr]]`. `locr` will move the image to the right.

**Inner Image Position**
`![[image.png|pl]]`. `pl` will move the inside of the image to the left.
`![[image.png|pr]]`. `pr` will move the inside of the image to the right.
`![[image.png|pt]]`. `pt` will move the inside of the image to the top.
`![[image.png|pb]]`. `pb` will move the inside of the image to the bottom.
`![[image.png|pc]]`. `pc` will move the inside of the image to the center.

**Sizing**
`![[image.png|htiny]]`. `htiny` will resize the image to about 100px in height.
`![[image.png|hsmall]]`. `hsmall` will resize the image to about 200px in height.
`![[image.png|hmed]]`. `hmed` will resize the image to about 500px in height.
`![[image.png|htall]]`. `htall` will resize the image to about 700px in height.

`![[image.png|wtiny]]`. `wtiny` will resize the image to about 100px in width.
`![[image.png|wsmall]]`. `wsmall` will resize the image to about 200px in width.
`![[image.png|wmed]]`. `wmed` will resize the image to about 500px in width.
`![[image.png|wtall]]`. `wtall` will resize the image to about 700px in width.