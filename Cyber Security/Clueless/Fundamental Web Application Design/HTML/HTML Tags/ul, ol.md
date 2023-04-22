`<ul>` and `<ol>` are HTML tags used to create ordered and unordered lists, respectively.

`<ul>` is used to create an unordered list. It has the following syntax:

```html
<ul>
  <li>List item 1</li>
  <li>List item 2</li>
  <li>List item 3</li>
</ul>
```

The `<ul>` tag defines the unordered list, and the `<li>` tags define each item in the list. The items are typically displayed with bullet points, but the exact appearance can vary depending on the web browser and CSS styling.

`<ol>` is used to create an ordered list. It has the following syntax:

```html
<ol>
  <li>List item 1</li>
  <li>List item 2</li>
  <li>List item 3</li>
</ol>
```

The `<ol>` tag defines the ordered list, and the `<li>` tags define each item in the list. The items are displayed with numbers or letters by default, but this can be customized with CSS styling.

Both `<ul>` and `<ol>` can be nested to create nested lists. For example:

```html
<ul>
  <li>List item 1</li>
  <li>List item 2
    <ul>
      <li>Nested list item 1</li>
      <li>Nested list item 2</li>
    </ul>
  </li>
  <li>List item 3</li>
</ul>
```

This code creates an unordered list with three items. The second item contains a nested unordered list with two items. When rendered in a web browser, this will display as a nested list with the second item indented and the nested items displayed with bullet points.