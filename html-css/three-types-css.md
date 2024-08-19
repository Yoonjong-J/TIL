# Three Types of CSS Styles

## Inline

```HTML
<p style="color:yellow; background-color:black;">Hello world</p>
```

- Not a recommended type
- Impair readability
- Use for only short and simple code

## Internal

```HTML
<!DOCTYPE html>
<html lang="ko-KR">
  <head>
    <meta charset="UTF-8" />
    <title>Internal</title>
    <style>
      p {
        color: yellow;
        background-color: black;
      }
    </style>
  </head>
  <body>
    <p>Hello world</p>
  </body>
</html>
```

## External

```HTML
<!-- index.html -->
<!DOCTYPE html>
<html lang="ko-KR">
  <head>
    <meta charset="UTF-8" />
    <title>외부 스타일</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <p>Hello world</p>
  </body>
</html>
```

```CSS
/* style.css */
p {
  color: yellow;
  background-color: black;
}
```

- Recommended type
- Enhance readability
