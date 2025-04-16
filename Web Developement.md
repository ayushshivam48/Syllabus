# 📘 Module I: Introduction to HTML Programming and Overview of UX

## 🔹 Introduction to HTML5.0

### History of HTML

HTML was introduced by Tim Berners-Lee in 1991. HTML5, released in 2014, supports video, audio, and semantic elements for better web apps.

### Structure of HTML

<!DOCTYPE html>
<html>
  <head>
    <title>Sample Page</title>
  </head>
  <body>
    <h1>Welcome!</h1>
  </body>
</html>

### Adding Comments

<!-- This is a comment -->


### Formatting Text

<b>Bold</b>, <i>Italic</i>, <u>Underline</u>, <strong>Strong</strong>, <em>Emphasized</em>

### Creating List

<ul><li>Item 1</li></ul> | <ol><li>Step 1</li></ol>

### Creating Definition List

<dl>
  <dt>HTML</dt>
  <dd>Markup language for web</dd>
</dl>

### Creating Hyper Text Links

<a href="https://example.com">Go to Example</a>

### Creating Link Lists

<ul>
  <li><a href="page1.html">Page 1</a></li>
</ul>

### Inserting Inline Images

<img src="image.jpg" alt="My Image">

### Creating Image Links

<a href="https://example.com"><img src="logo.png" alt="Logo"></a>
### Horizontal Rules

<hr>

### Address Tag

<address>Contact: info@example.com</address>

### Changing font Sizes and Colors

<p style="color: red; font-size: 20px;">Styled Text</p>

### Using Background Image

<body style="background-image: url('bg.jpg');">

### Marquee Tag

<marquee>Scrolling text</marquee>

## 🔹 Overview of User Experience Design (UX)

Focuses on improving satisfaction, usability, and interaction of the user with the product.

Example: A clean and responsive layout improves UX.

## 🔹 Fundamentals of Design

Principles: Alignment, Contrast, Balance, Repetition, Proximity

Example: Using consistent buttons and layout increases clarity.

## 🔹 Overview of WordPress and WIX

WordPress: Open-source, flexible CMS

Wix: No-code, drag-and-drop builder

Example: WordPress is great for blogs and e-commerce; Wix is ideal for personal portfolios.


# 📘 Module II: Tables, iFrames, and Forms

## 🔹 Creating Tables

<table border="1">
  <tr><th>Name</th><th>Age</th></tr>
  <tr><td>Alice</td><td>25</td></tr>
</table>

### Adding Border: border="1"

### Column Headings: <th>

### Spacing and Padding: Use CSS → cellspacing, cellpadding (older HTML), or:

<style>
  td { padding: 10px; }
</style>

### Caption

<caption>Student Info</caption>

### Table Width and Height

<table width="500" height="200">

### Row Headings

<tr><th scope="row">Name</th><td>Alice</td></tr>

### Aligning Cell Contents

<td align="center">Centered</td>

### Setting Column Width

<td width="100">Fixed width</td>

### Centering a Table

<div style="text-align:center;">
  <table>...</table>
</div>

### Inserting an Image in a Table Cell

<td><img src="photo.jpg"></td>

### Spanning Columns and Rows

<td colspan="2">Spanning 2 columns</td>
<td rowspan="2">Spanning 2 rows</td>

### Background Colors

<td style="background-color: yellow;">Colored Cell</td>


## 🔹 Introduction to Forms

<form action="submit.php" method="post">
  <label>Name:</label>
  <input type="text" name="username">
  <input type="submit" value="Submit">
</form>

### Elements: input, textarea, select, checkbox, radio, submit



# 📘 Module III: CSS and CSS Frameworks

## 🔹 Cascading Style Sheets (CSS)

Used to style HTML elements (colors, layout, fonts).

## 🔹 Ways to use CSS

### Inline

<p style="color: red;">Red Text</p>

### Internal

<style>
  p { color: blue; }
</style>

### External

<link rel="stylesheet" href="style.css">

## 🔹 Selectors

p { color: green; }       /* element selector */
#main { font-size: 20px; } /* ID selector */
.box { border: 1px solid; } /* class selector */

## 🔹 DIV and SPAN Elements

<div> = block-level container

<span> = inline container

## 🔹 Using Classes and IDs

<div id="header">Welcome</div>
<p class="highlight">Important</p>

## 🔹 Pseudo-classes

a:hover { color: red; }   /* link hover effect */

## 🔹 CSS Framework Introduction

### Why use?

Faster, cleaner styling with prebuilt classes.

Examples: Bootstrap, Tailwind CSS

## 🔹 Types of CSS Frameworks

Front-end: Bootstrap, Foundation

Back-end: Laravel Mix, SASS-based tools



# 📘 Module IV: JavaScript

## 🔹 Introduction to JavaScript

JavaScript adds interactivity to web pages (e.g., button clicks, alerts).

## 🔹 Data Types & Variables

var name = "Alice";
let age = 25;
const pi = 3.14;

## 🔹 Dialog Boxes

alert("Hello!");
confirm("Are you sure?");
prompt("Enter your name:");

## 🔹 Event Handling

<button onclick="sayHello()">Click Me</button>
<script>
  function sayHello() {
    alert("Hello!");
  }
</script>

### Other Events:

onclick, ondblclick, onfocus, onblur

onmouseover, onmouseout, onmousemove

onkeyup, onkeypress, onchange, onload

## 🔹 Front-end Validations

if(document.forms["myForm"]["email"].value == "") {
  alert("Email is required");
  return false;
}

## 🔹 Overview of AJAX, jQuery, JSON

AJAX – Asynchronous page updates without refresh

jQuery – JS library for easier DOM manipulation

JSON – Data format for APIs and AJAX

{ "name": "Alice", "age": 25 }
