# Context Menu

Use this repository as cdn

```html
<script src="https://cdn.jsdelivr.net/gh/shashfrankenstien/lib-contextmenujs/lib-contextmenu.js"></script>
```
```html
<script src="https://cdn.jsdelivr.net/gh/shashfrankenstien/lib-contextmenujs@v0.0.1/lib-contextmenu.js"></script>
```

Try the minified version
```html
<script src="https://cdn.jsdelivr.net/gh/shashfrankenstien/lib-contextmenujs/lib-contextmenu.min.js"></script>
```
```html
<script src="https://cdn.jsdelivr.net/gh/shashfrankenstien/lib-contextmenujs@v0.0.1/lib-contextmenu.min.js"></script>
```

# Usage

```js
document.getElementById('element').addEventListener('contextmenu', (e)=>{
    e.preventDefault()
    let menu = new ContextMenu(e.clientX, e.clientY)
    menu.addNewOption("Option 1", ()=>{
        alert("You chose Option 1")
        menu.close()
    })
    menu.addNewOption("Option 2", ()=>{
        alert("You chose Option 2")
        menu.close()
    })
    menu.open()
})

```

# Example

[lib-contextmenujs](https://shashfrankenstien.github.io/lib-contextmenujs/)
