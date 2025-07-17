//Javascriptprojects
//My Javascript Learnings

//creating an object with properties and their values (Syntax literals and dot Notation)
var assistantManager = {
    rangeTilesPerTurn: 3,
    socialSkills: 30,
    streetSmarts: 30,
    health: 40,
    specialAbility: "young and ambitious",
    greeting: "Let's make some money"
}

/*An alternative approach of building objects is to first save an empty object literal to a variable, then use the dot notation to declare new properties on the fly, and use the assignment operator to add values to those properties; for example:  */

var house2 = {};
house2.rooms = 4;
house2.color = "pink";
house2.priceUSD = 12345;

/*
Object literals and the brackets notation
There is an alternative syntax to the dot notation I used up until this point.

This alternative syntax is known as the brackets notation.

To understand how it works, it's best to use an example, so I'll go through the process of coding the house2 object again, in the same way that I did with the dot notation, only this time, I'll use the brackets notation */


var house2 = {};
house2["rooms"] = 4;
house2['color']= "pink";
house2["priceUSD"] = 12345;
console.log(house2); // {rooms: 4, color: 'pink', priceUSD: 12345}


/*
I can both access and update properties on objects using either the dot notation, or the brackets notation, or a combination of both, like in the following example:
*/

var car = {};
car.color = "red";
car["color"] = "green";
car["speed"] = 200;
car.speed = 100;
console.log(car); // {color: "green", speed: 100}

/*
Finally, there's one really useful thing that bracket notation has but is not available in the dot notation: It can evaluate expressions.

To understand what that means, consider the following example:
*/


var arrOfKeys = ['speed', 'altitude', 'color'];
var drone = {
    speed: 100,
    altitude: 200,
    color: "red"
}
for (var i = 0; i < arrOfKeys.length; i++) {
    console.log(drone[arrOfKeys[i]])
}
/* Results
100
200
red
*/
