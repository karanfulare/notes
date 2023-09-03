# HTML Form Tags

HTML forms allow users to input data interactively on a web page. This document provides a comprehensive overview of HTML form tags, their attributes, use cases, and examples.

## 1. `<form>`

**Description:**
The `<form>` element defines an interactive form that collects user input. It encapsulates form controls like text inputs, radio buttons, checkboxes, etc.

**Attributes:**

- `action`: Specifies the URL where the form data should be sent.
- `method`: Defines the HTTP method for sending form data (`GET` or `POST`).
- `target`: Specifies where the response should be displayed (`_blank`, `_self`, `_parent`, `_top`, or a custom frame name).
- `enctype`: Specifies the encoding type for form data (`application/x-www-form-urlencoded`, `multipart/form-data`, or `text/plain`).

**Example:**

```html
<form action="/submit" method="POST">
  <label for="username">Username:</label>
  <input type="text" id="username" name="username" required />
  <button type="submit">Submit</button>
</form>
```

## 2. `<input>`

- Description:
  The `<input>` element is used to create various form controls, such as text inputs, radio buttons, checkboxes, and more.

### Attributes (varies by type):

- type: Specifies the type of input control (text, password, radio, checkbox, etc.).
- name: Assigns a name to the input, which is used when submitting data.
- id: Provides a unique identifier for the input element.
- value: Sets the initial or default value.
- required: Makes the input field mandatory.
- placeholder: Displays a brief hint to the user.
- disabled: Disables the input control.
- maxlength: Limits the number of characters.
  ...and more depending on the type.

**Example:**

```html
<label for="username">Username:</label> <input type="text" id="username" name="username" required placeholder="Enter your username" />
```

## 3. `<label>`

Description:
The `<label>` element associates text with form controls, making them more accessible.

### Attributes

for: Links the label to the id of the associated input element.

**Example:**

```html
<label for="username">Username:</label> <input type="text" id="username" name="username" />
```

## 4. `<textarea>`

Description:
The `<textarea>` element allows users to input multiple lines of text.

### Attributes

name: Assigns a name to the textarea.
id: Provides a unique identifier.
rows and cols: Define the visible number of rows and columns.
**Example:**

```html
<label for="comments">Comments:</label> <textarea id="comments" name="comments" rows="4" cols="50"></textarea>
```

## 5. `<button>`

Description:
The `<button>` element represents a clickable button.

### Attributes

type: Specifies the type of button (submit, reset, or button).
name: Assigns a name to the button.
value: Sets the value to be submitted when clicked.

**Example:**

```html
<button type="submit" name="submitBtn" value="Submit">Submit</button>
```

## 6. `<select> and <option>`

Description:
The `<select>` element creates a dropdown list, while `<option>` defines individual options within the list.

### Attributes

`<select>`: name, id, size, multiple, and more.

`<option>`: value, selected, disabled, and more.

**Example:**

```html
<label for="colors">Select a color:</label>
<select id="colors" name="color">
  <option value="red">Red</option>
  <option value="green">Green</option>
  <option value="blue">Blue</option>
</select>
```

## 7. `<fieldset> and <legend>`

Description:
`<fieldset>` groups related form elements, and `<legend>` provides a title for the fieldset.

### Attributes

`<fieldset>`: name, id, disabled, form, and more.
`<legend>`: No specific attributes.

**Example:**

```html
<fieldset>
  <legend>Contact Information</legend>
  <!-- Form elements go here -->
</fieldset>
```

## 8. `<input type="radio"> and <input type="checkbox">`

Description:
These input types create radio buttons and checkboxes, respectively.

### Attributes

type, name, id, value, checked, disabled, and more.

**Example:**

```html
<input type="radio" id="male" name="gender" value="male" />
<label for="male">Male</label>

<input type="checkbox" id="subscribe" name="newsletter" value="subscribe" />
<label for="subscribe">Subscribe to Newsletter</label>
```
