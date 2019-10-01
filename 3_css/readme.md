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

          .text-gray {
             color: #323232
          }

Otherwise...

          .main-wrapper {
             color: #323232;
             font-size: 16px;
             line-height: 1.6;
             text-decoration: none;
          }

Following along you can see in the previous example that I want my `main-wrapper` to have

- A color of #323232 which is like a medium darker gray
- font size of 16px
- line-height (which is the space that separates text vertically between lines) and helps with reading comprehension.
- And text-decoration set to `none` (to remove extra styles like underlines, upper lines, etc.)

This rules only applies to the `.main-wrapper`, which is a class selector (we'll be explaining what class selectors are further more in the next section) for now jus remember how is called.

#### Formating

There is two ways of writting CSS 

- inline: That is considered a bad practice 'cause it is not very human-readable.

          .main-wrapper { color: #323232; font-size: 16px; line-height: 1.6; text-decoration: none; } 

- block: <strong> Highly recommended </strong> for human readability

          .main-wrapper {
             color: #323232;
             font-size: 16px;
             line-height: 1.6;
             text-decoration: none;
          }

#### Comments

Comments are intended for better code comprehension, this are pieces of the code that are not executed by the computer, and in CSS are written in the following manner:

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

## CSS basic selectors 
    TODO
### A note about specificity
    TODO
## The Box Model
    TODO