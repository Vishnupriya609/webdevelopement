# Intermediate HTML
## List Elements
 Used to organize and display related items in a structured format.
List Item  – Represents an individual item inside a list.
## Ordered List  

Displays items in a specific order using numbers or letters.

```
<ol>
    <li>Wake Up</li>
    <li>Brush Teeth</li>
    <li>Eat Breakfast</li>
    <li>Study HTML</li>
</ol>
```
## Unordered List  

Displays items using bullet points where order does not matter.
```
<ul>
    <li>Rava</li>
    <li>Water</li>
    <li>Onion</li>
    <li>Salt</li>
</ul>
```
## Description List 

Used to display a list of terms and their corresponding descriptions.

 <dt> – Description Term (the term/title)

 <dd> – Description Definition (the description/explanation)
```
<dl>
    <dt>HTML</dt>
    <dd>HyperText Markup Language</dd>

    <dt>CSS</dt>
    <dd>Cascading Style Sheets</dd>

    <dt>Java</dt>
    <dd>A programming language</dd>
</dl>
```
## Nesting & Indentation
Nesting means placing one HTML element inside another HTML element.
```
<ul>
    <li>Programming Languages
        <ul>
            <li>Java</li>
            <li>Python</li>
        </ul>
    </li>
</ul>
```
Indentation means adding spaces or tabs before nested elements to make the code easy to read.
### Benefits
○ Improves code readability
○ Makes debugging easier
○ Clearly shows parent-child relationships
○ Keeps code clean and maintainable
```
<ul>
    <li>Java</li>
    <li>Python</li>
</ul>
```

## Anchor Element
Used to create hyperlinks that allow users to navigate from one page to another page, website, email, or phone number.

```
<a href="https://www.google.com">Visit Google</a>
```
### Types of Links

○ External Link – Links to another website.

○ Internal Link – Links to another page within the same website.

○ Email Link – Opens the user's email application.

○ Phone Link – Allows calling a phone number on supported devices.
 Examples: Navigation menus

## Attributes
Attributes add additional information to tag.we can no.of attributes
Example: href,draggable,start,type
```
<a href="https://www.google.com"
   target="_blank"
   type="text/html"
   draggable="true">
   Visit Google
</a>
```
## Image Element
 Used to display images on a web page.
```
<img src="nature.jpg" alt="Beautiful Nature" width="300" height="200">
```
## Common Attributes

○ src – Specifies the path or URL of the image.

○ alt – Alternative text displayed if the image cannot be loaded.

○ width – Sets the width of the image.

○ height – Sets the height of the image.

○ title – Displays a tooltip when hovering over the image.

○ draggable – Makes the image draggable (true or false).

 Example:Profile photos,logos,blog posts,photo galleries
## Project
[Birthday Invite Project](https://github.com/Vishnupriya609/webdevelopement/blob/main/Day%204/index.html) in code used the anchor,image,lists,headings elements

