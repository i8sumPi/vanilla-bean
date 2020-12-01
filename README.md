# Vanilla Bean JS
Do you ever feel tired of the long and cumbersome `document.getElementById()`? Do you want to replace it with something shorter, but you don't want to sacrifice that precious load time? Well struggle no more, and use Vanilla Bean Js!

## What Does It Do?
Shortens document.getElementById without sacrificing load time.

## How To Include It
If you already have JavaScript file, just include the simple one-liner at the start of your file:
```javascript
const el = id=>document.getElementById(id);
```
Now, instead of saying
`document.getElementById("myElement")`,
use
`el("myElement")`.
You can remember this because `el` is short of element. Using this method does not sacrifice load time because you are not including any extra files.


If, for some reason, you want to make this its own JavaScript file, include `vanilla-bean.js` as the first JavaScript file:
```html
<script src="path/to/vanilla-bean.js"></script>
<script src="other/javascript/files"></script>
```
or use
```html
<script src="https://raw.githubusercontent.com/i8sumPi/vanilla-bean/main/vanilla-bean.js"></script>
<script src="other/javascript/files"></script>
```

## Customization
If you want to rename the function, for example to `$`, use
```javascript
const $ = id=>document.getElementById(id);
```
Now, you can use `$("myElement")`.
