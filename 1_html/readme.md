# HTML

Hypertext Markup Language (HTML) is the standard markup language for documents designed to be displayed in a web browser. HTML describes the structure of a web page semantically. [Wikipedia](https://en.wikipedia.org/wiki/HTML)

HTML consists of several *elements* which are used to modify different parts of the content such as: adding headings, paragraphs, images, making the text bold or italic etc. An element can be created with the help of a *tag* by enclosing the name of the element within the starting tag <"name"> and closing it with the ending tag <\"name"> 

**Note:** in empty elements, the end tag is not allowed. For example, to insert a single line break we use the <br> tag which is an empty tag and hence is not followed by a ending tag.

We can also add comments to our code. HTML comments are visible to anyone that views the source code, but are not displayed in the browser. They are useful to make the code more concise and easier to understand. An HTML comment begins with ```<!––``` and closes with ```––>```.
consider the line "What is HTML?"
If we wanted this line to be displayed in the browser by itself we could specify that it is a para by enclosing in the paragraph tags. 

``` <p> What is HTML? <\p> ```
    
## The anatomy of the HTML Document
HTML elements are the building blocks of HTML page. [Wikipedia](https://en.wikipedia.org/wiki/HTML)
> An HTML document is composed of several different elements arranged in the following way:
```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>My test page</title>
  </head>
  <body>
    <p>This is my page</p>
  </body>
</html>
```
 
 The different parts of this document are:
 1. `<!DOCTYPE html>` : The doctype. Initially, doctypes were links to a set of rules which decided whether the HTML qualified as a good page. Nowadays, instead of using several different doctypes we just use <!DOCTYPE html> which is the shortest string of characters that counts as a valid doctype to make our page work right.   

2. `<html></html>`: The `<html>` element. This element wraps all the content on the entire page.   

3. `<head></head>`: The `<head>` element. This element acts as a container for things which you don't want to show to the viewer. This includes things like keywords, a page description that you want to appear in search results, links to CSS or Javascript files, character set declarations, etc.

4. `<meta charset="utf-8">`: This element sets the character set of your document to UTF-8, which includes most characters from majority of the human written languages.

5. `<title></title>`: The `<title>` element. This sets the title of your page, which is the title that appears in the browser tab on opening the page, and is used to describe the page when you bookmark it.

6. `<body></body>`: The <body> element. This contains all the content that you want to show the viewers when they visit your page, which can be text, images, gifs, videos etc.  

## Whitespace in HTML
In HTML the use of whitespace is only to improve code readability. i.e. the HTML parser reduces any amount of whitespace to a single whitespace. In the following example, both paragraphs will be rendered the same way.

 ```
 <p> no extra whitespace <\p>
 
 <p> lots 
   of   extra   
   whitespace    <\p>
 ```

## Semantic HTML
Semantic tags in HTML are used to provide information about meaning of the web page to the browser rather than just presentaion. 

For example, the tags `<div\>` and `<span\>` are non semantic tags, they only define structure of the web page. However, tags like `<table\>` and `<article\>` clearly define their content.

### Why should we use it?
Semantic tags make the code more readable and easier to maintain. It also improves automated processing of documents.

### Accessibility from day one!
    TODO
## Consuming external resources through links
In HTML, we can access external web pages using the anchor tag. The anchor tag is denoted by `<a>`
```
<a href="https://github.com">Clicking me will open the github page</a>
```
The `href` attribute refers to Hypertext reference and may contain like to an external web page or an internal section in the current page as its value. The `<a>` tag can enclose any other tag and is capable of converting it into a link. 

---
This work is licensed under the Creative Commons Attribution-ShareAlike 4.0 International License. To view a copy of this license, visit [http://creativecommons.org/licenses/by-sa/4.0/](http://creativecommons.org/licenses/by-sa/4.0/).
