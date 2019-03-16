+++
date = "2017-01-22T18:04:24-05:00"
title = "EMS / REMS"
toc = true
next = "/14-responsive-design/responsive-images"
prev = "/14-responsive-design/code-along"
weight = 19

+++


## What are EMs?

- Scalable unit that is used in web document media

- Font-size is computed relative to font-size of parent element

- Does not lock users into an absolute font-size (older browsers do not re-size text set in pixels when users zoom)

- Provides users with highlest level of control over the content they are viewing


{{% notice tip %}}
History: Old-fashioned metal typesetting, the em referred to the size of the metal plates that contained a raised letter, which had to be wide enough to fit the widest letter, the capital M.  Many people assume that digital ems are also based on the width of the letter M, but they aren’t.
{{% /notice %}}


---


## EMs in practice

 ``` 

 html {
   // set base font-size for entire site
   font-size: 16px;
 }

 h1 {
   // translates to "make h1 element 1.4x larger than base font size (16px)"
   // resulting in a font size of 22.4px
   font-size: 1.4em;
 }

 h2 {
   // translates to "make h1 element 1.3x larger than base font size (16px)"
   // resulting in a font size of 20.8px
   font-size: 1.3em;
 }

 ```

---

## How is REM different?

- Instead of sizing fonts relative to their parent containers, REM sizes fonts relative to the root view (<html>)


<a class="jsbin-embed" href="https://jsbin.com/jejubot/embed?css,output">JS Bin on jsbin.com</a><script src="https://static.jsbin.com/js/embed.min.js?3.41.5"></script>

{{% notice tip %}}
You don't need to set the base font-size on the `<html>` element because it inherits font-size from the `<body>` tag by default. Therefore, most developers set the base font-size on the `<body>` tag
{{% /notice %}}

---

## Why are we using EMs?

- Main reason is to effectively scale our text up and down depending on the screen size

- Click [here for a great example of responsively styled text](http://alistapart.com/d/responsive-web-design/ex/ex-article.html) (resize your browser window to see the effect)


---

## What about Percentages for Text Sizing?

- Percentages are a relative unit of measurement similar to EMs

- Default font-size in percentages is 100%

- Can also be used instead of EMs (many options available)

- Some developers find that they [behave more consistently](http://kyleschaeffer.com/development/css-font-size-em-vs-px-vs-pt-vs/) than ems/rems

---

## How should we set up font size?

- The author from this [blog](http://engageinteractive.co.uk/blog/em-vs-rem-vs-px) avocates a certain approach to using ems to improve a site's accessibility:


```

body {
	/* set the base font to 62.5% to address any potential zoom issues */
	/* 62.5% translates to a default font-size of 10px */
	/* makes math easier so now 1.6em === 16px */
	font-size: 62.5%;
}


.content {
	// use ems or rems for all other font-sizes
	font-size: 1.2em;
}

```
