# JS Object Literals; The DOM


## Understanding the problem domain

Most developers think that writing code can get quite difficult at times, and attribute it to factors such as: learning a new technology, naming things, testing their code, debugging, fixing bugs, or making software maintainable; however, the thing that most developers never even consider is the **problem domain.** John Sonmez described the problem domain as trying to find a solution without knowing what the problem is in the big picture, or trying to find an answer, without knowing what the question is. He is directly quoted as saying “The big issue is that many problem domains are like a puzzle with a blurry picture or no picture at all.” Sonmez says that understanding the problem domain will make writing code a lot easier; however, if you are in a situation where you don’t have all the information that you need before you start writing code, you have two options: Make the problem domain easier or Get better at understanding the problem domain. If you choose the option of making the problem domain easier, it’s basically breaking a bigger problem down into smaller steps and moving on, because Sonmez said that “it is often beneficial to take a part of the problem and fully understand that part before expanding the problem domain.” He used the example of playing a video game, and starting at an easy level and then eventually moving on to more complex levels, and using the upgrades that you gained from previous easier levels, to work your way through the entire game. If you choose to get better at understanding the problem domain, you have to realize that sometimes it is better to gather up as much information as possible, before you start to code. You can do this by taking the time to sit down and talk to customers or business people, which will help you gain a better understanding of the problem domain and help you know it inside out, as opposed to just starting the project, without having a full understanding of the problem domain, and end up having to do things over again, which ends up being more expensive and more of a waste of time in the long run. *(Sonmez, John “Understanding The Problem Domain Is The Hardest Part Of Programming”, 2013July15)*  


## What’s the difference between primitive values and object references

Within JavaScript there are eight data types: boolean, null, undefined, number, BigInt, string, symbol, and objects. The first seven are known as primitive types and the last is an object. In JavaScript the primitive type values and object references are stored differently. Whenever a primitive value is assigned to a variable, it is set directly to that value. Whenever a variable is assigned to an object, the variable contains a reference to it, and stores it in the compute memory, as opposed to being assigned that value. It doesn’t contain the new object but rather the reference to the memory address that currently stores that object. Within JavaScript there is something called mutability, and this relates to whether or not a value can be changed. Primitive values are immutable, which means they cannot be changed and object references are mutable and can be changed. Javascript programs will use in many cases equality operators to check if two values are the same. In order to do this, the == is used to check Loose equality, and the === is used to check strict equality *( Geelhoed, Chris, “What’s the difference between primitive values and object references in JavaScript”, 2020January16)*

## Object Literals

Within JavaScript an object groups together a set of variables and functions in order to create a recognizable model of something from the real world. Variables that are a part of an object are called property. They tell you things about the object, like names and numbers that give the user information about a property. Functions that are a part of an object are called a method. a method shows things that need to be done or tasks that are associated with the object that it is a part of. For example, you may need to use a method if you are trying to figure out how much money a bank has available, by subtraction the amount of expenses from the current money stock. A key is a name and a value that like variables, named functions, properties and methods that are a part of an object have. In order to create an object you would use literal notation, which is the most common and easiest way to do so. Objects are created with a name and curly brackets. For example:

Var farm = {

Name: West Farm

Barms: 3

Animals: 60

checkProductions: functions() {

Bring animals to market - this Saturday;

}

};


The other method in which to create an object is called object literals, which is pretty much using the same template as literal notation, but the values of the object’s properties will be different. 


*(Duckett, Jon, JavaScript & JQuery: Interactive front end web development, pp.100-105, 2014.)* 

