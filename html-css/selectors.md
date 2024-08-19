# Selectors

## \*

- Universal selector
- Selects every elements in the document

```CSS
* {
  margin: 0;
  padding: 0;
}
```

## Type (Tag) Selector

- Selects a specific HTML tag to apply styles

```CSS
h1 {
  color: blue;
}

p {
  font-size: 32px;
  font-weight: bold;
}
```

## ID Selector

```HTML
<p id="one">one</p>
```

```CSS
#one {
    color: blue;
}
```

- Value of the ID must be unique within the document
- Higher specificity than type selector
- Low reusability

## Class Selector

```HTML
<h1 class="fc-red">hello wolrd</h1>
<p>Lorem ipsum dolor sit amt</p>
<p class="fc-red">Lorem ipsum dolor sit amt</p>
```

```CSS
.fc-red {
  color: red;
}
```

- Same class value can be used more than once within the document
- Can define several class values in a tag
- High reusability
- Writing rules
  - Must not start with a number
  - Can start with hyphen, underscore, and characters

## Attribute Selector

```HTML
<button type="button" class="btn">button</button>
<button type="submit" class="btn">submit</button>
<button type="reset">reset</button>
```

```CSS
[type='button'] {
  border: 0;
  cursor: pointer;
}

[class^='btn'] {
  color: #fff;
  background: royalblue;
}
```

- \[type]
  - Selects elements that have 'type' attribute
- \[type="button"]
  - Selects elements with a 'type' attribute value of 'button'
- \[class^="btn"]
  - Selects elements with a 'class' value starting with 'btn'
- \[class$="btn"]
  - Selects elements with a 'class' value ending with 'btn'
- input:not([class*="btn"])
  - Selects elements with a 'class' value containing 'btn'
    - 'not' keyword selects elements that do not match the specified condition

## Group Selector

```HTML
<h1>hello</h1>
<h2>hello</h2>
<h3>hello</h3>
```

```CSS
h1,
h2,
h3 {
  color: blue;
}
```

- Apply the same style to multiple selectors at once by separating them with commas

## Descendent Selector

```HTML
<p>lorem ipsum dolor sit amet</p>
<p>lorem ipsum dolor sit amet</p>
<p>lorem ipsum dolor sit amet</p>
<section>
  <div>
    <p>lorem ipsum dolor sit amet</p>
  </div>
  <p>lorem ipsum dolor sit amet</p>
  <p>lorem ipsum dolor sit amet</p>
</section>
<p>lorem ipsum dolor sit amet</p>
<p>lorem ipsum dolor sit amet</p>
<p>lorem ipsum dolor sit amet</p>
```

```CSS
section p {
  font-weight: bold;
}
```

![Descendent Selector](https://www.books.weniv.co.kr/images/basecamp-html-css/chapter03/03-2.png)

- Selects all descendent elements of a specified element

## Child Selector

```HTML
<p>lorem ipsum dolor sit amet</p>
<p>lorem ipsum dolor sit amet</p>
<p>lorem ipsum dolor sit amet</p>
<section>
  <div>
    <p>lorem ipsum dolor sit amet</p>
  </div>
  <p>lorem ipsum dolor sit amet</p>
  <p>lorem ipsum dolor sit amet</p>
</section>
<p>lorem ipsum dolor sit amet</p>
<p>lorem ipsum dolor sit amet</p>
<p>lorem ipsum dolor sit amet</p>
```

```CSS
section > p {
  color: royalblue;
}
```

![Child Selector](https://www.books.weniv.co.kr/images/basecamp-html-css/chapter03/03-3.png)

- Selects only the direct child elements of a specified element

## General Sibling Selector

```HTML
<p>lorem ipsum dolor sit amet</p>
<p>lorem ipsum dolor sit amet</p>
<p>lorem ipsum dolor sit amet</p>
<section>
  <div>
    <p>lorem ipsum dolor sit amet</p>
  </div>
  <p>lorem ipsum dolor sit amet</p>
  <p>lorem ipsum dolor sit amet</p>
</section>
<p>lorem ipsum dolor sit amet</p>
<p>lorem ipsum dolor sit amet</p>
<p>lorem ipsum dolor sit amet</p>
```

```CSS
section ~ p {
  text-decoration: underline;
}
```

![General Sibling Selector](https://www.books.weniv.co.kr/images/basecamp-html-css/chapter03/03-4.png)

- Selects only the siblings that follow the specified element

## Adjacent Sibling Selector

```HTML
<p>lorem ipsum dolor sit amet</p>
<p>lorem ipsum dolor sit amet</p>
<p>lorem ipsum dolor sit amet</p>
<section>
  <div>
    <p>lorem ipsum dolor sit amet</p>
  </div>
  <p>lorem ipsum dolor sit amet</p>
  <p>lorem ipsum dolor sit amet</p>
</section>
<p>lorem ipsum dolor sit amet</p>
<p>lorem ipsum dolor sit amet</p>
<p>lorem ipsum dolor sit amet</p>
```

```CSS
section + p {
  background: yellow;
}
```

![Adjacent Sibling Selector](https://www.books.weniv.co.kr/images/basecamp-html-css/chapter03/03-5.png)

- Selects only the immediately adjacent sibling
