# Selector Specificity

## How to Calculate

1. inline style: 1000 points
2. ID selector: 100 points
3. class selector, pseudo-class selector, attribute selector: 10 points
4. type selector, pseudo-element selector: 1 point
5. universal selector: 0 point

---

```CSS
p {
  color: blue;
}

p {
  color: red;
}
```

- Red color will be applied to \<p> tag

---

```HTML
<p class="important">Hello, World!</p>
```

```CSS
p { color: blue; }
.important { color: red !important; }
```

- Color red will be applied to \<p> tag
