# CSS

## Box Model

- box-sizing: border-box

## Layout

### The display Property

1. display: block
1. display: inline

```html
<span>
  <a> <img /></a>
</span>
```

> `display: inline-block`
> allows to set a width and height on the element

1. display: none

> `visibility: hidden`
> still take up the same space as before

### float and clear

```css
.clearfix::after {
  content: "";
  clear: both;
  display: table;
}
```

### flex
