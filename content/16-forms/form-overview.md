+++
date = "2017-01-22T18:04:24-05:00"
title = "Form Overview"
toc = true
next = "/16-forms/form-elements"
prev = "/16-forms/agenda"
weight = 10

+++

## What are forms?

- Forms allow us to get data from users

![inline](/images/16/ga_example_form.png)


---

## How do forms work?

![inline](/images/16/how_forms_work.png)

---

## Form Structure


```html
<form action="http://www.example.com/subscribe.php" method="get">
  <p>This is where the form controls will appear.</p>
</form>

```

---

## Form Attributes

- **action**: Required, the url on the server that will receive the information from the form

- **method**: Either a **get** or **post**
  * Use **get** when the data being sent to server is not senstive information and is relatively small (search form)
  * Use **post** when sending senstive data and when sending large amounts of data (registration form)
