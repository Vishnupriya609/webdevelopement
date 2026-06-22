# Introduction to CSS

## What is a Style Sheet?

A **Style Sheet** is a set of rules that describes how a document should be displayed, including its colors, fonts, spacing, layout, and overall appearance.

Style sheets separate the **content** of a document from its **presentation**.

---

## Different Types of Style Sheets

### 1. CSS (Cascading Style Sheets)

The standard style sheet language used to style HTML web pages.

```css id="fwd6cq"
h1 {
    color: blue;
}
```

### 2. Sass (Syntactically Awesome Style Sheets)

A CSS preprocessor that extends CSS with features like variables, nesting, and mixins.

```scss id="vgn3nb"
$primary-color: blue;

h1 {
    color: $primary-color;
}
```

### 3. Less (Leaner Style Sheets)

A CSS preprocessor similar to Sass that adds programming-like features to CSS.

```less id="tdwz43"
@primary-color: blue;

h1 {
    color: @primary-color;
}
```

## Why CSS?

CSS is used to:

Add colors 🎨
Change fonts 🔤
Adjust spacing 📏
Create layouts 🏗️
Make websites responsive 📱

# Three Ways of Adding CSS

## 1. Inline CSS

CSS is added directly inside an HTML element using the `style` attribute.

```html id="5d9h2d"
<h1 style="color:red;">Hello World</h1>
```

**Use:** Styling a single element.

---

## 2. Internal CSS

CSS is written inside the `<style>` tag in the `<head>` section of the HTML document.

```html id="rr4w44"
<head>
    <style>
        h1 {
            color: blue;
        }
    </style>
</head>
```

**Use:** Styling a single webpage.

---

## 3. External CSS

CSS is written in a separate `.css` file and linked to the HTML document.

**HTML**

```html id="ggsnr0"
<link rel="stylesheet" href="style.css">
```

**style.css**

```css id="iijm4v"
h1 {
    color: green;
}
```

**Use:** Styling multiple webpages.

---

## Quick Comparison

| Method       | Location                                |
| ------------ | --------------------------------------- |
| Inline CSS   | Inside HTML element (`style` attribute) |
| Internal CSS | Inside `<style>` tag                    |
| External CSS | Separate `.css` file                    |

To link a CSS file to an HTML file, use the <link> tag inside the <head> section.

# CSS Selectors

**CSS Selectors** are used to select HTML elements and apply styles to them.

## 1. Element Selector

Selects all elements of a specific type.

```css
h1 {
    color: blue;
}
```

---

## 2. ID Selector (`#`)

Selects an element with a specific `id`.

```html
<h1 id="title">Hello</h1>
```

```css
#title {
    color: red;
}
```

---

## 3. Class Selector (`.`)

Selects elements with a specific class.

```html
<h1 class="heading">Hello</h1>
```

```css
.heading {
    color: green;
}
```

---

## 4. Universal Selector (`*`)

Selects all elements.

```css
* {
    margin: 0;
    padding: 0;
}
```

---

## 5. Attribute Selector (`[ ]`)

Selects elements based on their attributes.

```html
<input type="text">
<input type="password">
```

```css
input[type="text"] {
    border: 2px solid blue;
}
```

Only the text input will receive the style.

---

## Quick Summary

| Selector           | Symbol | Example              |
| ------------------ | ------ | -------------------- |
| Element Selector   | none   | `h1`                 |
| ID Selector        | `#`    | `#title`             |
| Class Selector     | `.`    | `.heading`           |
| Universal Selector | `*`    | `*`                  |
| Attribute Selector | `[ ]`  | `input[type="text"]` |


### Include all topics I made project is [color Vocab website](https://github.com/Vishnupriya609/webdevelopement/blob/main/Day%206/Output.png)

