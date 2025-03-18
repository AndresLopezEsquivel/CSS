# CSS selectors

CSS selectors are patterns used to select the element(s) you want to style.

## Element selector

Selects all elements with the specified element name. For example, the following CSS rule will apply to all `<p>` elements:

```css
p {
  color: red;
}
```

## Class selector

Selects all elements with the specified class attribute. For example, the following CSS rule will apply to all elements with the class `highlighted`:

```css
.highlighted {
  background-color: yellow;
}
```

```html
<p class="highlighted">This paragraph has a yellow background.</p>
```

## ID selector

Selects a single element with the specified ID attribute. For example, the following CSS rule will apply to the element with the ID `main-heading`:

```css
#main-heading {
  color: blue;
}
```

```html
<h1 id="main-heading">This heading is blue.</h1>
```

## Attribute selector

Selects elements with the specified attribute. For example, the following CSS rule will apply to all elements `<p>` with the attribute `draggable`:

```css
p[draggable] {
  border: 1px solid black;
}
```

```html
<p draggable="true">This paragraph can be dragged.</p>
```

We can also select elements with a specific attribute value. For example, the following CSS rule will apply to all elements `<p>` with the attribute `draggable` set to `true`:

```css
p[draggable="true"] {
  border: 1px solid black;
}
```

```html
<p draggable="true">This paragraph can be dragged.</p>
```

## Grouping selector

Selects all elements that match any of the selectors. For example, the following CSS rule will apply to all `<h1>` and `<h2>` elements:

```css
h1, h2 {
  color: green;
}
```

```html
<h1>This heading is green.</h1>
<h2>This heading is also green.</h2>
```

## Descendant selector

Selects an element that is a descendant of another element. For example, the following CSS rule will apply to all `<p>` elements that are descendants of a `<div>` element:

```css
div p {
  color: purple;
}
```

```html
<div>
  <p>This paragraph is purple.</p>
</div>
```

## Child selector

Selects an element that is a direct child of another element. For example, the following CSS rule will apply to all `<p>` elements that are direct children of a `<div>` element:

```css
div > p {
  color: orange;
}
```

```html
<div>
  <p>This paragraph is orange.</p>
</div>


<div>
  <span>
    <p>This paragraph is not orange.</p>
  </span>
</div>
```

## Adjacent sibling selector

Selects an element that is the adjacent sibling of another element. For example, the following CSS rule will apply to all `<p>` elements that are immediately preceded by an `<h1>` element:

```css
h1 + p {
  color: pink;
}
```

```html
<div>
  <h1>This heading is not pink.</h1>
  <p>This paragraph is pink.</p>
</div>

<div>
  <h1>This heading is not pink.</h1>
  <h2>This heading is not pink.</h2>
  <p>This paragraph is not pink.</p>
</div>
```
