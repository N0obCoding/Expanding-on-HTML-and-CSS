# Cascade style sheets (CSS)

## Why that name?

Cascading Style Sheets mainly referred to as CSS, is a simple design language intended to simplify the process of making web pages appealing. Using CSS, you can control the layout of the web page, their font size, and color, variations for display (for different devices and screen sizes) as well as a variety of other effects. CSS is easy to learn and understand as it provides powerful control over the presentation of an HTML document.

## CSS Syntax

#### Definition

CSS files are denoted with the extension `.css` and usually, their name refers to the webpage they are dealing with. For example `about.css` would most likely contain all the styles you want to apply to your about page.

CSS has a pretty and concise syntax

1) The rules need to be wrap within `{}`

2) They follow the pattern: `property: value;` (where `;` is only required for when adding multiple rules)

For example if we have a rule that only applies color to a given text, there is no need to append the `;` at the end of the line.

``` CSS
.text-gray {
    color: #323232
}
```
Otherwise...

``` CSS
.main-wrapper {
     color: #323232;
     font-size: 16px;
     line-height: 1.6;
     text-decoration: none;
}
```

Following along you can see in the previous example that I want my `main-wrapper` to have

- A color of #323232 which is like a medium darker gray
- font size of 16px
- line-height (which is the space that separates text vertically between lines) and helps with reading comprehension.
- And text-decoration set to `none` (to remove any extra styles like underlines, upper lines, etc.)

This rules only applies to the `.main-wrapper`, which is a class selector (we'll be explaining what class selectors are further more in the next section)

#### Formating

There is two ways of writting CSS 

- inline: That is considered a bad practice 'cause it is not very human-readable.
``` CSS
.main-wrapper { color: #323232; font-size: 16px; line-height: 1.6; text-decoration: none; } 
```
- block: <strong> Highly recommended </strong> for human readability
``` CSS
.main-wrapper {
     color: #323232;
     font-size: 16px;
     line-height: 1.6;
     text-decoration: none;
}
```
#### Comments

Comments are intended for better code comprehension, this are pieces of the code that are not executed by the computer, and in CSS are written in the following manner:

``` CSS
/ This is an inline and short comment
.main-wrapper {
   color: #323232;
   font-size: 16px;
   line-height: 1.6;
   text-decoration: none;
}

/* --------------------------------------------------
** This is a huge and extensive comment that
** requires many lines to be able to be read properly.
** --------------------------------------------------
*/
.main-wrapper {
   color: #323232;
   font-size: 16px;
   line-height: 1.6;
   text-decoration: none;
}
```
## CSS basic selectors 
    CSS selectors are used to select the HTML element that we want to style.
    Basic selectors in CSS are the following:
    
    1) Element selector: Selects HTML element using their name.
    2) ID selector: Selects HTML element using their id attribute. Usage: Hash(#) followed by id.
    3) Class selector: Selects HTML element using their class name. Usage: Period(.) followed by class name.
    4) Universal selector: Selects all HTML elements in the page. Usage: Asterisk(*) is used as universal selector
    
- <strong>Type selector </strong>lets us modify the properties of the element we are specifying. In the following code we are selecting all the 'h3' tags in our file and modifying its color to be red.
``` CSS
h3 {
    color: red;
}
```
- <strong>.class selector</strong> matches all elements which belongs to a particular class attribute. For example, let's say we have an specific text, that only displays "Hello N0obCoding!", which belongs to the "greetings" class. We want to modify this single element without affecting the rest. Notice that a .class selector, is preceded by a dot.

``` HTML
<h3 class="greetings">
	Hello N0obCoding!
</h3>

<style>
.greetings {
	color: green; /* <- our awesome text decoration */
}
</style>
```
You can notice that we are using the ```<style>``` here. This tag let us write CSS code inside our HTML file! Is not that cool?

- <strong>#id selector</strong> since we can assign identifiers (id) to an HTML element, we can then modify its properties by referencing this unique identifier in our CSS code. This can be done by the following:
``` HTML
<div id="uniqueid">I have an identifier!</div> 

<div>I don't have an identifier</div>

<style>
#uniqueid{
    background-color: #FFA500;
    padding: 20px;
}
</style>
```
<strong>* Universal selector</strong> What if we want that all of our page have a specific background color or font? CSS allows us to do this by using its universal selector '*' , where any of our elements will have the property we're specifying. In the following example, we are selecting all elements, and set their background color to aqua.
``` CSS
* {    
	background-color: #00FFFF;   
}
```
No one told us that CSS selectors could be so easy! 
### A note about specificity
    Specificity of CSS elements determine which style rule is applied to an element. That is if multiple CSS selectors
    are targeting the same HTML element, the highest specific selector will take effect.
    
    Specificity order: ID selector > Class selector > Element selector
## The Box Model
    TODO
