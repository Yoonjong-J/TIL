# forms & table tags

## forms

- Used to receive data from the user and send it to the server
- Used in many cases that need interaction such log in, sign up, search, or survey

### form tag

```HTML
<form action="/login" method="POST"></form>
```

- Serves as a container for composing a form
- Can use several input elements inside
- action attribute
  - Specifies the URL of the server that will process the form data
- method attribute
  - Specifies the method for sending data to the server
  - Typically uses **GET** or **POST**

### input tag

```HTML
<input type="text" id="username" name="username" />
<input type="password" id="password" name="password" />
<input type="checkbox" id="remember" name="remember" />
<input type="radio" id="gender-male" name="gender" value="male" />
```

- The most basic element for receiving user input
- Supports various types of input, including text, password, checkboxes, and radio buttons
- type attribute
  - Specifies the type of the input field
- value attribute
  - Specifies the name of the field that will be used when the form data is sent
  - Server uses it to identify the data

### label tag

- Provides description for an input field
- Ensures that clicking the label focuses the associated input element
- for attribute
  - Specifies the ID of the input element that the \<label> describes
  - Value of the for attribute must match the ID attribute of the associated input element

```HTML
<label for="username">ID:</label>
<input type="text" id="username" name="username" />

<label for="password">PW:</label>
<input type="password" id="password" name="password" />
```

## table tag

- Used to structure and display information
- Organizes data into rows and columns, making various types of information easier to understand visually

```HTML
<table>
  <tr>
    <th>Product</th>
    <th>Price</th>
    <th>Quantity</th>
  </tr>
  <tr>
    <td>Laptop</td>
    <td>$1000</td>
    <td>10</td>
  </tr>
  <tr>
    <td>Smartphone</td>
    <td>$800</td>
    <td>20</td>
  </tr>
  <tr>
    <td>Tablet PC</td>
    <td>$600</td>
    <td>15</td>
  </tr>
</table>
```

![Table Tag](/TIL/Screenshots/table.png)
