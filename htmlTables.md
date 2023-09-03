# HTML Tables Guide

## Introduction

HTML tables are a fundamental part of web development used to display data in rows and columns. They provide a structured way to organize and present information on web pages.

## Table Structure

HTML tables are composed of several key elements:

- `<table>`: This is the container element for the entire table.
- `<tr>`: Represents a table row. It contains table data cells (`<td>`) or table header cells (`<th>`).
- `<th>`: Table header cell. Typically used for column headers.
- `<td>`: Table data cell. Used to display data.
- `<caption>`: An optional element that provides a title or description for the table.

## Basic Table Example

Here's a simple example of an HTML table:

```html
<table>
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
  </tr>
  <tr>
    <td>Data 1</td>
    <td>Data 2</td>
  </tr>
</table>
```

## Table Attributes

HTML tables can have various attributes to control their appearance and behavior:

1. **colspan** and **rowspan**: These attributes allow a cell to span multiple columns or rows.

- rowspan

```html
<table border="1">
  <tr>
    <td rowspan="2">This cell spans 2 rows</td>
    <td>Row 1, Cell 2</td>
  </tr>
  <tr>
    <td>Row 2, Cell 2</td>
  </tr>
  <tr>
    <td>Row 3, Cell 1</td>
    <td>Row 3, Cell 2</td>
  </tr>
</table>
```

- colspan

```html
<table border="1">
  <tr>
    <td>This cell spans 1 column</td>
    <td colspan="2">This cell spans 2 columns</td>
  </tr>
  <tr>
    <td>Row 2, Cell 1</td>
    <td>Row 2, Cell 2</td>
    <td>Row 2, Cell 3</td>
  </tr>
</table>
```

```html
<table>
  <tr>
    <td colspan="2">Cell spans 2 columns</td>
    <td>Cell 1</td>
  </tr>
  <tr>
    <td rowspan="2">Cell spans 2 rows</td>
    <td>Cell 2</td>
    <td>Cell 3</td>
  </tr>
  <tr>
    <td>Cell 4</td>
    <td>Cell 5</td>
  </tr>
</table>
```

2. **border**: This attribute is used to define the width of the table border (though it's considered outdated; CSS is preferred).

```html
<table border="1">
  <tr>
    <td>Row 1, Cell 1</td>
    <td>Row 1, Cell 2</td>
  </tr>
  <tr>
    <td>Row 2, Cell 1</td>
    <td>Row 2, Cell 2</td>
  </tr>
</table>
```

3. **width** and **height**: Sets the width and height of the table.

```html
<table width="400" height="200">
  <tr>
    <td>Row 1, Cell 1</td>
    <td>Row 1, Cell 2</td>
  </tr>
  <tr>
    <td>Row 2, Cell 1</td>
    <td>Row 2, Cell 2</td>
  </tr>
</table>
```

4. **align** and **valign**: Aligns the content horizontally and vertically.

```html
<table align="center">
  <tr>
    <td align="center">Centered Content</td>
  </tr>
</table>
```

```html
<tr>
  <td valign="bottom">Data 1</td>
  <td>Data 2</td>
</tr>
```

5. **bgcolor**: Specifies the background color of table cells (deprecated; use CSS instead).

```html
<table bgcolor="#FFD700">
  <tr>
    <td>Row 1, Cell 1</td>
    <td>Row 1, Cell 2</td>
  </tr>
  <tr>
    <td bgcolor="#00FF00">Row 2, Cell 1</td>
    <td bgcolor="#FF0000">Row 2, Cell 2</td>
  </tr>
</table>
```

6. **Summary** : The summary attribute provides a summary or description of the table's content for accessibility.

```html
<table summary="This table displays monthly sales data for 2023.">
  <tr>
    <td>Month</td>
    <td>Sales</td>
  </tr>
  <!-- Table content here -->
</table>
```

7. **cellpadding and cellspacing** : cellpadding adds space within each cell, and cellspacing adds space between cells.

```html
<table cellpadding="10" cellspacing="5">
  <tr>
    <td>Row 1, Cell 1</td>
    <td>Row 1, Cell 2</td>
  </tr>
  <tr>
    <td>Row 2, Cell 1</td>
    <td>Row 2, Cell 2</td>
  </tr>
</table>
```

## Nested Tables

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Nested Table Example</title>
  </head>
  <body>
    <table border="1">
      <tr>
        <th>Header 1</th>
        <th>Header 2</th>
        <th>Header 3</th>
      </tr>
      <tr>
        <td>Row 1, Cell 1</td>
        <td>Row 1, Cell 2</td>
        <td>Row 1, Cell 3</td>
      </tr>
      <tr>
        <td colspan="3">
          <table border="1">
            <tr>
              <th>Nested Header 1</th>
              <th>Nested Header 2</th>
            </tr>
            <tr>
              <td>Nested Row 1, Cell 1</td>
              <td>Nested Row 1, Cell 2</td>
            </tr>
            <tr>
              <td>Nested Row 2, Cell 1</td>
              <td>Nested Row 2, Cell 2</td>
            </tr>
          </table>
        </td>
      </tr>
      <tr>
        <td>Row 3, Cell 1</td>
        <td>Row 3, Cell 2</td>
        <td>Row 3, Cell 3</td>
      </tr>
    </table>
  </body>
</html>
```

## table caption

```html
<table>
  <caption>
    Employee Information
  </caption>
  <!-- Table content -->
</table>
```

## table headers

Use <thead>, <tbody>, and <tfoot> to group table rows for better structure.

```html
<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Age</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>John</td>
      <td>30</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td colspan="2">Footer Text</td>
    </tr>
  </tfoot>
</table>
```

```

```
