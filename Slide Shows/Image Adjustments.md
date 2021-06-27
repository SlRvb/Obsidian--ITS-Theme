## Image Adjustments
###### by [[SlRvb]]
Inspired by [Lithou's Image Flags](https://github.com/Lithou/Sandbox/blob/main/.obsidian/snippets/pub-Image%20Flags.css)

---
## Syntax
**General syntax formatting**: `![[Image.png|modifier+modifier|#]]`

*Example*: `![[Image.png|left+pt|200]]`

- `|` is required *after* the image extension and *before* Obsidian's sizing numbers
- `+` can be anything:
	- `![[Image.png|left-pt-sban|200]]`
	`![[Image.png|left_pt_sban|200]]`
	`![[Image.png|left|pt|sban|200]]`
	`![[Image.png|left pt sban|200]]`
	
---
## Simplified Version
Optimized for easier comprehension and "quicker" styling

`![[Image.png|left+small]]`

---
### Positions
`left`, `center`, `right`

![[Image Adjustments-Simple - Positions.png]]

---
### Types
Style of sizing for images.

||
---|---|
`banner` | Expand image to width of the page
`portrait` | Larger image height than image's width
`profile` | Width and height of the image are equal (Needs `pc`)

---
### Sizing
<i>⚠ **Note**: Obsidian's number sizing `|###` will **not** work with these.</i>

Format: `![[Image.png|modifier+size]]`

Banner & Portrait use `+small` and `+tall` sizing, but Profile uses `+medium` only.

---