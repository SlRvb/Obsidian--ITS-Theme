# Image Positions
Obsidian internal images `![[]]` will change immediately, but for external images `![]()`, the page needs to be reopened to see the changes. 

### Clear

Example | Description |
---|---|
`![[image.png\|clear]]`| `clear` will allow that image to sit below another image<br>If it's on the same side instead of sitting in the middle of the page.

### Image Grid

Example | Description |
---|---|
`![[image.png\|grid]]` | `grid` will allow that image and others with this to display side-by-side in a grid

![](../Images/Image_Adjustments-Image-Grids.png)

### Cover (Mostly for Customizable Version)

Example | Description |
---|---|
`![[image.png\|cover]]`| `cover` will resize the image, maintain aspect ratio and avoid stretching.

### Sizing (Mostly for Customizable Version)

Example | Description |
---|---|
`![[image.png\|loc\|sban\|200]]`| Place the `\|<numbers>` sizing at the *end* of the text and it will shrink the image to that size.


## Simplified Version

### Left/Right/Center

Example | Description |
---|---|
`![[image.png\|left]]`| `left` will move the image to the left.
`![[image.png\|right]`| `right` will move the image to the right.
`![[image.png\|ctr]`| `ctr` will move the image to the center.

![](../Images/Image_Adjustments-Simple-Positions.png)


### Types

![](../Images/Image_Adjustments-Simple-Sizing.png)

#### Banner

Example | Description |
---|---|
`![[image.png\|banner]]`| `banner` will crop the image height-wise to about 150px while setting the width to cover the entire page.
`![[image.png\|banner+small]]`| `banner+small` will crop the image height-wise to about 100px while setting the width to cover the entire page.
`![[image.png\|banner+tall]]`| `banner+tall` will crop the image height-wise to about 500px while setting the width to cover the entire page.


#### Portrait

Example | Description |
---|---|
`![[image.png\|portrait]]`| `portrait` will crop the image width-wise to about 40% while setting the height to a standard of about 400px.
`![[image.png\|portrait+small]]`| `portrait+small` will crop the image width-wise to about 20% while setting the height to a standard of about 200px.
`![[image.png\|portrait+tall]]`| `portrait+tall` will crop the image width-wise to about 50% while setting the height to a standard of about 500px.


#### Profile

Example | Description |
---|---|
`![[image.png\|profile]]`| `profile` will round the borders of the image to create a round image and size it to about 100px.
`![[image.png\|profile+medium]]`| `profile+medium` will round the borders of the image to create a round image and resize it to about 250px.


## Customizable Version
### Left/Right

Example | Description |
---|---|
`![[image.png\|locl]]`| `locl` will move the image to the left.
`![[image.png\|locr]]`| `locr` will move the image to the right.


### Inner Image Position

![](../Images/Image_Adjustments-Custom-Inner_Position_Precise.png)

Example | Description |
---|---|
`![[image.png\|pl]]`| `pl` will move the inside of the image to the left.
`![[image.png\|pr]]`| `pr` will move the inside of the image to the right.
`![[image.png\|pt]]`| `pt` will move the inside of the image to the top.
`![[image.png\|pb]]`| `pb` will move the inside of the image to the bottom.
`![[image.png\|pc]]`| `pc` will move the inside of the image to the center.


> These will inch the images around if the ^ above syntax isn't enough.

Example | Description |
---|---|
`![[image.png\|p+cr]]`| `p+cr` will move the inside of the image to the center right.
`![[image.png\|p+cl]]`| `p+cl` will move the inside of the image to the center left.
||
`![[image.png\|p+ct]]`| `p+ct` will move the inside of the image to the center top of the image.
`![[image.png\|p+cct]]`| `p+cct` will move the inside of the image to the center top, slightly higher than `p+ct`|
`![[image.png\|p+tc]]`| `p+tc` will move the inside of the image to the center top, slightly lower than `pt`|
`![[image.png\|p+tcc]]`| `p+tcc` will move the inside of the image to the center top, slightly lower than `p+tc`|
||
`![[image.png\|p+cb]]`| `p+cb` will move the inside of the image to the center bottom of the image.
`![[image.png\|p+ccb]]`| `p+ccb` will move the inside of the image to the center bottom, slightly lower than `p+cb`|
`![[image.png\|p+bc]]`| `p+bc` will move the inside of the image to the center bottom, slightly higher than `pb`|
`![[image.png\|p+bcc]]`| `p+bcc` will move the inside of the image to the center bottom, slightly higher than `p+bc`|

### Sizing
![](../Images/Image_Adjustments-Custom-Sizing.png)

Example | Description |
---|---|
`![[image.png\|htiny]]`|`htiny` will resize the image to about 100px in height.
`![[image.png\|hsmall]]`| `hsmall` will resize the image to about 200px in height.
`![[image.png\|hs-med]]`| `hs-med` will resize the image to about 300px in height.
`![[image.png\|hm-sm]]`| `hm-sm` will resize the image to about 400px in height.
`![[image.png\|hmed]]`| `hmed` will resize the image to about 500px in height.
`![[image.png\|hm-tl]]`| `hm-tl` will resize the image to about 600px in height.
`![[image.png\|htall]]`| `htall` will resize the image to about 700px in height.
||
`![[image.png\|wtiny]]`| `wtiny` will resize the image to about 100px in width.
`![[image.png\|wsmall]]`| `wsmall` will resize the image to about 200px in width.
`![[image.png\|ws-med]]`| `ws-med` will resize the image to about 300px in width.
`![[image.png\|wm-sm]]`| `wm-sm` will resize the image to about 400px in width.
`![[image.png\|wmed]]`| `wmed` will resize the image to about 500px in width.
`![[image.png\|wm-tl]]`| `wm-tl` will resize the image to about 600px in width.
`![[image.png\|wtall]]`| `wtall` will resize the image to about 700px in width.
