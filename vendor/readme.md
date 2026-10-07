To build the vendor library:

Run from the plugin root:

```sh
npx -p webpack@5 -p webpack-cli@5 webpack --mode none --config vendor/webpack.config.json --entry ./vendor/vendor.js --output-path vendor --output-filename bundle.js
```

To use the library:

```html
<script src='bundle.js'></script>
<script>
window.AdminPowerTools.Sortable
// or
AdminPowerTools.Sortable
</script>
```