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

## Floating elements :

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
- width:This sets the width of the columns.
- float:This positions the columns next to each other.
- margin:This creates a gap between the columns.

# Fixed and Liquied layout
**1. Fixed Layout**
Fixed width layout designs do not change size as the user increases or decreases the size of their browser window.Measurements tend to be given in pixels.

**Advantages**                                                                        
- Pixel values are accurate at controlling size andpositioning of elements.  
- The designer has far greater control over the appearance and position of items on the page than with liquid layouts.
- You can control the lengths of lines of text regardless of the size of the user's window.
- The size of an image will always remain the same relative to the rest of the page.

**Disadvantages**
- You can end up with big gaps around the edge of a page.
- If the user's screen is a much higher resolution than the designer's screen, the page can look smaller and text can be harder to read.
- If a user increases font sizes, text might not fit into the allotted spaces.
- The design works best on devices that have a site or resolution similar to that of desktop or laptop computers.
- The page will often take up more vertical space than a liquid layout with the same
content.

**2.Liquid Layout**
Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window.They tend touse percentages.

**Advantages** 
- Pages expand to fill the entire browser window so there are no spaces around the page
on a large screen.
- If the user has a small window, the page can contract to fit it without the user having to scroll to the
side. 
- The design is tolerant of users setting font sizes larger than the designer intended
(because the page can stretch).

**Disadvantages**
- If you do not control the width of sections of the page then the design can look very different than you intended,with unexpected gaps around certain elements or items squashed together 
- If the user has a wide window, lines of text can become very long, which makes them harder to read.
- If the user has a very narrow window, words may be squashed and you can end up with few words on each line.
-  If a fixed width item (such as an image) is in a box that is too small to hold it (because the user has made the window smaller) the image can overflow over the text.