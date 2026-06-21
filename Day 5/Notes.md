# File Paths
## What is a File Path?

### A file path is the address that tells the browser where a file is located. It is used to access images, web pages, CSS files, JavaScript files, videos, and other resources.
```
<img src="images/photo.jpg" alt="Photo">
```
### Here, images/photo.jpg is the file path.
## Types of File Paths
### 1. Absolute File Path: An absolute path provides the complete location of a file.
#### Using a Website URL
```
<img src="https://example.com/images/photo.jpg" alt="Photo">
```
#### Local Computer Path (Not Recommended)
```
<img src="C:\Users\Vishnu\Pictures\photo.jpg" alt="Photo">
```
#### Advantages:

- Gives the exact file location.

#### Disadvantages:

- Local computer paths do not work for other users.
-Less portable than relative paths.


### 2. Relative File Path: A relative path specifies the location of a file relative to the current HTML file.
#### Same Folder
```
<a href="about.html">About</a>
```
#### Child Folder
```
<img src="./images/photo.jpg" alt="Photo">
```
#### Parent Folder
```
<img src="../photo.jpg" alt="Photo">
```
| Symbol   | Meaning            |
| -------- | ------------------ |
| `./`     | Current directory  |
| `../`    | Parent directory   |
| `../../` | Two directories up |

#### Advantages:

- Easy to maintain.
- Works when moving the entire project.
- Commonly used in web development.

# Web Pages
## A web page is a document displayed in a web browser. It is created using HTML and can be styled with CSS and made interactive with JavaScript.
### Examples of Web Pages
- Home Page
- About Me Page
- Contact Me Page
- Portfolio Page
- Login Page

## Website VS Web Pages

| Web Page               | Website                   |
| ---------------------- | ------------------------- |
| A single page/document | A collection of web pages |
| About Me page          | Portfolio website         |
```
<h1>Welcome to My Portfolio</h1>

<a href="about.html">About Me</a>
<a href="contact.html">Contact Me</a>
```

### Each page is a web page. Together, they form a website.

# HTML Boilerplate

An **HTML Boilerplate** is the basic template or skeleton of every HTML document. It contains the essential tags required for a webpage to work properly.

## Standard HTML Boilerplate

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Website</title>
</head>
<body>

</body>
</html>
```

---

## Explanation

### 1. `<!DOCTYPE html>`

Tells the browser that this document uses **HTML5**.

```html
<!DOCTYPE html>
```

---

### 2. `<html>`

The root element of the webpage.

```html
<html lang="en">
```

* `lang="en"` specifies that the page content is in English.

---

### 3. `<head>`

Contains information about the webpage that is not directly displayed.

```html
<head>
</head>
```

---

### 4. `<meta charset="UTF-8">`

Sets the character encoding.

```html
<meta charset="UTF-8">
```

Allows proper display of:

* English
* Telugu
* Japanese
* Hindi
* Other languages

---

### 5. `<meta name="viewport">`

Makes the webpage responsive on mobile devices.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

---

### 6. `<title>`

Sets the title shown in the browser tab.

```html
<title>My Website</title>
```

---

### 7. `<body>`

Contains all visible content.

```html
<body>
    <h1>Hello World</h1>
</body>
```

---

## Structure Diagram

```text
HTML Document
│
├── <!DOCTYPE html>
└── <html>
    │
    ├── <head>
    │   ├── meta
    │   └── title
    │
    └── <body>
        └── Visible Content
```

---

## Why Use a Boilerplate?

✅ Provides a standard structure
✅ Ensures browser compatibility
✅ Supports multiple languages with UTF-8
✅ Makes websites mobile-friendly
✅ Serves as the starting point for every webpage

### Easy Memory Trick

```text
DOCTYPE → HTML → HEAD → BODY
```

Every HTML page starts with this basic structure. 🚀


## Web Hosting
### Web hosting is a service that stores your website files and makes them available on the internet so anyone can access them using a URL.

### Without Hosting
```
Your Computer
     ↓
index.html
```
#### Called local development

### With Hosting
Your Website Files
        ↓
Web Hosting Server
        ↓
    Internet
        ↓
   Visitors
#### Anyone can access your website from anywhere.

## Types of Web Hosting
### 1. Free Hosting
Good for beginners and portfolio websites.
Examples:

- GitHub Pages
- Netlify
- Vercel
### 2. Paid Hosting

### Used for business and production websites.

Examples:

- Hostinger
- Bluehost

## Complete flow in github

Create Website
      ↓
Upload to Hosting
      ↓
Hosting Server Stores Files
      ↓
User Opens URL
      ↓
Server Receives Request
      ↓
Server Sends Files
      ↓
Browser Renders Website
      ↓
Website Displayed


