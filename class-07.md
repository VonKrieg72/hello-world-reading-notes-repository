Read 07 - HTML Tables; JS Constructor Functions

# Object-Oriented Programming, HTML Tables


## Domain Modeling

Within code, there may be situations where you have to create a model for a specific project that describes various entities, their attributes and behaviors. Along with this, the model would also have to describe the constraints that govern the problem domain. One such modeling that you can use in code for a specific project is called **Domain Modeling,** which is the process of creating a conceptual model in code for a specific problem. Another model that you can use in code would be the **Object Oriented Model,** which is a model that stores data in properties and encapsulates behaviors in methods. *(Sobol, Ryan, Hamm, Samm, Hansen, Keil, “Domain Modeling”. 2018 February 03)* If you construct your domain model well, you will be able to verify and validate the understanding of a specific problem among various stake holders. When used as a communication tool, it has the ability to define vocabulary that can be used within and between business and technical teams. The best way to describe how this model works is through example. If you were on a team, and you were given the job of building a program model that shows the popularity of **funny cat videos**, after you’ve completed your research, you determined that there are two essential metrics for measuring the popularity, which are  **many likes** and **whether or not the videos has dogs** in them as well. 

var FunnyCatVideos = function(manyLikes, hasDogs) {
	this.funnyCatVideo = manyLikes;
	this. hasDogs = hasDogs;
}

var parkourFail = new FunnyCatVideos(9, false);
var corgiFail = new FunnyCatVideo(6, true);

console.log(parkourFail);
console.log(corgiFail);

*(Sobol, Ryan, Hamm, Samm, Hansen, Keil, “Domain Modeling”. 2018 February 03)*


## Tables

Within HTML a table is used to represent information with the use of a grid. Using a grid enables you to understand difficult data by referencing information on two axes. Whenever you want to create a table, you can do so by using the < table > < /table > tag. The children of the table tag are < tr > < /tr > and < td > < /td > tags. The < tr > < /tr > tag stands for table row, and you would use this tag to indicate the start of each row. The < td > < /td > tag stands for table data, and it is used to represent each each cell. The table row and table data tags are used very similarly to the ordered and un-ordered list tags with the list item tags under them. If you wish to represent the heading for either a column or a row, you can use the < th > < /th > tag. Along with these tags used in tables, there are three additional tags that you can use to help you distinguish between the main content of the table and the first and last rows. These tags are the < thead > < /thead > , < tbody > < /tbody >, and < tfooot > < /tfoot > tags. The thead tag is used for the headings of the table to sit inside of. The tbody tag is used for the body of the table to sit inside of, and the tfoot tag is used as the footer of the entire table. *(Duckett, Jon, HTML & CSS: design and build websites, pp. 131-135 2011.)*


## Functions, Methods, and Objects

In the event that you wish to create a new object, you can do so using the *new* keyword followed by *object.* This creates a blank object, which you can add properties and methods to. You are also able to use this syntax to add properties and methods to any object that you have created. 

var stadium = new Object( );

In the even that you wish to update an object, you can do so by using dot notation or square brackets. These work on objects already created by using the literal or constructor notation. In order to delete a property, you would use the delete keyword. 

stadium . name = ‘Yankee’ ;

stadium [’name’] = ‘Yankee’;

You are also able to use object constructors, which use functions as a template for creating objects. You would do this by creating the template with the object’s properties and methods. This method would be used if you wanted several objects to represent similar things.

function Stadium (name, seats, booked)

this.name = name;
this.seats = seats;
this.booked = booked;

this.orderTickets = function ( ) {
return this.seats - this.booked;
};


*(Duckett, Jon, JavaScript & JQuery: Interactive front end web development, pp.106-144, 2014.)* 


