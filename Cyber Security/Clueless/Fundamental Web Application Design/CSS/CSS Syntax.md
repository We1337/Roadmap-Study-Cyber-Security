CSS (Cascading Style Sheets) is a styling language used to add styles and layout to web pages. The basic syntax of CSS consists of selectors, properties, and values:

Selector: A selector is used to select the HTML element(s) that you want to style. It could be an element, class, ID or other attribute. Selectors are followed by a set of curly braces {} that contain the styles.

Example:

```css
h1 {
  color: blue;
}
```

This example selects all the `h1` elements and sets the color property to blue.

Property: A property is a specific styling attribute that you want to apply to the selected HTML element(s). CSS provides a wide range of properties such as font-size, color, background-color, margin, padding, etc.

Example:

```css
h1 {
  font-size: 24px;
}
```

This example sets the font-size property of all `h1` elements to 24 pixels.

Value: A value is a specific setting for the selected property. It could be a color, a size, a position, or any other valid CSS value.

Example:

```css
h1 {
  margin: 10px 20px;
}
```

This example sets the margin property of all `h1` elements to 10 pixels on top and bottom, and 20 pixels on the left and right.

CSS rules are usually written inside a `<style>` element in the head section of an HTML document or in an external CSS file that is linked to the HTML document.