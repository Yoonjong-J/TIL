# HTML Basics

## index.html

```HTML
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body></body>
</html>
```

### Why 'index.html'...?

We name an HTML file 'index.html' that will be used as the main page of a site because....

- Coding convention
  - One of the agreements that had been made by many developers letting collaboration process easier
- Web server's default setting
  - When client makes an HTTP request, web server search for 'index.html' file as a default

### < !DOCTYPE html >

- This tag means the HTML file is the HTML Living Standard one
- Lets the browser to accurately interpret and render the document according to the latest standards

### < html lang="eng" >

- html tag is the root of the document
- 'lang' attribute means 'language'

  | Language code | Language | Country Code                                                              |
  | ------------- | -------- | ------------------------------------------------------------------------- |
  | en            | English  | US(USA), GB(England), PH(Philippines)                                     |
  | ko            | Korean   | KR(South Korea)                                                           |
  | zh            | Chinese  | CN(China), HK(Hong Kong), TW(Taiwan), Hans(Simplified), Hant(Traditional) |
  | ja            | Japanese |                                                                           |
  | de            | German   |                                                                           |

### < head >

- Tag that stores metadata
  - data for search engines

### Metadata

- Information about the data
- Search engines read and interpret metadata
- charset (attribute)
  - Attribute insiede meta tag that specifies the character encoding for the HTML document
  - Character encoding determines how the characters in the document are represented as bytes, which is essential for displaying text correctly in a web browser
    - **UTF-8** is the most commonly used character encoding
- title (tag)
  - Title of a web page
  - Text we see on browser tab, search engine results, bookmarks, and social media
- link (tag)
  - Represents relationship with outer resource such as CSS file
    - ```HTML
      <link rel="stylesheet" href="style.css">
      ```
      - rel: relations
      - href: hyper-references

### < body >

- Represents main content of a web page

## Self-closing tag (a.k.a. void element)

Tag that does not need a closing tag

Non-self-closing tags:

```HTML
<p></p>
<h1></h1>
<div></div>
```

Self-closing tags:

```HTML
<br />
<img src="" alt="">
<input type="text" />
```
