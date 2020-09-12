# What's the hardest thing about programming 
The hardest thing about programming is learning the problem domain.

## Why problem domains are hard 
  Writing code is a lot like putting together a jigsaw puzzle.  We put together code with the purpose of building components that we have taken out of the “bigger picture” of the problem domain.The big issue is that many problem domains are like a puzzle with a blurry picture or no picture at all. and as programmers, we also are often not given complete information about the problem domain, so we don’t even have the information we need to understand it.

  ## What you can do about this problem ?

**1. Make the problem domain easier**
**2. Get better at understanding the problem domain**

## How to make proble domain easier?
You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem then after you understand  start to expand the problem domain. 

## How to get better at understanding the problem domain?
You can get better understanding by sitting down and talking to customers or business people who know about the problem domain, and before trying to solve the problem domain with code you have to make sure you understand a problem inside and out.

# Java script

# What is an object ?
Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names. so the varibales become known as properties which will tell us about the object, and the functions will be known as methods which represent tasks that are associated with
the object.

# How to create it?
![image](objectmethod.png)

# What's the meaning of document object model DOM

The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window. 

The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules.It is implemented by all major browser makers, and covers two primary areas: 
- first area:  making a model of the HTML page ,When the browser loads a web page, it creates a model of the page in memory.The DOM specifies the way in which the browser should structure this model using a DOM tree.
- second area: Accessing and changing the HTML page ,The DOM also defines methods and properties to access and update each object in this model, which in turn updates what the user sees in the browser.

# Working with the DOM tree
Accessing and updating the DOM tree involves two steps:

1. Locate the node that represents the element you want to work with.

2.  Use its text content, child elements, and attributes. 

## Step 1 How to access the elements ?

![image2](access.png)

## Step 2: work with those elemnts

![image3](step2.png)

# Caching dom queries
Methods that find elemnts in the DOM tree called DOM queries.Ex: getElementById('one');

*Note: when you need to work with an element more than once, you should use a variable to store the result of this query*

when you store elements in variable you are actually storing the location of the element(s) within the DOM tree in a variable.the properies and methods of that element node work on the variable 
Ex: var itemOne = getElementById('one');

# How to access elements?
DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes. 

## Methods return a single element node
**1. getElementByld('id')**

Selects an individual element given the value of its i d attribute . 

**2. querySelector( 'css selector')**

Uses CSS selector syntax that would select one or more elements .This method returns only the first of the matching elements. 

![image](getelement.png)
## Methods that return one or more elemnts ( as a nodelist)
 
**1. getElementsByClassName('class)**

Selects one or more elements given the value of their class attribute.The HTML must have a cl ass attribute for it to be selectable.This method is faster than querySelectorA11 () . 

**2. getElementsByTagName('tagName')**

Selects all elements on the page with the specified tag name.This method is faster than querySelectorA11 (). 

**3.querySelectorAll ('css selector')**

Uses CSS selector syntax to select one or more elements and returns all of those that match. 

# nodelist
nodelist: a collection of element nodes. Each node is given an index number (a number that starts at zero, just like an array). 

## nodelist properties:
• The length property tells you how many items are in the Nodelist.
• The item() method returns a specific node from the Nodelist when you tell it the index number of the item that you want (in the parentheses).However, it is more common to use array syntax

## Types of nodelist:
1. live nodelist

In a live Nodelist, when your script updates the page, the Nodelist is updated at the same time.The methods beginning getEl ementsBy_ return live Node lists. They are also typically faster to generate than static Nodelists. The new methods that begin querySelector._(which use CSS selector syntax) return staticNodelists

2. Static nodelist

In a static Nodelist when your script updates the page, the NodeList is not updated to reflect the changes made by the script. 

## Selecting an elements from nodelist
**1. THE item() METHOD**
Nodelists have a methodcalled item() which will return an individual node from the Node list.You specify the index number of the element you want as a parameter of the method (inside the parentheses). 

![image4](stepsitem.png)

**2. Array syntax method**
Array syntax is prefered over the item method because it's faster. before selecting a node from nodelist check that it contaions nodes.

![arraysyntax.png]

# Traversing the DOM 
When you have an element node, you can select another element in relation to it using these five properties

- parentNode :This property finds the element node for the containing (or parent) element in the HTML.

- previousSibling and nextSibling:These properties find the previous or next sibling of a node if there are siblings. 

- firstChild and lastChild: These properties find the first or last child of the current element. 

# Access and update a text node with node value 

![image](nodevalue.png)

# Adding or removing HTML content

1. The inner html property

 - adding content

 a. storing new content (including markup) as a string in a variable 

 b. select the element whose content you want to replace

 c. set the element's innerHTML property to be the new string

 - removing content 
 
 to remove all content from an element,you set innerHTML to an empty string .

 2. DOM manipulation method 

 - Adding content

 to add content you use a DOM method to create new content pne node at a time and store it in a variable then another DOM  method is used to attach it to the right place in the DOM tree

 - removing content

 you can remove an element using single method

 # Adding elemnts using DOM manipulation

 DOM manipulation offers another technique to add new content to a page (rather thaninnerHTML). It involves three steps:

 1. CREATE THE ELEMENT

 code: createElement ()

You start by creating a new element node using the createElement() method.This element node is stored in a variable.When the element node is created, it is not yet part of the DOM tree. 

2. give it content

code:createTextNode() 

This provides the content for the element, although you can skip this step if you want to attach an empty element to the DOM tree. 

3. ADD IT TO THE DOM 

code:appendChild() 

Now that you have your element (optionally with some content in a text node), you can add t to the DOM tree using the appendChild () method. The appendChild() method allows you to specify which element you want this nodeadded to, as a child of it. 

# Removing elements using DOM manipulation

1. STORE THE ELEMENT TO BE REMOVED IN A VARIABLE 

You start by selecting the element that is going to be removed and store that element node in a variable.You can use any of the methods you saw in the section on DOM queries to select the element. 

2. STORE THE PARENT OF THAT ELEMENT IN A VARIABLE

Next, you find the parent element that contains the element you want to remove and store that element node in a variable. The simplest way to get this element is to use the parentNode property of this element. 

3. REMOVE THE ELEMENT FROM ITS CONTAINING ELEMENT 

The removeChild() method is used on the containing element that you selected in step 2.
The removeChild() method takes one parameter: the reference to the element that you no longer want. 
