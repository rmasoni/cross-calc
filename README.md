# cross-calc

Sass mixin for cross-browser `calc()`. Hopefully we won't need this in the near future.

## Example

This code:

```sass
@import "cross-calc"

div
  +calc(width, "100% - 200px")
```

Compiles to:

```css
div {
  width: -moz-calc(100% - 200px);
  width: -webkit-calc(100% - 200px);
  width: calc(100% - 200px);
}
```
