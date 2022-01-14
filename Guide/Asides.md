# Aside
> Add comments/asides within text that supports _most_ markdown syntax.

### Syntax
Recommend using `<s class="aside-">Text</s>` to keep markdown formatting (For Reading Mode).

```markdown
<s class="aside-hide">Text</s>

<s class="aside-show">==**Title**==
Text goes in here
</s>
```

### Class Types

Class | Description |
---|---|
`aside-show` | Aside content will be shown in the margin of the page.
`aside-hide` | Aside content will be hidden and only display an icon 🗨.<br>To see comment, hover over the icon
`aside-in` | Aside content will be embedded inside the page.
`aside-clean` | Aside content that doesn't have the stylized box.

### Examples
Aside code is highlighted.
![](../Images/Aside-Snippet.png)

# Supported Markdown
###### Markdown Supported:
```md
Text
**Bolded Text**
~~Strikethrough Text~~
*Italic Text*
==Highlighted Text==
[[Links]]
`Inline code`
[Markdown Links](https://github.com/SlRvb/Obsidian--ITS-Theme#aside)\
<b>Alternate Blockquotes</b>
<i>Personal `<i></i>` adjustments</i>

Images: ![[Where on Sovera.svg|invertb]]
Embeds: ![[In The Shadows|hsmall]]
```

###### Unsupported Markdown:

-   Lists
-   Headings
-   Code Blocks
-   Blockquotes