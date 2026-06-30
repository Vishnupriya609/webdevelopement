In CSS, the `display` property controls how an element is displayed on a web page.

### Common `display` Values

| Value          | Description                                                     |
| -------------- | --------------------------------------------------------------- |
| `block`        | Starts on a new line and takes full width available.            |
| `inline`       | Stays in the same line and only takes the width of its content. |
| `inline-block` | Like `inline`, but allows setting width and height.             |
| `none`         | Hides the element completely.                                   |
| `flex`         | Makes the element a flex container for flexible layouts.        |
| `grid`         | Makes the element a grid container.                             |

### Examples

#### `display: block`

```css
div {
  display: block;
}
```

#### `display: inline`

```css
span {
  display: inline;
}
```

#### `display: inline-block`

```css
button {
  display: inline-block;
  width: 150px;
}
```

#### `display: none`

```css
.hidden {
  display: none;
}
```



### Visual Difference

```html
<div style="display:block">Block 1</div>
<div style="display:block">Block 2</div>

<span style="display:inline">Inline 1</span>
<span style="display:inline">Inline 2</span>
```

**Output:**

* Block elements appear on separate lines.
* Inline elements appear on the same line.

## CSS `float`

The `float` property is used to **move an element to the left or right** of its container, allowing other content (like text) to wrap around it.

### Syntax

```css
float: left;
float: right;
float: none;
```

---

## 1. `float: left`

Moves the element to the **left**.

```html
<div class="box">Box</div>
<p>This text wraps around the box.</p>
```

```css
.box{
    float: left;
    width: 100px;
    height: 100px;
    background: lightblue;
}
```

**Output:**

```
[Box] This text wraps around the box.
```

---

## 2. `float: right`

Moves the element to the **right**.

```css
.box{
    float: right;
    width: 100px;
    height: 100px;
    background: pink;
}
```

**Output:**

```
This text wraps around the box.    [Box]
```

---

## 3. `float: none`

Default value. The element does **not** float.

```css
.box{
    float: none;
}
```

---

## Common Problem: Parent Height Collapses

When all child elements are floated, the parent may lose its height.

**Solution: Use `clear` or a clearfix.**

```css
.clear{
    clear: both;
}
```

Or with a clearfix:

```css
.parent::after{
    content: "";
    display: block;
    clear: both;
}
```

---

## Easy Example (Navigation)

```html
<ul>
    <li>Home</li>
    <li>About</li>
    <li>Contact</li>
</ul>
```

```css
li{
    float: left;
    list-style: none;
    margin-right: 20px;
}
```

**Output:**

```
Home   About   Contact
```

---

## Interview Answer (1 line)

> **The `float` property moves an element to the left or right of its container, allowing surrounding content to wrap around it.**

### Note

In modern CSS, **`flex`** and **`grid`** are preferred for creating layouts. `float` is mainly used today for wrapping text around images or maintaining older codebases.

## I made one project is [PetVerse](https://github.com/Vishnupriya609/webdevelopement/blob/main/Day%209/output.png) 
