# prettier

A Highlight JS theme with support for Dark Mode. prettier is (hopefully) unique with it's different take on code blocks, as well as using more vibrant colours when highlighting code, and wide range of colours used.

## Installation

To use prettier, you need Highlight JS, and our CSS code. Place `<script src="https://cdn.jsdelivr.net/gh/highlightjs/cdn-release@11.9.0/build/highlight.min.js"></script>`, and `<script>hljs.highlightAll();</script>` at the end of your `<body>`, like so:

``` html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script src="https://cdn.jsdelivr.net/gh/highlightjs/cdn-release@11.9.0/build/highlight.min.js"></script>
    <script>hljs.highlightAll();</script>
</body>
</html>
```

Then, you need to reference the prettier CSS file by placing `<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/skrillx13/prettier/dist/prettier.min.css">` in your `<head>`.

``` html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/skrillx13/prettier/dist/prettier.min.css">
    <title>Document</title>
</head>
<body>
    <script src="https://cdn.jsdelivr.net/gh/highlightjs/cdn-release@11.9.0/build/highlight.min.js"></script>
    <script>hljs.highlightAll();</script>
</body>
</html>
```

### Adding the library

If are planning on making some customizations to the library, or need the dark mode colours, it is best to add the library yourself. Take the `prettier.css` file, `prettier.light.css`, or `prettier.dark.css` file from our `dist` folder, and toss it into your project.

Reference the Highlight JS JavaScript as usual, while pointing to your self-hosted prettier CSS file:

``` html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="path/to/prettier.css">
    <title>Document</title>
</head>
<body>
    <script src="https://cdn.jsdelivr.net/gh/highlightjs/cdn-release@11.9.0/build/highlight.min.js"></script>
    <script>hljs.highlightAll();</script>
</body>
</html>
```

## Usage

If you are using prettier with HTML, wrap your code within `<pre>`, and `<code>` tags. Reference the language by giving `<code>` a class. For example, highlighting CSS code would look something like this:

``` html
<body>
    <pre>
        <code class="language-css">
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900:ital@0;1&display=swap');

body {
    font-family: Poppins;
    background-color: #fffff8;
    padding-left: 10%;
    padding-right: 10%;
}
        </code>
    </pre>
</body>
```

if you are authoring in Markdown, it's even easier! 

``` css
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900:ital@0;1&display=swap');

body {
    font-family: Poppins;
    background-color: #fffff8;
    padding-left: 10%;
    padding-right: 10%;
}
```

## Dark Mode

Currently a WIP