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
### A note about specificity
    >Specificity of CSS elements determine which style rule is applied to an element. That is if multiple CSS selectors
    are targeting the same HTML element, the highest specific selector will take effect.
    
    Specificity order: id selector>class selector>Element selector
## The Box Model
    TODO
