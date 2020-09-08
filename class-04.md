# HTML
# Links:
**Why we use links?** we use links to allow the user to move from one web page to another 

## How to insert links to HTML?

Links are created using the < a> element. Users can click on anything
between the opening < a> tag and the closing </ a> tag. You specify
which page you want to link to using the href attribute.
*We can use it to linking to other sites or to link to other pages in the same site*

## How to link a specific part on the same site 
Before you can link to a specific part of a page, you need to identify the points in the page that the link will go to. You do this using the id attribute .

## linking to a specific part of of another page
As long as the page you are linking to has id attributes that identifyspecific parts of the page, you can simply add the same syntax to the end of the link for that page.

# How to layout your webpage
Before starting to layout you have to know that CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.

## Different between inline box and block-level box
**Block-level boxes:**  start on a new line and act as the main building blocks of any layout.*ex:h1,p,ul,li.*

 **inline boxes :**flow between surrounding text. You can
control how much space each box takes up by setting the width of the boxes (and sometimes the height, too). To separate boxes, you can use borders, margins, padding, and background colors. *ex:img ,b , i*

# What's the containing element:
If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

# Controlling the position of elements:
CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the position property in CSS. You can also float elements using the float property.

## Types of floats:
**1. normal flow:**

Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one. way in which browsers treatway in which browsers treat .

*Note:  you do not need a CSS property to indicate that elements should appear in normal flow, but the syntax
would be:
position: static;*

**2. relative positioning:**

This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. This does not affect the position of surrounding elements; they stay in the position they would be in normal flow.

**3. absolute positioning:**

This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements(as they simply ignore the space it would have taken up).Absolutely positioned elements move as users scroll up and down the page.

## Floating elemnts :

The float property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible

*Note:When you use the float property, you should also use the width property to indicate how wide the floated element should be. If you do not, results can be inconsistent but the box is likely to take up the full width of the containing element (just like it
would in normal flow).*

## Uses of floats:
 
 You can use float to place elemnts side by side.When elements are floated, the height of the boxes can affect where the following elements sit.

## Use of clear float:

The clear property allows you to say that no element (withinthe same containing element) should touch the left or righthand sides of a box. It can take the following values:**left,right,both,none**

## Problem you might face in float:
If a containing element only contains floated elements, some browsers will treat it as if it is zero pixels tall.

## How to fix the problem 

The pure CSS solution adds two CSS rules to the containing element:The overflow property is
given a value auto.The width property is set to 100%.

## How to create multi-column layouts using floats

Many web pages use multiple columns in their design. This is achieved by using a < div> element to represent each column. The following three CSS properties are used to position the columns next to each other:
- width:This sets the width of the
columns.
- float:This positions the columns next
to each other.
- margin:This creates a gap between the
columns.

# JavaScript
# What is a function?
Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements). 

## Benefit of using function:
Grouping together the statements that are required to answer a question or perform a task  helps organize your code. 

## Reason to give your function a name
If you are going to ask the function to perform its task later you need to give your function a name that name should describe the task it is performing .

## calling function:
when you ask the function to perform the task it's called calling function

## Parametrs:
some functions need to be provided with information in order to achieve a given task these pieces of information known as a parametrs.

## Return value:
when you write a function and you expect it to provide you with an answer ,the response called return value.

# How to create a function :
to create a function you give it a name and then write the statements needed to achieve its task inside the curly braces 

## How to call a function
Having a declared function  let you execute all of statements between it's curly braces with just one line of code. to call it you will write the function name followed by parentheses.



