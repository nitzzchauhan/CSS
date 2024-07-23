<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Module 4</title>
    <style>
        body {
            background-color: black;
            color: white;
        }
        h1, h2, h3, h4, h5, h6 {
            color: white;
        }
    </style>
</head>
<body>

Here is a comprehensive set of examples demonstrating the use of all CSS selectors mentioned:

### CSS Code for All Selectors

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Selectors Example</title>
    <style>
        /* Universal Selector */
        * {
            margin: 0;
            padding: 0;
        }

        /* Type Selector */
        p {
            color: blue;
        }

        /* Class Selector */
        .intro {
            font-size: 20px;
        }

        /* Multiple Classes Selector */
        .name1.name2 {
            color: red;
        }

        /* Descendant Selector */
        .name1 .name2 {
            font-weight: bold;
        }

        /* ID Selector */
        #firstname {
            background-color: lightblue;
        }

        /* Class with Type Selector */
        p.intro {
            color: green;
        }

        /* Grouping Selector */
        div, p {
            margin: 10px;
        }

        /* Descendant Selector */
        div p {
            color: red;
        }

        /* Child Selector */
        div > p {
            color: purple;
        }

        /* Adjacent Sibling Selector */
        div + p {
            color: orange;
        }

        /* General Sibling Selector */
        p ~ ul {
            color: pink;
        }

        /* Attribute Selector */
        [target] {
            border: 1px solid black;
        }

        /* Attribute Value Selector */
        [target="_blank"] {
            color: green;
        }

        /* Attribute Value with Word Selector */
        [title~="flower"] {
            color: violet;
        }

        /* Attribute Value Starting with Selector */
        [lang|="en"] {
            color: brown;
        }

        /* Attribute Value Beginning with Selector */
        a[href^="https"] {
            color: navy;
        }

        /* Attribute Value Ending with Selector */
        a[href$=".pdf"] {
            color: maroon;
        }

        /* Attribute Value Containing Selector */
        a[href*="example"] {
            color: teal;
        }

        /* Pseudo-Class Selectors */
        a:active {
            color: red;
        }

        p::after {
            content: " (after)";
        }

        p::before {
            content: " (before)";
        }

        input:checked {
            background-color: yellow;
        }

        input:default {
            border: 2px solid orange;
        }

        input:disabled {
            background-color: gray;
        }

        p:empty {
            border: 1px dashed red;
        }

        input:enabled {
            background-color: lightgreen;
        }

        p:first-child {
            font-weight: bold;
        }

        p::first-letter {
            font-size: 2em;
        }

        p::first-line {
            text-transform: uppercase;
        }

        p:first-of-type {
            color: blue;
        }

        input:focus {
            outline: 2px solid blue;
        }

        :fullscreen {
            background-color: yellow;
        }

        h2:has(+p) {
            color: red;
        }

        a:hover {
            color: purple;
        }

        input:in-range {
            background-color: lightyellow;
        }

        input:indeterminate {
            background-color: orange;
        }

        input:invalid {
            border-color: red;
        }

        p:lang(it) {
            font-style: italic;
        }

        p:last-child {
            font-style: italic;
        }

        p:last-of-type {
            color: darkblue;
        }

        a:link {
            text-decoration: underline;
        }

        ::marker {
            color: red;
        }

        :not(p) {
            color: gray;
        }

        p:nth-child(2) {
            color: lime;
        }

        p:nth-last-child(2) {
            color: cyan;
        }

        p:nth-last-of-type(2) {
            color: magenta;
        }

        p:nth-of-type(2) {
            color: gold;
        }

        p:only-of-type {
            font-weight: bold;
        }

        p:only-child {
            font-size: 1.5em;
        }

        input:optional {
            border: 2px dashed blue;
        }

        input:out-of-range {
            background-color: pink;
        }

        input::placeholder {
            color: gray;
        }

        input:read-only {
            background-color: lightgray;
        }

        input:read-write {
            border: 2px solid black;
        }

        input:required {
            border: 2px solid red;
        }

        :root {
            --main-color: coral;
        }

        ::selection {
            background: yellow;
        }

        #news:target {
            background-color: lightblue;
        }

        input:valid {
            border-color: green;
        }

        a:visited {
            color: darkmagenta;
        }
    </style>
</head>
<body>

    <p>This is a paragraph.</p>
    <p class="intro">This is an introductory paragraph.</p>
    <p id="firstname">This paragraph has an ID.</p>
    <div class="name1">
        <p class="name2">This is a nested paragraph with two classes.</p>
        <p class="name2">Another nested paragraph.</p>
    </div>
    <div>
        <p>This is a child paragraph.</p>
        <p>This is an adjacent sibling paragraph.</p>
    </div>
    <p>This is another paragraph.</p>
    <ul title="flower">
        <li>List item</li>
    </ul>
    <a href="https://example.com" target="_blank" title="example">Example Link</a>
    <a href="https://example.com/doc.pdf">PDF Link</a>
    <a href="https://example.com">Another Example Link</a>
    <input type="checkbox" checked>
    <input type="text" disabled>
    <input type="radio" disabled>
    <input type="radio" checked>
    <input type="text" required>
    <input type="text" placeholder="Enter text">
    <input type="range" min="0" max="100" value="50">
    <input type="text" value="Invalid" pattern="[a-zA-Z]+">
    <h2>Heading</h2>
    <p>This paragraph follows a heading.</p>
    <p>This is an indeterminate paragraph.</p>
    <p lang="it">Questo è un paragrafo in italiano.</p>
    <div>
        <p>This is the first child paragraph.</p>
        <p>This is the last child paragraph.</p>
    </div>
    <p>This is the only paragraph of its parent.</p>
    <p>This is the second child paragraph.</p>
    <p>This is the second last child paragraph.</p>
    <p>This is the nth child paragraph.</p>
    <input type="text" value="Valid" pattern="[a-zA-Z]+">
    <p class="intro">Another introductory paragraph.</p>
    <input type="text" readonly>
    <p>This is a paragraph that is not selected by :not(p).</p>
    <div>
        <a href="#news">Go to news section</a>
        <p id="news">This is the news section.</p>
    </div>
    <ul>
        <li>List item 1</li>
        <li>List item 2</li>
        <li>List item 3</li>
    </ul>
</body>
</html>
```

This HTML and CSS code demonstrates the usage of various CSS selectors, applying different styles to elements based on their types, classes, IDs, attributes, states, and more. You can add or modify elements and attributes as needed to further explore the capabilities of CSS selectors.