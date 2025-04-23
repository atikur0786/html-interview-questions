# What is HTML and what does it stand for?

## Answer

HTML stands for **HyperText Markup Language**. It is the standard markup language used to create and structure content on the web. HTML describes the structure of web pages using markup.

HTML elements are represented by tags, which label pieces of content such as "heading", "paragraph", "table", etc.

## Key Points

- HTML is not a programming language; it's a markup language
- HTML documents are described by HTML tags
- HTML tags label pieces of content such as "heading", "paragraph", "table", etc.
- Browsers do not display the HTML tags, but use them to render the content of the page

## Code Example

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Basic HTML Document</title>
  </head>
  <body>
    <header>
      <h1>This is a Heading</h1>
    </header>

    <main>
      <p>This is a paragraph.</p>

      <section>
        <h2>This is a sub-heading</h2>
        <p>
          This is another paragraph with a
          <a href="https://example.com">link</a>.
        </p>
      </section>
    </main>

    <footer>
      <p>&copy; 2025 Example Company</p>
    </footer>
  </body>
</html>
```

## Additional Information

HTML was first created by Tim Berners-Lee in 1990. Since then, there have been many versions of HTML. The most recent version is HTML5, which introduced many new semantic elements and APIs.

## Related Questions

- [What are the new features in HTML5?](html5-features.md)
- [What is the difference between HTML elements and tags?](elements-vs-tags.md)
