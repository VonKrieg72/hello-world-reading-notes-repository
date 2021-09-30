# HTML Text, CSS Introductions, and Basic JavaScript Instructions


## HTML

HTML stands for hyper text markup language, and it is a language that consists of tags, which are known as markup. There are two main markups that you can utilize to help you structure your web page, when you create it. They are **structural markup,** which consists of elements such as *headings* and *paragraphs*, and **semantic markup,** which enables you to display additional information, such as bold and italics text, which brings attention to certain words and sentences, as well as things like quotes and abbreviations. 

In HTML structural markup, there are six different types of headings that you can utilize when designing your web page. These six headings consist of a letter **h** inside of  <    >    and a number (1-6), with < h1 > being the biggest heading, < h6 > being the smallest heading, and corresponding sub-headings of < h2 > through < h5 > in between. For example, If you were designing a web page and the main heading of your web page was…….. **Understanding HTML**, you would write it in your HTML like this……..


< h1 > Understanding HTML < /h1 >

And it would display on your web page like

# Understanding HTML

If you had the sub-headings under it, which were titled < h2 > HTML Structural Markup < /h2 > and < h3 > HTML Semantic Markup < /h2 > they would appear on your web page like…….

## HTML Structural Markup

And 

## HTML Semantic Markup

If you wanted to write a paragraph on your web page, you would utilize the < p > < /p > tags, and you would write your paragraph in between the two tags. For example, the paragraph…….

< p > HTML is one of the main three languages that you will utilize in web page design. It is very important that you master all of the features. < /p >

This sentence would display on your web page as……

HTML is one of the main three languages that you will utilize in web page design. It is very important that you master all of the features. 

In HTML semantic markup you can utilize tags like < strong > < /strong > which will put a word in bold print. For example, if you wrote the sentence……..

The capital of North Dakota is < strong > Bismarck. < /strong >

That sentence would display on your webpage as 

The capital of North Dakota is **Bismarck.**

By the way, the tags < strong > and < b > pretty much do the same thing as they both put the content within them in bold print. Similarly the tags < em > and < i > both put the content within them in italics. 


## CSS

CSS stands for Cascading Style Sheets, and it is a language used to add style to an HTML document, such as the background color of a webpage, the background color of a header,  and the color of the letters in a paragraph. It is able to do this by treating each HTML element as if it resides in it’s own independent box, which can be affected by CSS styling commands. The CSS language affects each HTML element through what are known as selectors and declarations. The selector lets you know which HTML element the style will apply to or directly affect. The Declaration lets you know how the element that is being affected will be styled. Within the declaration there are properties, which lets you know the aspects of the element that you want to affect, such as color, font, width, height, and border, and the values will let you know the specific color that the declaration will be. 

When creating your CSS styles, you have the option of using either an internal CSS or an external CSS. If you use an internal CSS, you can place it within a < style > < /style > tag and place it in the < head > element.  For example, it you wanted to make the background of your body blue, you would write it as …..

body {

background: blue; 

}

You also have the option to create an external CSS file and link it to your HTML. In order to this you would create a link element and put it in your < head >  < /head > tag. 


## JavaScript

JavaScript is a script, which contains specific instructions, which in many cases enables the user to interact with your webpage, when they visit it. One main way that JavaScript does this is through the use of variables. 

