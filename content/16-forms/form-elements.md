+++
date = "2017-01-22T18:04:24-05:00"
title = "Form Elements"
toc = true
next = "/16-forms/styling-forms"
prev = "/16-forms/form-overview"
weight = 11

+++

## Text Input

```html

<form action="http://www.example.com/login.php">
  <p>
    Username:
    <input type="text" name="username" maxlength="30" />
  </p>
</form>

```

---

## Text Input Example

![inline](/images/16/text_input.png)

---

## Text Input Attributes

- **type="text"**: Tells browser input will store plain text
- **name**: Used by the server to identify which form control that data came from
- **maxlength**: (optional) Specifies that max number of characters that can be entered

---

## Password Input

```html

<form action="http://www.example.com/login.php">
  <p>
    Username:
    <input type="text" name="username" size="15" maxlength="30" />
  </p>

  <p>
    Password:
    <input type="password" name="password" size="15" maxlength="30" />
  </p>
</form>

```

---

## Password Input Example

![inline](/images/16/password_input.png)

---

## Password Input Attributes

- **type="password"**: Tells browser input will store sensitive information, block characters from being displayed
- **name**: Used by the server to identify which form control that data came from
- **maxlength**: (optional) Specifies that max number of characters that can be entered

---

## Text Area

```html

<form action="http://www.example.com/comments.php">
  <p>What did you think of FEWD?</p>
  <textarea name="comments" cols="20" rows="4">Enter your comments...</textarea>
</form>

```

---

## Text Area Example

![inline](/images/16/text_area.png)

---

## Text Area Attributes

- **col**: Controls number of columns
- **rows**: Controls number of rows

**Do not use these, current best practice is to use css to control the width and height of ``<textarea>``**

---

## Radio Button

```html

<form action="http://www.example.com/profile.php">
  <p>Please select your favorite sport:
    <br />
    <input type="radio" name="sport" value="football" checked="checked" /> Football
    <input type="radio" name="sport" value="soccer" /> Soccer
    <input type="radio" name="sport" value="basketball" /> Basketball
  </p>
</form>

```

---

## Radio Button Example

![inline](/images/16/radio_button.png)

---

## Radio Button Attributes

- **type="radio"**: Allows users to pick just one of the number of options
- **name**: Identifies which form control that data came from (radio buttons in the same group share the same name attribute)
- **value**: Indicates the value that is sent to the server for the selected option
- **checked**: Used to indicate which value (if any) should be selected when the page loads

**Once a radio button is selected it cannot be deselected**

---

## Checkbox

```html

<form action="http://www.example.com/profile.php">
  <p>Please select your favorite music service(s):
    <br />
    <input type="checkbox" name="service" value="itunes" /> iTunes
    <input type="checkbox" name="service" value="lastfm" /> Last.fm
    <input type="checkbox" name="service" value="spotify" /> Spotify
  </p>
</form>

```

---

## Checkbox Example

![inline](/images/16/checkbox.png)

---

## Checkbox Attributes

- **type="checkbox"**: Allows users to pick one or more options
- **name**: Used by the server to identify which form control that data came from (checkboxes in the same group share the same name attribute)
- **value**: Indicates the value that is sent to the server for the selected option
- **checked**: Used to indicate which value (if any) should be selected when the page loads

---

## Select Box

```html
<form action="http://www.example.com/profile.php">
  <p>What device do you listen to music on?</p>
  <select name="devices">
    <option value="ipod">iPod</option>
    <option value="radio">Radio</option>
    <option value="computer">Computer</option>
  </select>
</form>

```

---

## Select Box Example

![inline](/images/16/select_dropdown.png)

---

## Select Box Attributes

- ``<select>``: Creates a drop down list box
  - **name**: Identifies which form control that data came from

- ``<option>``: Specifies the options that the user can select from
  - **value**: Indicates the value that is sent to the server for the selected option
  - **selected**: Indicates which option should be selected when the page loads

---

## Multiple Select Box

```html

<form action="http://www.example.com/profile.php">
  <select name="instruments" size="3" multiple="multiple">
    <option value="guitar" selected="selected">Guitar</option>
    <option value="drums">Drums</option>
    <option value="keyboard" selected="selected">Keyboard</option>
    <option value="bass">Bass</option>
  </select>
</form>

```

---

## Multiple Select Box Example

![inline](/images/16/multiple_select_box.png)

---

## Multiple Select Box Attributes

- **size**: Specifies how many options should be displayed
- **name**: Used by the server to identify which form control that data came from
- **multiple**: Allows users to select multiple options
 - PC Users: hold down ``control`` key to select multiple options
 - Mac Users: hold down ``command`` key to select multiple options

---

## Submit Button


```html

<form action="http://www.example.com/subscribe.php">
  <p>Subscribe to our email list:</p>
  <input type="text" name="email" />
  <input type="submit" name="subscribe" value="Subscribe" />
</form>

```

---

## Submit Button Example

![inline](/images/16/submit_button.png)

---

## Submit Button Attributes

- **type="submit"**: Submit button are used to submit a form to a server

- **name**: Used by the server to identify which form control that data came from

- **value**: Controls the text that appears on the button

The ``<button>`` element can also be used [more info](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/button)

---

## Labels

```html
  <form action="http://www.example.com/subscribe.php">
    <label>Age: <input type="text" name="age" /></label>
    <br/ >
    Gender:
    <input id="female" type="radio" name="gender" value="f">
    <label for="female">Female</label>
    <input id="male" type="radio" name="gender" value="m">
    <label for="male">Male</label>
  </form>
```


---

## Label Example

![inline](/images/16/labels.png)

---

## Label 

The `<label>` element can be used in two ways:

1) Wrap around both the text and form input

or

2) Kept separate from the form control and use the **for** attribute to indicate which form control it is a label for

---

## Label attributes

- **for** attribute states which form control the label belongs to

- value of the for attribute matches that of the id attribute on the form control it is labelling

- This technique using the for and id attributes can be used on any form control

- When a `<label>` element is used with a checkbox or radio button, users can click on either the form control or the label to select; the expanded clickable area makes the form easier to use


---

## Field Set

Used to group elements

```html
  <form action="http://www.example.com/subscribe.php">
    <fieldset>
      <legend>Contact details</legend>
      <label>Email:<br /><input type="text" name="email" /></label><br />
      <label>Mobile:<br /><input type="text" name="mobile" /></label><br />
      <label>Telephone:<br /><input type="text" name="telephone" /></label>
    </fieldset>
  </form>

```

---

## Field Set Example


![inline](/images/16/fieldset.png)

---

## Field Set Attributes

- `<fieldset>`: Use to group related elements together

- `<legend>`: Contains caption which ehlps identify the purpose of the group of form controls
