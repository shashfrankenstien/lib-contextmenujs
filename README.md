# HTML Table Filter!!

Use this repository as cdn

```html
<script src="https://cdn.jsdelivr.net/gh/shashfrankenstien/lib-contextmenujs/lib-contextmenu.js"></script>
```
```html
<script src="https://cdn.jsdelivr.net/gh/shashfrankenstien/lib-contextmenujs@v0.0.5/lib-contextmenu.js"></script>
```

Try the minified version
```html
<script src="https://cdn.jsdelivr.net/gh/shashfrankenstien/lib-contextmenujs/lib-contextmenu.min.js"></script>
```
```html
<script src="https://cdn.jsdelivr.net/gh/shashfrankenstien/lib-contextmenujs@v0.0.5/lib-contextmenu.min.js"></script>
```

# Usage

```html
<div id="table-container">
    <h2>Context Menu</h2>
    <span>Right Click</span>

    <input type="text" placeholder="filter">

    <span></span>

    <table>
        ...
    </table>
</div>

</body>

<script src="lib-tablefilter.js" ></script>

<script>
    const table = document.querySelector("#table-container table")
    const filter = document.querySelector("#table-container input")
    const filter_status = document.querySelector("#table-container span")
    options = {
        persist: false,                     // 'true' is the default
        focus: true,                        // 'true' is the default
        input_active_bg: "red"              // background color of input element when a filter is active
    }
    const tf = new TableFilter(table, filter, filter_status, options) // filter_status and options are optional
</script>

```

# Example

[lib-contextmenujs](https://shashfrankenstien.github.io/lib-contextmenujs/)
