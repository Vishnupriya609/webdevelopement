# CSS Properties

## CSS Colors

### CSS Color Types

1. **Named Colors** – Uses predefined color names like `red`, `blue`, and `green`.
```
  color: red;                  /* Named Color */
```

2. **HEX Colors** – Uses hexadecimal values (`#RRGGBB`) to represent colors.
```
   color: #FF0000;              /* HEX */
```

3. **RGB Colors** – Defines colors using Red, Green, and Blue values ranging from 0 to 255.
```
   color: rgb(255, 0, 0);       /* RGB */
```

4. **RGBA Colors** – Similar to RGB but includes an Alpha value for transparency.
```
   color: rgba(255, 0, 0, 0.5); /* RGBA */
```

5. **HSL Colors** – Defines colors using Hue, Saturation, and Lightness values.


    ```
    color: hsl(0, 100%, 50%);    /* HSL */
    ```

6. **HSLA Colors** – Similar to HSL but includes an Alpha value for transparency.
```
color: hsla(0, 100%, 50%, 0.5); /* HSLA */
```

### CSS Size Units

#### 1. `px` (Pixels)

A  unit used to set an 1/96th inch.

```css
font-size: 16px;
```

#### 2. `pt` (Points)

A unit mainly used for printing documents. 1pt = 1/72 of an inch.

```css
font-size: 12pt;
```

#### 3. `em`

A relative unit based on the font size of the parent element.

```css
font-size: 1.5em;
```

#### 4. `rem` (Root Em)

A relative unit based on the root (`html`) element's font size.

```css
font-size: 2rem;
```

### Quick Comparison

| Unit  | Relative To       | Usage                        |
| ----- | ----------------- | ---------------------------- |
| `px`  | Fixed size        | Precise sizing               |
| `pt`  | Print measurement | Printing                     |
| `em`  | Parent font size  | Scalable layouts             |
| `rem` | Root font size    | Consistent responsive design |

### `font-weight` Property in CSS

The **`font-weight`** property is used to specify the **thickness (boldness)** of text.

**Syntax:**

```css
font-weight: value;
```

### Common Values

| Value    | Description       |
| -------- | ----------------- |
| `normal` | Normal text (400) |
| `bold`   | Bold text (700)   |
| `100`    | Thin              |
| `300`    | Light             |
| `400`    | Normal            |
| `500`    | Medium            |
| `700`    | Bold              |
| `900`    | Extra Bold        |

### Example

```css
h1 {
    font-weight: bold;
}

p {
    font-weight: 300;
}
```

**Definition:** The `font-weight` property is used to control how thick or bold the text appears.

### `font-family` Property in CSS

The **`font-family`** property is used to specify the **font style (typeface)** of text.

**Syntax:**

```css id="o3r5l7"
font-family: font-name;
```

### Example

```css id="8ws4jr"
h1 {
    font-family: Arial, sans-serif;
}

p {
    font-family: "Times New Roman", serif;
}
```

### Common Font Families

* `Arial`
* `Verdana`
* `Times New Roman`
* `Georgia`
* `Courier New`

In `font-family`, a **backup (fallback) font** is used if the browser cannot load the first font.

### Example

```css id="z7r7v7"
font-family: Arial, Helvetica, sans-serif;
```

**Explanation:**

* First choice: `Arial`
* If Arial is unavailable → `Helvetica`
* If Helvetica is unavailable → `sans-serif`

### Definition

**Fallback fonts (backup fonts)** are alternative fonts specified in the `font-family` property that the browser uses when the preferred font is not available on the user's system.


### Generic Font Families

| Family       | Description                         |
| ------------ | ----------------------------------- |
| `serif`      | Fonts with small decorative strokes |
| `sans-serif` | Clean fonts without strokes         |
| `monospace`  | Each character has equal width      |
| `cursive`    | Handwriting-style fonts             |
| `fantasy`    | Decorative fonts                    |

**Definition:** The `font-family` property is used to set the typeface of text and can include multiple fallback fonts.

### `text-align` Property in CSS

The **`text-align`** property is used to specify the **horizontal alignment of text** inside an element.

**Syntax:**

```css id="k3s4pl"
text-align: value;
```

### Values

| Value     | Description                              |
| --------- | ---------------------------------------- |
| `left`    | Aligns text to the left                  |
| `right`   | Aligns text to the right                 |
| `center`  | Centers the text                         |
| `justify` | Stretches text so both edges are aligned |

### Example

```css id="4lzqf9"
h1 {
    text-align: center;
}

p {
    text-align: justify;
}
```

**Definition:** The `text-align` property is used to control the horizontal alignment of text within an element.
### CSS Box Model Properties

#### 1. Margin

The **margin** is the space **outside** an element's border. It creates distance between the element and other elements.

```css id="ll8k4i"
margin: 20px;
```

#### 2. Border

The **border** is the line that surrounds the padding and content of an element.

```css id="4hk6yi"
border: 5px solid white;
```

#### 3. Padding

The **padding** is the space **inside** the border, between the content and the border.

```css id="1hmhmc"
padding: 10px;
```

### Visual Representation

```text
Margin
 ┌─────────────────┐
 │     Border      │
 │ ┌─────────────┐ │
 │ │   Padding   │ │
 │ │ ┌─────────┐ │ │
 │ │ │ Content │ │ │
 │ │ └─────────┘ │ │
 │ └─────────────┘ │
 └─────────────────┘
```
### I made [Japanese love Poster](https://github.com/Vishnupriya609/webdevelopement/blob/main/Day%207/Output.png)



