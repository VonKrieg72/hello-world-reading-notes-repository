## HTML lists

As you are completing tasks with code, there may be some occasions, where you need to use a list to enumerate items. Within HTML there are three different types of lists; **ordered lists, unordered lists, and definition lists.** You would use an **ordered list** when you are creating a list, where it would be necessary for list items to be numbered. You would use an ordered list when the items you are listing have to be done in a certain order or sequence, or when you are listing items in a contract, where each item has to be sectioned off by a number. In order to make an ordered list you have to use the…….

< ol > < /ol > tag and you have to place each list item within the ordered list in between < li > < /li > (list item) tags. For example,

In order to make a pizza from scratch you must do the following steps……

< ol >
      < li > pour flour into a bowl and add yeast and water and allow it to sit for 2 hours < /li >
      < li > after 2 hours the dough should rise and you should be able to start flattening the dough into a pizza < /li >
      < li > after the dough is flattened throw it into an oven which has been pre-heated to 425 degrees < /li >
      < li > cook the dough at 425 degrees for 8 - 10 minutes < / li >
      < li > take the cooked pizza dough out of the oven and start adding your toppings to the pizza < /li >
      < li > start with a layer of tomato sauce, then a layer of cheese, then whatever toppings you choose after that < /li >
      < li > after you have added all of your toppings throw the pizza back in the oven (still at 425 degrees) and bake for another 8-10 minutes < /li >
      < li > after this take the pizza out of the oven and allow it to cool for about 5 minutes < /li >
      < li > slice up your pizza and enjoy < / li >
< /ol >

On an HTML document the above list would have a number from 1-9 before each list item, putting them in a sequence or order. 

If you wish to create a list where is not necessary or important to enumerate items in a particular order or sequence, you would use an unordered list. An unordered list follows the same format as an ordered list except you use a < ul > < /ul > tag. For example, if you were just simply listing items on a shopping list.

< ul >
     < li > peaches < /li >
     < li > watermelon < /li >
     < li > cantaloupe < /li >
     < li > brussels sprouts < /li >
     < li > cauliflower < /li>
     < li > broccoli < /li>
     < li > kale < /li >
     < li > chicken < /li >
     < li > steak < /li >
     < li > salmon < /li >
     < li > tuna steak < /li >

If you wish to define a word with multiple definitions, like you would see in a dictionary, then you would use the < dl > < /dl > tag, which is the definition list . Nested within the < dl > < /dl> tag would be the < dt > < /dt > tags which stands for definition term, and the < dd > < /dd > tag would be the last tag which contains the actual definition. 

< dl >
     < dt > enumerate < /dt >
     < dd > to ascertain the number of: count < /dd >
     < dd > to specify one after another : list < /dd >

     < dt > computer < /dt >
     < dd > specifically: a programmable usually electronic device that can store, retrieve, and process data. < /dd >
< /dl >

Nested lists are the items that are indented under the main list item. For example, < li > < / li > , < dt > < /dt > , and < dd > < /dd > are nested list items. *(Duckett, Jon, HTML & CSS: design and build websites, pp. 62-73 2011.)*

## Boxes 

Boxes in HTML come in default sizes that are just big enough to hold the contents within it. In order to set your own box sizes you can use the height and weight properties in CSS. The three most commonly used ways to set the size of boxes are pixels, percentages and ems. Using pixels to adjust the size of your box is the most accurate way to do it; however,  if you adjust the size of the box using percentages, the size is relative to the size of the browser window, and if you use ems, the size of the box is based on the size of the text inside the box. The border, margin, and padding of each box is also adjustable with CSS. The border of each box separates the edges of one box to another, the margin. The margin is on the outside of the edge of the border. The width of the margin can be set, in order to create a gap, between the borders of two boxes which are adjacent to each other. The space between the border of the box and the space within it is called the padding, and if you add the padding in your box, it can increase the readability of its contents. With CSS, there is a visibility property, which enables you to hide boxes from users, which will leave a space where the hidden box was. The visibility property has two settings: hidden and visible. The border image property puts an image to the border of any box. The box shadow property enables you to add a drop shadow around a box. Box shadows has three values: horizontal offset, vertical offset, blur distance, and spread of shadow. *(Duckett, Jon, HTML & CSS: design and build websites, pp. 301-320 2011.)*


## Basic JavaScript Instructions

An array is a special variable that is able to store more than one value. One of the most useful features of an array is when you have to create a list, and you don’t know how many items are going to be on it, so rather than just creating enough variables for a long list, you can just create that list, and add to it as you go. When you create an array, you do so just like a regular variable, by using the **var** keyword and the name of the array after it. In an array you use square brackets, and each list item is separated by a comma. This is the preferred way of creating an array and it is called an **array literal.** The other way to create an array is called an **array constructor.** If you create an array using this method, you use the keyword **new** followed by **array** and then you use regular parenthesis, to put the values in, which are separated by commas. Each item within an array is given a number , which is known as an index,  and the numbered items always start at zero. Arrays also have a property called length and this holds the number of items in an array. *(Duckett, Jon, JavaScript & JQuery: Interactive front end web development, pp.14, 49, 2014.)* 


## Decisions and Loops

An **if…else statement** performs the task of checking a condition. If the condition is resolved to true, then the first code block is executed, and if the condition is resolved to false, then the second code block is run. For example, 

Var pass = 70;
Var score = 90;
Var msg;

If (score >= pass) {
msg= “Great Job, You passed!” ;
} else {
msg= “Sorry, you did not pass. Take the test again” ;
}

Var el= document.getElementbyId(“answer”);
el.textContent = msg;

As you can see from the if…else statement above, the variables are assigning a value, and the if…else statement is set to give you two possible outcomes: if the **if statement** turns out to be true, then it will stop there and return the message to the user “Great Job, You passed.” However, if the it doesn’t turn out to be true then it will go onto the **else statement,** which will return a message to the user as “Sorry, you did not pass. Take the test again.”

Whenever you use a **Switch Statement,** you begin it with a variable, which is known as the *switch value.* Each case will let you know a possible value for this variable and the code that’s suppose to run, if the variable is a match for that value. 

Switch (level) {
Case 1: 
	msg = ‘Good luck on the first test’
	break;

Case 2:
	msg = ‘Second of three - keep going!’ ;
	break;

Case3:
	msg = ‘Final round, almost there!’ ;
	break;

Default;
	msg = ‘Good luck!’ ;
	break;

From the example above, you can see that the purpose of the switch statement is to show the user with a different message, which will depend on the level they are at, and the message is stored in a variable called **msg.** *(Duckett, Jon, JavaScript & JQuery: Interactive front end web development, pp.164, 165, 2014.)* 

JavaScript uses weak typing, which means that the data type for a value can change. Programs that use strong typing will require you to specify what data type each variable will be. **Type coercion is when JavaScript is able to convert data types behind the scenes, in order to complete an operation. Type coercion has the possibility of leading to values that are unexpected within your code, which is why it is a good idea when checking it two values are equal, it would be a good idea to use strict equal operators = = = and ! = = as opposed to = = and ! = because the strict equal operators are able to check that the value and data types match. Because of **type coercion** every vale in JavaScript has the ability to be treated as if it were true or false. If a value is **falsy** it is treated like it is false. If a value is **truthy** then its value is treated like it it true. Pretty much every value that is not false can be treated like it is true, with a few exceptions. 

There are three loops in JavaScript the for loop, while loop and do while loop. You use a loop whenever you want to check a condition. If the condition returns true it will run again and again in a loop until it returns false, then it will stop. You use a for loop if you need to run code a specified number of times. The condition in most cases is a counter, which tells how many times the loop should run. A while loop should be used if you’re not aware of how many times the code should run. In a while loop the condition can be something other than the counter, and the code continues to loop as long as the condition is true. The do while loop will always run the statements inside the curly braces at least once, even if the the condition is false. *(Duckett, Jon, JavaScript & JQuery: Interactive front end web development, pp.162-170, 2014.)* 

 

