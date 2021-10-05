Class 04 

# HTML Links, JS Functions, and Intro to CSS Layout


## Links

If you want to create a link, you do so using the **< a > < /a >** tag. In the opening < a > tag, make sure you add an **href** attribute within it, followed by the actual web address. In between both the opening and the closing **< a > < /a >** tag you have the IMDB, which is what the web user actually sees and clicks on to visit the website you are trying to direct them to. For example:

**< a  href=“http://www.website.com” > IMDB < /a >**

The href attribute within the **< a >** tag is the actual web page that you want the users to go to, when they click the IMDB. When ever you link the user to a different website, the value of the href attribute will be the full URL web address. This is known as the **absolute URL.** Whenever you link a page within the same website you would use a **relative URL.** So, instead of typing out the full web address after the href attribute, if all the pages within the website are in the same folder, the you just type the name of the file. This is very useful to your website, and for the user, because it enables you to create links between pages without having to set up your domain name or hosting.  *(Duckett, Jon, HTML & CSS: design and build websites, pp. 79-80 2011.)*

**< a href=“pagetwo.html” > web site section < /a>**

In the event that you want to create a link that starts up the user’s email program and addresses you would still use the **< a > < /a >** tags; however, you would change what the value of the **href** attribute is. In this case the value of the **href** would be **mail to** followed by the **email address** that you would like to have the email sent to. For example

**< a href=“mail to: billsmith@website.com” > contact me < /a >**

In order to to create links that bring the user to different sections of the same page, you would use the **id** attribute within the **< h1 > < /h1 >** tags. The **id** attribute will identify those section of the page. 

**< h1 id=“middleofpage” > < /h1 > 


*(Duckett, Jon, HTML & CSS: design and build websites, pp. 85-88 2011.)*


## Layout

When one block level element sits inside of another one, then the outer box is called the containing or parent element. Commonly, these block level elements are grouped together within a **< div >** element.  The default way in which web browsers treat and display HTML elements is called **Normal Flow,** which puts your webpage in a static position. In this layout, each block level element is placed on top of the next one. If you use **Relative Positioning,** you are able to move elements in relation to where they would be in a normal flow. For example, you are able to move block level elements 5 pixels lower and 15 percent to the left, as opposed to what it would be in a normal flow. In **Absolute Positioning** the box is taken out, and because of this, it no longer has any affect on the position of the other elements on the page.  In **Fixed Positioning** the value of the positioning property has to be fixed. So, it is kind of like a type of absolute positioning. In the event that you use the **Float Element** you are able to take an element in normal flow, and place it to either the right or left side as far as you’d like. If you use **Fixed Width Layouts**, you have much more control over the appearance and position of items on the page, as opposed to liquid layouts; however, you can end up with big gaps around the edges of the page. If you use **Liquid Layouts** your pages will expand to fill the entire browser window, so that there are no spaces around the page; however, if you don’t have control over the width of sections of the page, then the design has the possibility of looking much more different than you intended, with unexpected gaps around certain elements, or items can appear squashed together as well. 

Being that most users will be able to see web pages that are 960-1000 pixels wide, web designers will mostly try to create web pages at that size. On some websites, you are able to see a set of thick vertical lines, which are super imposed over the top of a website to show you how the page was designed according to a grid. This grid is known as the **960 pixel grid,** which is widely used by web designers. With these grids the web designer is able to set consistently proportions and spaces between items. This helps in creating a very professional design look. **CSS Frameworks** provide you with the code for common tasks, which enable you to create grid layouts, style forms, and create printer friendly versions of pages. CSS Frameworks save you time by not making it necessary to write code for the same tasks.*(Duckett, Jon, HTML & CSS: design and build websites, pp. 362-391 2011.)*


## Functions, Methods and Objects

In JavaScript, functions are what enable you as a web designer to group a series of statements together, in order to perform a specific task. In order to create a function, you do so by giving it a name, then you write the statements needed to achieve its task inside the curly braces. This is called declaring a function. Once you declare a function, you are able to call or invoke that function by just writing the function and the parenthesis, without having to write all the stuff in the curly braces that follow. Calling a function enables you to execute all of the statements between the curly braces, with just one line of code. In the event that you need to declare a function with specific information to perform a certain task, you have to give it parameters. The parameters within the functions act like variables. When ever you want to get a single value out of a function, you set them up to perform a calculation and return a result. If you want a function to return more than one or multiple values, you would do so, by using an array. For example:

Function getDistance (feet, meters, miles, kilometers) {
var area = distance * time;
var volume = distance * time * speed;
var size = [value,  etc]; 
Return sizes; 
}

