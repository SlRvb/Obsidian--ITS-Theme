## Aside
###### by [SlRvb](https://SlRvb.github.io/Site/)

Inspired by [Palatinate's Aside CSS](https://github.com/eleanorkonik/-palatinate/blob/main/aside.css)

---

## Syntax
**HTML:** `<s class="aside-type"></s>`

<s class=aside-in>**⚠Note:** ITS Theme/Image Position Snippet uses `<i></i>` for other type's of formatting which may result in strange styling.
	
	The ITS Theme also uses `<b></b>`.</s>
- Can use other html types that supports markdown:
	- `<i></i>`
	- `<u></u>`
	- `<b></b>`

---

## Types

Type Syntax | Description|
---|:---|
`aside-in` | Displays aside *within* the page, <br> shifts text to wrap around the aside.
`aside-show` | Displays aside on the right edge of the page, <br> doesn't move text
`aside-hide` | Displays aside at the right edge of page as an icon, <br> hovering will show aside content


---

## Supported/Unsupported Markdown
(As far as I know)

-  `![[Embeds]]`
-  `**Bold**`
-  `*Italics*`
-  `[Markdown Links]()`

**Don't work:**
-  `# Headings` will not work within asides must be HTML versions.