# Cascade style sheets (CSS)

## Why that name?

Cascading Style Sheets mainly referred to as CSS, is a simple design language intended to simplify the process of making web pages appealing. Using CSS, you can control the layout of the web page, their font size, and color, variations for display (for different devices and screen sizes) as well as a variety of other effects. CSS is easy to learn and understand as it provides powerful control over the presentation of an HTML document.

## CSS Syntax

CSS files are denoted with the extension `.css` and usually, their name refers to the webpage they are dealing with for example `about.css` would most likely contain all the styles you want to apply to your about page. CSS syntax is a pretty concise one, in CSS is necessary to wrap with `{}` the rules you want to apply to a given element and the rules have the following syntax: `property: value;` the `;` is only required for adding other rules in the next line otherwise you can do it without `;` (i.e: `property: value`).

          .main-wrapper {
             color: #323232;
             font-size: 16px;
             line-height: 1.6;
             text-decoration: none;
          }

In the previous examples. You can see that I want my `main-wrapper` to have a text color of #323232 which is like a medium darker gray, a font size of 16px so the user can understand what is reading without much effort with their eyes, a line-height which is the space that separates text vertically between lines and text-decoration set to `none` for the text to not have any extra styles like underlines, upper lines, etc.

You could write css like the following: 

          .main-wrapper { color: #323232; font-size: 16px; line-height: 1.6; text-decoration: none; }

But is considered a bad practice 'cause it is not very human-readable. That's why is <strong> highly recommended </strong> to write CSS in the following format like I did with the first example. Remember:

          // Badly formatted CSS
          .main-wrapper { color: #323232; font-size: 16px; line-height: 1.6; text-decoration: none; }

         // Nicely formatted CSS
          .main-wrapper {
             color: #323232;
             font-size: 16px;
             line-height: 1.6;
             text-decoration: none;
          }

You can write comments in CSS, which are intended for better code comprehension (that are not executed by the computer) in the following manner:

         // This is an inline and short comment
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

You may ask what does it mean the `.` in the `.main-wrapper` more into that in the following section

## CSS basic selectors 
    TODO
### A note about specificity
    TODO
## The Box Model
    TODO