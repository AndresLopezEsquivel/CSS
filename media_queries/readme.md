# Media Queries
Media Queries are used to apply styles based on the viewport size or device characteristics. They allow you to create responsive designs that adapt to different screen sizes and orientations.

## max-width
The max-width media query applies styles when the viewport width is less than or equal to a specified value.
```css
@media (max-width: 600px) {
  div {
    width: 100%;
    background-color: lightblue;
  }
}
```
This media query will apply styles to devices with a maximum width of 600px.
The styles inside the media query will override the default styles for devices that match the condition.

## min-width
The min-width media query applies styles when the viewport width is greater than or equal to a specified value.
```css
@media (min-width: 600px) {
  div {
    width: 50%;
    background-color: lightgreen;
  }
}
```
This media query will apply styles to devices with a minimum width of 600px.
The styles inside the media query will override the default styles for devices that match the condition.

## combined

```css
@media (min-width: 600px) and (max-width: 1200px) {
  div {
    width: 75%;
    background-color: lightcoral;
  }
}
```
This media query will apply styles to devices with a width between 600px and 1200px.
The styles inside the media query will override the default styles for devices that match the condition.

```css
@media (max-width: 600px) and (min-width: 1200px) {
  div {
    width: 25%;
    background-color: lightyellow;
  }
}
```
This media query will apply styles to devices with a width less than 600px and greater than 1200px.
