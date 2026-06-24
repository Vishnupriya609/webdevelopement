# CSS  - Specificity & inheritance

Talking about the **CSS Cascade** — the factors used to determine which CSS rule wins.

The 4 broad categories are:

## 1. CSS Position (Source Order)

Where the rule appears in the stylesheet.

Example:

```css
h1 {
    color: blue;
}

h1 {
    color: red;
}
```

Output:

```text
Red
```

Because the second rule comes later.

---

## 2. CSS Specificity

How specific the selector is.

Priority:

```text
Inline
   ↓
ID (#)
   ↓
Class (.)
   ↓
Element (h1)
```

Example:

```css
h1 {
 color: blue;
}

.title {
 color: red;
}
```

`.title` wins.

---

## 3. CSS Type (Origin)

Where the CSS comes from.

Priority:

```text
Browser CSS
    ↓
User CSS
    ↓
Author CSS (your CSS)
```

Your CSS usually overrides browser default styles.

---

## 4. Importance

Using `!important`.

Example:

```css
h1 {
 color: red !important;
}
```

`!important` overrides normal rules.

---

Final order:

```text
1. Importance (!important)
2. Type (origin)
3. Specificity
4. Position (source order)
```

These four decide the final CSS rule applied. ✅

# Combining CSS Selectors

CSS selectors can be combined to target elements more precisely.

---

## 1. Group Selector (`,`)

Applies the same styles to multiple elements.

### Syntax

```css
h1, h2, p {
    color: blue;
}
```

### Example

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<p>Paragraph</p>
```

All elements will have blue text.

---

## 2. Descendant Selector (space)

Selects elements that are inside another element.

### Syntax

```css
div p {
    color: red;
}
```

### Example

```html
<div>
    <p>Selected</p>
</div>

<p>Not Selected</p>
```

Only the `<p>` inside the `<div>` is selected.

---

## 3. Child Selector (`>`)

Selects only direct children of a parent element.

### Syntax

```css
div > p {
    color: green;
}
```

### Example

```html
<div>
    <p>Selected</p>

    <section>
        <p>Not Selected</p>
    </section>
</div>
```

Only the direct child `<p>` is selected.

---

## 4. Chaining Selector (No Space)

Targets a single element that matches multiple selectors at the same time.

### Syntax

```css
p.note {
    color: orange;
}
```

### Example

```html
<p class="note">Selected</p>

<div class="note">
    Not Selected
</div>
```

Only the `<p>` with class `note` is selected.

### Multiple Classes

```css
.btn.primary {
    background-color: blue;
}
```

```html
<button class="btn primary">
    Submit
</button>
```

The element must contain both classes.

---

If you want a **single example that combines Descendant and Chaining together**, use:

```css
.menu .item.active {
    color: red;
}
```

### HTML

```html
<div class="menu">
    <p class="item active">Home</p>
    <p class="item">About</p>
</div>
```

### How it works

```text
.menu .item.active
   ↓        ↓
Descendant  Chaining
```

* `.menu` → parent element
* Space (` `) → descendant combinator
* `.item.active` → same element must have both `item` and `active` classes

### Selected

```html
<p class="item active">Home</p>
```

✅ Inside `.menu` and has both classes.




# Quick Summary

| Selector            | Symbol    | Meaning                                |
| ------------------- | --------- | -------------------------------------- |
| Group Selector      | `,`       | Select multiple elements               |
| Descendant Selector | `(space)` | Select elements inside another element |
| Child Selector      | `>`       | Select direct children only            |
| Chaining Selector   | No space  | Same element must match all selectors  |

### Example Comparison

```css
.menu.active
```

* Same element has both classes.

```html
<div class="menu active"></div>
```

---

```css
.menu .active
```

* `.active` is inside `.menu`.

```html
<div class="menu">
    <span class="active"></span>
</div>
```

**Remember:**

```text
.menu.active  → Same element (Chaining)

.menu .active → Descendant element
```

# CSS Positioning

The `position` property determines how an element is positioned on a webpage.

## Types of Positioning

<img width="1200" height="398" alt="image" src="https://github.com/user-attachments/assets/fc96bde7-c6df-41a2-a926-057c0e5d512d" />


### 1. Static (Default)

```css
.box {
    position: static;
}
```

* Default position
* Follows normal document flow
  

* `top`, `right`, `bottom`, `left` do not work

---

### 2. Relative

```css
.box {
    position: relative;
    top: 20px;
    left: 30px;
}
```

* Moves relative to its original position
* Original space is preserved

---

### 3. Absolute

```css
.parent {
    position: relative;
}

.child {
    position: absolute;
    top: 0;
    right: 0;
}
```

* Removed from normal flow
* Positioned relative to the nearest positioned ancestor (`relative`, `absolute`, `fixed`, or `sticky`)
* If no positioned parent exists, it uses the page (`body`)

---

### 4. Fixed

```css
.box {
    position: fixed;
    bottom: 20px;
    right: 20px;
}
```

* Removed from normal flow
* Positioned relative to the browser viewport
* Stays in the same place while scrolling

---


# Quick Summary

| Position | Normal Flow           | Reference Point           |
| -------- | --------------------- | ------------------------- |
| static   | Yes                   | Default flow              |
| relative | Yes                   | Original position         |
| absolute | No                    | Nearest positioned parent |
| fixed    | No                    | Viewport (screen)         |


## Easy Memory Trick

```text
Static   → Normal
Relative → Move from original place
Absolute → Move relative to parent
Fixed    → Fixed to screen
Sticky   → Sticks while scrolling
```

### Most Common Combination

```css
.parent {
    position: relative;
}

.child {
    position: absolute;
    top: 0;
    right: 0;
}
```

Use `relative` on the parent and `absolute` on the child to place elements precisely inside containers. ✅
