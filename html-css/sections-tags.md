# Sections Tags

- Semantically divide the HTML document
- Helps to express the structure and content of the document more clearly

```HTML
<body>
    <header>
        <nav></nav>
    </header>
    <main>
        <article></article>
        <aside></aside>
    </main>
    <footer></footer>
</body>
```

## nav tag

> nav: navigation

- Section that contains links to navigate to the current page or other pages
- Used for menus, tables of contents, breadcrumbs, and similar navigational elemenets

## footer tag

- Located at the bottom of a web page
- Contains information such as the page's author, copyright details, and related documents

## section tag

```HTML
<section>
    <h2></h2>
</section>
```

- Used to define specific section within a document
- Typically used to divide or distinguish topics and content
- Must contain at least one heading tag as a child tag

## article tag

- Represents a section that can be independently separated, distributed, or reused
- Performs an independent function without affecting other features of the site

## article vs section

- If confused, try using \<article> first
- Use \<article> for content that can be used independently, and use \<section> when the web page's context requires a connection or when there is no more suitable semantic element
- Use \<div> for only styling purpose

## aside tag

- Represents content that is indirectly related to the main content of the document
- Content inside this tag does not follow the main flow of the document and serves as a supplementary or ancillary space
- Can be used to display sidebars, advertisements, related links, illustrations, quotes, small web applications, and similar content on a web page
- Can provide related links by using \<nav> inside
