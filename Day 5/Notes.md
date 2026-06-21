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

Portfolio Website
│
├── Home Page
├── About Me Page
├── Contact Me Page
└── Projects Page
