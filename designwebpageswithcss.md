# Design-Web-Pages-with-CSS

## What is CSS

In the previous module, we learned how HTML uses different features such as headers, which will look larger than regular text, how paragraphs break onto the next line and have space between them, and how links are a different color, to make them noticeable from normal text. In HTML these features are known as default styles, which are very basic styles that the browser applies, to make sure that it's basically readable, even if no noticeable style is made specific by the author. The browser fashions HTML documents in an internal style sheet. With CSS you can control exactly how these HTML elements will look in the browser.  *(Mozilla and Individual Contributors, “What is CSS”, 2005-2021)*

CSS stands for Cascading Style Sheets, and it's a language that specifies how documents are presented, styled, and laid out to users. Other things that CSS is used for in basic document text styling include changing the color and size of headings and links, creating a layout from a single column of text, into a layout with a main content area, and a sidebar for related information. CSS can also be used for animation. *(Mozilla and Individual Contributors, “What is CSS”, 2005-2021)*

### CSS syntax

CSS is a language based on rules. Specifically, this means that the rules are defined by you, and you specify which groups of styles should be applied to an exacting element, or groups of elements on your web page. For example, if you want the main heading on your page to be shown as large red text, you would write it in CSS as:

h1 {
    color: red;
    font-size: 5em;
}

-You would first select the element you're going to style, in this example, it's an HTML header.

-You would then use the set of curly braces { } , and inside these curly braces would be the declarations, which take the form of property and value pairs. These property value pairs specify a property of elements, and the value we'd like to give the property.

-In the example above, before the colon we have the property (color)(font size), and after the colon we have the value (red)(5em). 

CSS style sheets can have the rules written one after the other. For example,

h1 {
    color: red;
    font-size: 5em;
}

p {
    color: black;
}

*(Mozilla and Individual Contributors, “What is CSS”, 2005-2021)*

### CSS Modules

The CSS language is divided up and broken down into modules. For example, you could view and analyze the [Backgrounds and Borders](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Backgrounds_and_Borders) module to find out what it does, how it functions and what varying properties and features it has. *(Mozilla and Individual Contributors, “What is CSS”, 2005-2021)*

### CSS Specifications

All web standard language code (HTML, CSS, JavaScript, etc) are told about in documents called specifications (or specs), which are published by organizations such as [W3C](https://developer.mozilla.org/en-US/docs/Glossary/W3C), [WHATWG](https://developer.mozilla.org/en-US/docs/Glossary/WHATWG), [ECMA](https://developer.mozilla.org/en-US/docs/Glossary/ECMA), or [Khronos](https://developer.mozilla.org/en-US/docs/Glossary/Khronos), and these organizations make certified statements on how these technologies are suppose to behave. CSS was developed by [CSS Working Group](https://www.w3.org/Style/CSS/), which is a group within the W3C. *(Mozilla and Individual Contributors, “What is CSS”, 2005-2021)*

### Browser Support Information

Once CSS has been specified, then it only enables us to make web pages if one or more browsers have done it. What this means is that the code has been written to convert the instruction in our CSS file into an item that can be displayed on the screen. *(Mozilla and Individual Contributors, “What is CSS”, 2005-2021)*

## How to Add CSS

If you wish to insert CSS, then there’s three different style sheet options that are available to you: 

-External CSS

-Internal CSS

-Inline CSS

*(Refsnes Data, “How to Add CSS”, 1999-2021)*

### External CSS

If you want to change the look of an entire website, you can do so, by changing just one file with an External Style Sheet. However, it is necessary for each HTML page to include a reference to the external style sheet file inside the < link > element, inside the head section. Below is an example of External styles, which are defined within the < link > element, inside the < head> section of an HTML page.

< !DOCTYPE html>

< html>

< head>

< link rel="stylesheet" href="mystyle.css">

< /head>

< body>

< h1>This is a heading< /h1>

< p>This is a paragraph.< /p>

< /body>

< /html>

An external style sheet has the ability to be written in any text editor, and must have a .css extension, when you save it. The external .css file should not contain any HTML tags.

*(Refsnes Data, “How to Add CSS”, 1999-2021)*

### Internal CSS

In the event that one single HTML page has a unique style, then an internal style sheet may be used. Inside the head section, within the     <  style > element,  is where the internal style is defined. 

< !DOCTYPE html>
< html>
< head>
< style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
} 
< /style>
< /head>
< body>

< h1>This is a heading</h1>
< p>This is a paragraph.</p>

< /body>
< /html>

*(Refsnes Data, “How to Add CSS”, 1999-2021)*

### Inline CSS

If you need to apply a unique style for a single element, then an Inline Style can be used. In order to use Inline Styles, put the style attribute to the relevant element. The style attribute has the ability to contain any CSS property.

< !DOCTYPE html>
< html>
< body>

< h1 style="color:blue;text-align:center;">This is a heading</h1>
< p style="color:red;">This is a paragraph.</p>

< /body>
< /html>

*(Refsnes Data, “How to Add CSS”, 1999-2021)*

### Multiple Style Sheets

In the event that some properties have been labeled for the same selector (element) in different style sheets, then the value from the last read style sheet will be used.

h1 {
  color: navy;
}

h1 {
  color: orange; 
  }

In the event that an internal style is labeled after the link to the external style sheet, then the < h1> elements will be orange
  
  < head>
< link rel="stylesheet" type="text/css" href="mystyle.css">
< style>
h1 {
  color: orange;
}
< /style>
< /head>  

However, in the event that the internal style is defined before the link to the external style sheet, then the < h1> elements will be navy

< head>
< style>
h1 {
  color: orange;
}
< /style>
< link rel="stylesheet" type="text/css" href="mystyle.css">
< /head>

*(Refsnes Data, “How to Add CSS”, 1999-2021)*

## CSS Color Property

The color property in CSS specifies the color of text. You should set the text color for different elements.

body {
  color: red;
}

h1 {
  color: #00ff00;
}

p.ex {
  color: rgb(0,0,255);
}

If you would like to look at a complete list of possible color values, then you can look at the [CSS Color Values](https://www.w3schools.com/cssref/css_colors_legal.asp).

An initial sets the property to its default value. If you would like to read more about an initial you can look at [Read about initial](https://www.w3schools.com/cssref/css_initial.asp)

An inherit inherits its property from its parent element. If you would like to read more about inherit, you can read about it at [Read about inherit](https://www.w3schools.com/cssref/css_inherit.asp).

*(Refsnes Data, “CSS Color Property”, 1999-2021)*

## CSS Reference

Below is a basic rules syntax for CSS:

style-rule ::=
    
    selectors-list {
      
      properties-list
    }
    
    ...where:
    
    selectors-list ::=
    
    selector[:pseudo-class] [::pseudo-element]
    
    [, selectors-list]

properties-list ::=
    
    [property : value] [; properties-list]
    
 
 If you would like an alphabetical index of all the standard CSS properties, you can click on [CSS Alphabetical Index](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference#index).

*(Mozilla and Individual Contributors, “CSS Reference”, 2005-2021)* 
 