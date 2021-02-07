# Chapter 2 : Text
this chapter talk about how we can add markup the text that appears in pages and this markup divided to two type first one is semantics add extra information to the pages, and the second is strctural.
* as we known HTML  has six size of heading from `<h1>` to `<h6>`, `<h1>` is the largest one and the smallest is `<h6>`.
* text is easier to understand when we split it up into small unit of text, we can do that by tag which called `<p>`
**what is the paragraph?** the paragraph is a set of line that aline together in same block, and the new paragraph indicated by new line!
* to adjst your text in web page, you can use different tags like this, for example, **what we will use to make text bold?**
the answer is : we can use tag `<b>`your text`</b>` to make bold in the text.
and now, *what we will use to make text italic?*
again the answer is : we can use tag `<i>`your text `</i>` 
* now we need to talk about the **superScript** and **subScript**, we use the super to make the characters that should be superscript suchas the  dates or mathematical forms like number to a power.  we use the `<sup>` tag, so we write 4 `<sup>2</sup>` this means the number for to the power 2 is equal to 16. 
but if we need to write text that contain characters that should be subscript we ust the `<sub>` tag it is commonly used on chemical
formulas, so we write H`<sub>2</sub>`O to appears h2o.

now how we can make our text readable? 
we knows the special characters that we use in our text to make our code or any paragraph in the world readable is space !
so we use an extra space between our text in the page to make code easier to read, but in the web if we add two space behind each other it see like a one space, **similarly** if it comes via a line break, it treats as a single space and this is indicate the **white space collapsing**, the main purpose to use the white space collapsing is to indent the code in order to make it easier to read and follow it.
* as I mentions above if we need to start a new paragraph we use the new line by press enter key ! but if we need to add a new line and show the empty line for example I need to add a new line inside the
middle of a paragraph in our web page we use the tag `<br />`.
*  I have an important question I wanna to ask, **can we add a horizontal rule between sections in web page?**
the programmer always need to modify the code, and when we say modify so we think about delete some feature or section and add another, so how it can be done ? in simple way we use the `<hr />` tags to add a
horizontal rule between sections.
**to know** the `<br />` tag and `<hr />` tag are known as empty elements.
so now, **what is the empty element?**
elements that do not have any words between an opening and closing tag. and they are written differently, empty element has only one tag. 
*NOTE THAT* before the closing angled bracket of an empty element there will often be a space and a forward slash character.
*  now, we have two views of the page that we are creating:
1- a visual editor 2- code view.
**visual editor** it's contain some features common to most editors
that allow to control the text like how the text will be presented, and allow you to format text (such as Word) into a visual editor by using copy and past, so just you need to copy your text from word and then past into the visual editors! "easy right :) "
**Code views** just to  show the code that created by the visual editor so you can manually edit it, by adding or deleting a line of code, in this scope White space may be added to the code automatically by the editor in order to make the code able or easier to read.
* semantic markup :purpose to use it, to describe the content of web pages more accurately. for example we use `<em>`and `<blockquote>`, `<em>` to make *italic* and `<bllockquoute>` to indented, and you **shouldn't** 
use this tag to change the way that your text looks like!
strong tag indicates that its content has strong importance, by default browsers show the contents of this tag is bold.
# Chpter 10: Introducing CSS
CSS rule contains two parts: a selector and a declaration

> ![the_part_of_CSS](201/CSS1.jpg)

Declarations indicate how the elements referred to in the selector should be styled. declarations are split into two parts 
1- a property 
2- a value 
* this two parts  separated by a colon.
### We Can use CSS In :
Selectors indicate which element the rule applies to. Declarations indicate how the elements referred to in the selector should be styled.Declarations are split into two parts (a property and a value),and are separated by a colon.
`<Inline>` : It’s used to apply css style for a one element. 
`<Internal>` : `<style>` You can also include CSS rules within an HTML page by placing them inside a style element.
 `External`: The <link> element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. It is an empty element (meaning it does not need a closing tag), and it lives inside the `<head>` element. 
 It should use three attributes: `<href>` ,`<type>`,`<rel>`.

 # CSS Selectors :
 There are many different typesof CSS selector that allow you to target rules to specific elementsin an HTML document.

 |`Selector`| meaning    |Example|
 |----------   |-------    |-------|
 |`Universal Selector`   |Applies to all elements in the document       |* { } Targets all elements on the page|
 |`Type Selector`   |Matches element names    |h1,h2,h3 { } Targets the `<h1>`, `<h2>` and `<h3>` elements|

 |`Class Selector`   |Matches an element whose class attribute has a value thatmatches the one specified after the period (or full stop) symbol    |.note `{ }` Targets any element whose class attribute has a value of note|
 |`ID Selector`    |Matches an element whose id attribute has a value that matches the one specified afterthe pound or hash symbol    |#introduction { } Targets the element whose id attribute has a value of introduction|

