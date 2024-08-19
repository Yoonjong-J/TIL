# Contents Tags

## heading tag

```HTML
<h1></h1>
<h2></h2>
<h3></h3>
<h4></h4>
<h5></h5>
<h6></h6>
```

- Title of the page
- Importance decreases starting from h1
  - h1 is the most important one
  - h1 must be used only once per page

## anchor tag

```HTML
<a href="https://www.google.com/">Google</a>
```

- Creates a hyperlink that lets us move to other web page, file, or e-mail address through URL

### href

> href: hypertext reference

- Attribute that specifies the URL or path to which the link points

```HTML
<a href="https://www.google.com/">Google</a>
<a href="mail:xxxx@gmail.com">xxxx@gmail.com</a>
<a href="tel:000)000-0000">000)000-0000</a>
```

### target

- Attribute that specifies where the linked document will be opened
  - \_self: open in the current page
  - \_blank: open in the new page

```HTML
<a href="https://www.google.com/" target="_self">Google</a>
<a href="https://www.google.com/" target="_blank">Google</a>
```

### download

```HTML
<a href="index.html" download>Download</a>
```

- Attribute that makes the linked document to be downloaded when clicked

## paragraph tag

```HTML
<p>Hello World</p>
```

- Defines a block of text as paragraph
- Caanot use another \<p> tag inside a \<p> tag

## strong tag

```HTML
<p>
    Hello World <strong>Hello World</strong> Hello World
</p>
```

- Used to highlight the importance of the text
  - Semantically emphasizes the importance
- bold tag
  - ```HTML
    <p>
        Hello World <b>Hello World</b> Hello World
    </p>
    ```
  - Used for only visual effect
    - Has no semantical meaning

## br & hr tags

- \<br>
  - br: break (line break)
  - Used to change the line witin the paragraph
- \<hr>
  - hr: horizontal rule
  - Used to change the line and draw a horizontal line within the paragraph

```HTML
<p>
    Lorem ipsum dolor, sit amet consectetur adipisicing elit. <br /> Possimus
    perferendis libero illum id? <hr /> Nemo repudiandae quos sunt ea fugiat suscipit
    voluptas, omnis accusamus voluptatem, tempore dolor inventore sit
    voluptates corporis.
</p>
```

## pre tag

```HTML
<pre>
    Hello World
    Hello World
    Hello World
    Hello World
    Hello World
</pre>
```

- Defines performatted text
- Unlike paragraph tag, pre tag preserves both spaces and line breaks, displaying text exactly as it is written in the HTML document
