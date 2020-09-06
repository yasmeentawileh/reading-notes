# Elements to organizing text in html
1. ## Headings 
HTML has six levels of headings the first one called h1 which used for the main heading the  other h from 2 to 6 are used for subheadings h1 is the largest one the text will be big , h6 is the smallest one the text will be small

2. ## paragraph 
To create a paragraph, surround the words that make up the paragraph with an opening tag and closing  tag.

3. ## making text bold or itlaic
< i > < / i > to make text italic ex:<i>italic</i>

< b > < / b > to make text bold ex: <b>bold</b>

< strong > < / strong > to make text bold ex: <strong> strong </strong>

4. ## subscript and superscript
< sup > < / sup >  to make the text superscript ex : 4<sup>th</sup>

< sub > < / sub > to make text subscript ex: H<sub>2</sub>O

5. ## line breaks & horizantal ruler 
<  br / > to  add a line break inside the middle of a paragraph ex: yasmeen <br/> tawileh.

< hr / > To create a break betweenthemes — such as a change of topic in a book or a new scene in a play ex: section 1 <hr/>section 2

**note:** the hr and br tags don't need to have a closing tag ,just one tag.

6. ## quotations: 
< blockquote> < /blockquote> used for longer quotes that take up an entire paragraph.<br/>
you can click on [image](https://i0.wp.com/basecampatx.com/wp-content/uploads/2020/01/die-anleitung-zu-html-quotation.png?fit=688%2C452) to see the result of applying blackquote in html

< q>< /q>  used for shorter quotes that sit within a paragraph.<br/>
you can click on [image](https://o7planning.org/en/12467/images/47184216.png) to see an example of applying quote in html

# CSS
## What is CSS?

CSS means Cascading Style Sheets.it's describes how HTML elements are to be displayed on screen, paper, or in other media and it allows you to create rules that control the way that each individual box (and the contents
of that box) is presented.

## CSS rule
The CSS rile contaions two part: 
1. selector 
Selectors indicate which element the rule applies to,the same rule can apply to more than one element if you separate the element names with commas.

 2. declaration 
 indicate how the elements referred to in the selector should be styled.Declarations are split into two parts (a property and a value),and are separated by a colon.
  
![](1_1.png)

## CSS types:
1. External 

External CSS contains separate CSS file which contains only style property with the help of tag attributes
to link it with HTML page you have to write inside the head tag the link element which contaion three attributes.
click on [image](https://image.slidesharecdn.com/npblended3et03-140220213041-phpapp02/95/introducing-cascading-style-sheets-16-638.jpg?cb=1392931920) to see how to link the CSS file to HTML

2. internal 

we can style the document in the same HTML file by adding them inside a < style> element,
which usually sits inside the < head> element of the page.

3. inline

 Inline CSS contains the CSS property in the body section attached with element is known as inline CSS. This kind of style is specified within an HTML tag using the style attribute.

here is an [image](https://www.bitdegree.org/learn/storage/media/images/8c4493d3-110c-4a95-8b70-7626ce2d2f4e.jpg) to understand the diffirent between them.<br/>

# JAVASCRIPT
## Meaning of script and statement
 *script:* is a series of instructions that a computer can follow one-by-one.
 *statment:* Each individual instruction or step is known as a statement. 
  
  ## Why you should write comments ?
you should write comments to explain what your code does.They help make your code easier to read and understand.This can help you and others who read your code. 

## Why we use variable?
we use variable to temporarily store the bits of information that the script need it to do its job.

## Array meaning:
An array is a special type of variable. It doesn't just store one value; it stores a list of values.

## When we use array?
whenever you are working with a list or a set of values that are related to each other. it's realy helpful when you do not know how many items a list will contain because, when you create the array, you do not need to specify how many values it will hold. 

## How the operators work?
The operators allow programmers to create a single value from one or more values. 

### Types of operators
1. Arithmetic operators 

click on [image](https://ecomputernotes.com/images/stories/arithmetic%20operators.jpg) to know them 

2. String operators

There is just one string operator: the + symbol.It is used to join the strings on either side of it. 

## Decisions and loops

### **comparison operator:**

1. ==

this means equal to it gives true if they are equal.

2. !=

not equal to it gives true if they are not equal.

3. ===

strict equal to they must by the same data type and value to gives true.

4. !==

strict not equal to it gives true if they are not the same data type or the same value or both.

5. >

greater than checks if the number on the left is greater than the number on the right if it's greater it will give you true

6. <

less than cheks if the number on the left is less than the number on the right if it's less it will give you true.

7. >=

greater than or equal checks if the number on the left is greater than or equal the number on the right if it's greater or equal it will give you true.

8. <=

less than or equal cheks if the number on the left is less than or equal the number on the right if it's less or equal it will give you true.

### **structuring comparison operator**
in the left you will put opening bracket then write operand between brackets  then the comperasion operator then another operand between brackets then put the closing bracket.
 
 ![image](operator.png)
 
### **Logical operator:**

1. &&  logical *AND*

if both expressions evaluate to true then the result will be true otherwise it will returan false

2. | |  logical *OR* 

if one of the expressions evaluate to true then the result will be true the only way to get false that all of the expressions evaluate to false

3. !  Logical *Not*

this reverses the state of an expression if it was false it will return it to true and if it was true it will make it false.



# loops:
loops are used to repeatedly run a block of code - until a certain condition is met.
## loops types:
1. for loop 
it is used to run code a specific number of times.
2. while loop
it is used if you don't know many times the code should be run.
## FOR loop syntax:
click on [image](https://www.google.com/url?sa=i&url=https%3A%2F%2Fpt.slideshare.net%2FBaabtraMentoringPartner%2Floops-in-c%2F5&psig=AOvVaw3gS5Et72JL1b43BaI3XLFP&ust=1598540903173000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCOCn6IuVuesCFQAAAAAdAAAAABAD)

## for while loop syntax:
click on [image](https://web.engr.oregonstate.edu/~rookert/cs162/ecampus-video/CS161/template/chapter_5/chapter5_images/5_01.png)
 

