# Folder Styles Snippet
> Change the colors of your folders with the [Folder Styles Snippet](https://github.com/SlRvb/Obsidian--ITS-Theme/blob/main/S%20-%20Folder%20Styles.css)

![Image](https://media.discordapp.net/attachments/855181471643861002/930586979295453184/Obsidian_kszRvt3fwb.gif)

**Resources to help with icons:**
- [Search for icons using Iconify](https://iconify.design/icon-sets/)
- [Convert the SVG code into CSS ready code](https://yoksel.github.io/url-encoder/)

# How To
> **⚠ NOTE:** This snippet *will* require a bit of manual work. I do not recommend using it if you change your folders often.

1. Open the **Folder Styles snippet** and copy the template code around line 57:
```css
/*----Template Code----*/
/*--Add Icons--*/
.nav-folder-title[data-path=""] .nav-folder-title-content::before {
    content: url();
}

/*--Folder Color Styling--*/
/*Color Root Folder*/
.nav-folder-title[data-path=""] { /*Add "folder title"*/
    color: var(--c);              /*change to your variable*/
    background: var(--c2);
    border-bottom: 2px solid var(--c2);
}
/*Color Sub Folder Lines*/
.nav-folder-title[data-path*=""],
.nav-folder-title[data-path*=""] + .nav-folder-children,
.nav-file-title[data-path*=""] { 
    border-left: 3px solid var(--c2); 
    margin-left: -3px; 
}
/*Color Sub Folder Lines When Hovering Over Folder*/
.nav-folder-title[data-path*=""]:hover,
.nav-folder-title[data-path*=""] + .nav-folder-children:hover,
.nav-file-title[data-path*=""]:hover { 
    border-color: var(--c);
}
/*Opened Root Folder Background Color & Bottom Border*/
.nav-folder.mod-root > .nav-folder-children > .nav-folder > .nav-folder-title[data-path^=""] + .nav-folder-children {
    background-color: var(--c-t);
    border-bottom: 2px solid var(--c2);
}

```

2. Paste this under the line that says `Add Your Folder CSS Here` around line 156

3. Add the name of your folder to *all* the `data-path=""`. For example:
```css
.nav-folder-title[data-path="Example Folder Title"] .nav-folder-title-content::before {}

.nav-folder-title[data-path*="Example Folder Title"] {}
```

4. To change colors/icons, go back to line 30 that reads `Theme: Add Your Colors and Icons Here`
	- Add as many other variables here as you need for your folders. `--c`/`--i` is a placeholder variable just for the example later.
	
	- Call it whatever you want: `--root-folder-color`, `--ttrpg-folder`, `--pink`.
	
	- `--c` is text color, <br> `--c2` is the background color of the root folder, and <Br> `--c-t` is the translucent background color of the opened folder
```css
/*Theme: Add Your Colors and Icons Here*/
.theme-dark {
    /*Add your icon here for easy referencing.
    Change i to whatever variable name you want*/
    --i: url(""); 

    /*Add your folder colors here. 
    Change c to whatever variable name you want*/
    --c: gray;
    --c2: #000000;
    --c-t: #00000030; /*This is the Root Folder background color*/
}

.theme-light {
    /*Add your icon here for easy referencing.
    Change i to whatever variable name you want*/
    --i: url(""); 
    
    /*Add your folder colors here. 
    Change c to whatever variable name you want*/
    --c: gray;
    --c2: #000000;
    --c-t: #00000030; /*This is the Root Folder background color*/
}
```

# Example CSS:

Shown around line 97
```css
/*----Example (Delete Me Later)----*/
.theme-dark {
    /*Darkmode Icon*/
    --f-i: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' aria-hidden='true' focusable='false' width='16px' height='16px' style='vertical-align: -0.125em;-ms-transform: rotate(360deg); -webkit-transform: rotate(360deg); transform: rotate(360deg);' preserveAspectRatio='xMidYMid meet' viewBox='0 0 24 24'%3E%3Cpath fill='none' stroke='%238e93a7' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='M16.5 19a2.5 2.5 0 1 0 0-5a2.5 2.5 0 0 0 0 5zM10 5l2-2m-4.5 7a2.5 2.5 0 1 0 0-5a2.5 2.5 0 0 0 0 5zm.5 6l8-8M5.5 21a2.5 2.5 0 1 0 0-5a2.5 2.5 0 0 0 0 5zm13-13a2.5 2.5 0 1 0 0-5a2.5 2.5 0 0 0 0 5zM12 21l2-2'/%3E%3Crect x='0' y='0' width='24' height='24' fill='rgba(0, 0, 0, 0)' /%3E%3C/svg%3E");
    
    /*Darker Color for 2*/
    --f-c: #5d7085;
    --f-c2: #000000;
}

.theme-light {
    /*Lightmode Icon*/
    --f-i: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' aria-hidden='true' focusable='false' width='16px' height='16px' style='vertical-align: -0.125em;-ms-transform: rotate(360deg); -webkit-transform: rotate(360deg); transform: rotate(360deg);' preserveAspectRatio='xMidYMid meet' viewBox='0 0 24 24'%3E%3Cpath fill='none' stroke='%238e93a7' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='M16.5 19a2.5 2.5 0 1 0 0-5a2.5 2.5 0 0 0 0 5zM10 5l2-2m-4.5 7a2.5 2.5 0 1 0 0-5a2.5 2.5 0 0 0 0 5zm.5 6l8-8M5.5 21a2.5 2.5 0 1 0 0-5a2.5 2.5 0 0 0 0 5zm13-13a2.5 2.5 0 1 0 0-5a2.5 2.5 0 0 0 0 5zM12 21l2-2'/%3E%3Crect x='0' y='0' width='24' height='24' fill='rgba(0, 0, 0, 0)' /%3E%3C/svg%3E");

    /*Darker Color for 1*/
    --f-c: #000000;
    --f-c2: #5d7085;
}
.nav-folder-title[data-path*="Template"] .nav-folder-title-content::before {
    content: var(--f-i);
}
.nav-folder-title[data-path="Template"] { 
    color: var(--f-c);             
    background: var(--f-c2);
    border-bottom: 2px solid var(--f-c2);
}
.nav-folder-title[data-path*="Template"],
.nav-folder-title[data-path*="Template"] + .nav-folder-children,
.nav-file-title[data-path*="Template"] { 
    border-left: 3px solid var(--f-c2); 
    margin-left: -3px; 
}
.nav-folder-title[data-path*="Template"]:hover,
.nav-folder-title[data-path*="Template"] + .nav-folder-children:hover,
.nav-file-title[data-path*="Template"]:hover { 
    border-color: var(--f-c);
}
.nav-folder.mod-root > .nav-folder-children > .nav-folder > .nav-folder-title[data-path^="Template"] + .nav-folder-children {
    background-color: var(--c-t);
    border-bottom: 2px solid var(--c2);
}

/*----Example End (Delete Me)----*/
```