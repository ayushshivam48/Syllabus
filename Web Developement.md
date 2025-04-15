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


