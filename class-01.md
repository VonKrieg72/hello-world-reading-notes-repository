Code 201 reading notes

Class 01.md

HTML ch. 1

HTML stands for hyper text markup language and it provides a structural framework for your webpage. HTML structures your web pages through the use of elements. The elements are made up of an opening tag and a closing tag, and the stuff inside the opening and closing tags are called content. For example, an opening tag is made up of a less than and a greater than symbol with a character in between. The closing tag is made up of the same things with the exception of a forward slash included. Here is an example of a body tag.

< body > < /body >

In some instances, tags can have attributes within them as well. Attributes provide additional information about the contents of an element. For example, in the paragraph tag below you have attributes included in the tag.

< p lang=“eng-us” > Paragraph in English < /p > 

There is the opening and closing < p > < /p > and within the opening tag you have **lang=“eng-us,”** which means the paragraph within the tag is in American standard English. *(Duckett, Jon, HTML & CSS: design and build websites, pp. 25-26 2011.)*

When you are creating your page, you want to keep in mind that within your < html > < /html > tag you have the head element, the title element, and the body element. What ever content you see in the body element is what you are going to actually see on your page, and what ever you see in the title tags is what you are going to see in the tabs at the top of the page. 

< html >

< head >

< title > This is what you will see in the tab < /title >

< /head >

< body>
< h1 > < /h1 >
< p > < /p >

< /body >

< /html >


HTML ch. 8

When you are starting out your code for your HTML, you must always start it with a < !DOCTYPE html > declaration. What this declaration does is it tells the browser which version of HTML the page is using. In some instances you may want to add a comment to your HTML code, in order to make your code easier to understand, in the event you have to come back to your code after a long time, or if somebody else has to look at your code. *(Duckett, Jon, HTML & CSS: design and build websites, pp.181-182, 2011.)* You can add a comment with the following tag

< ! - -   - - >

Keep in mind that a comment tag will not display on your page. It will only be visible when the code is inspected. 

You can use the < div > < /div > element whenever you wish to put a set of elements together in a group. This feature may come in handy, in the event you wish to contain all the elements for the header of your site, contain the comments from visitors to your site, or contain the items located in the footer of your site. The span element < span > < /span >  does much the same thing as the division element, except it does it in an inline fashion. The use of < iframe > < /iframe > elements enables you to embed an interactive google map, or an HTML page. Make sure that you include attributes like the src, height and width. *(Duckett, Jon, HTML & CSS: design and build websites, pp. 181-189, 2011.)*


HTML ch. 17

In the new HTML5 layout, elements enable you divide up parts of a page. The names of these elements will determine what type content you’ll find in them. Older internet browsers are unable to figure out that the new HTML5 elements will automatically treat them as inline elements, because of this, if you are still using an older browser, it would be a good idea to include a line of CSS on the left, which lets the browser know which new elements should be rendered as block level elements. internet Explorer 9 was the first version of the browser, which allowed CSS rules with the new HTML5 layout elements. If you are using an older version of the Internet Explorer web browser, then it is going to be necessary for you to use a simple JavaScript, which is known as HTML5 shiv or HTML5 shim. If you do need to use it, then there is an available link from Google, which is hosted on its servers, which you can copy, and place it inside a conditional comment, which will verify if the browser version of Internet Explorer you are using is older than Internet Explorer 9. However, it is important to point out that if you are using a version of Internet Explorer, which is older than 9, then you have to have JavaScript enabled in your browser; otherwise, you will not have the ability to see the content of those HTML5 elements. *(Duckett, Jon, HTML & CSS: design and build websites, pp. 431, 432, 442, 2011.)* 


HTML ch. 18

In the process of designing your website, once you’ve figured out who your target audience is going to be, and what type of content you are going to have on your site, then it is time to start planning out your site map. A site map is like a diagram of pages that you will use to structure your website. *(Duckett, Jon, HTML & CSS: design and build websites, pp.461, 2011.)* A technique that is used to do this is called card sorting. You do this process by taking cards with information on them and then you sort them into related groups. In most cases, it would be a good idea to start out your site map with the home page, and then the corresponding pieces of information afterwards. The pages will help the users on how to correctly navigate through your website. Keep in mind that your final product should have its information organized towards the user’s understanding of things and not your (site designer) understanding of things. Once you’ve organized your site map, then you can start doing your wire frames. Wireframes are sketches of how the pages of your website are going to look, and what type of information and features are going to be displayed on them. Some developers use software to do their wireframes; however, you can also sketch out your wireframes by hand with either pen and paper or on a white board with a marker. If you choose to sketch your wireframe by hand, it will be easier to edit things and make corrections. The last thing you want to keep in mind with your site is the visual hierarchy. The visual hierarchy is the how you organize the sequence in which your eyes view what is on the screen. It’s important to design the visual hierarchy in such a way where it doesn’t come off as un-interesting, because nothing is standing out, or where too many aspects are trying to get your attention, which would make it hard for the user to focus on the key message of the site. *(Duckett, Jon, HTML & CSS: design and build websites, pp.461-464, 467-468 2011.)* 


JavaScript ch. 1

A script is a set of instructions, which your computer follows closely as a guide in order to accomplish a task that you command it to do. When writing out you JavaScript, it is best to write it in a separate file and then link it into your HTML document. For example, 

< !DOCTYPE html >
< html >
    < head >
	< title > Monthly earnings < /title >
	< link rel=“stylesheet” href= “css / c01.css” / >
   < /head >
   < body >
	< h1 > Common Wealth Realty < /h1 >
	< script src= “ js/add-content.js” > < /script >
	< p > Common Wealth Realty offers mortgages at low interest rates < /p >
   < /body >
</ html >

In the above example you can see that the JavaScript file is linked into the HTML file through the use of the < script > < /script > tags. Within the script tags you have the source of the JavaScript file, which enables the HTML document to read and implement what ever the JavaScript file says. In JavaScript you can also use objects and methods. The object in your JavaScript represents the entire web page. The method enables new information or material to be written into the page, where the script element sits. *(Duckett, Jon, 