# READ-06
# article
in the article about problem solving the author writes that teaching the same simple progrsm over and over, provides an easy fall back and farmiliar program and problem set to use to implament new technology. haivng the sae simple task to program that can be used with different technologies that can me taught through something farmilliar. using the farmiliar project it makes the new material less daunting because the objective is known. 

# Chapter 3: “Object Literals” (pp.100-105)
objects group together a set of variables and funtions. inside an object, variables become properties and functions become methods. the name of variables and functions are called keys while inside of an object. an object cannot have two keys of the same name. the value of a property can be any data type, but the value of a method is only a function. creating an object in literal notation means the object is stored in a variable and its contents live in the following braces. inside of an object you can use the 'this' keyword to refer to this inside of 'this' object. you can acces things inside of an object youing dot notation by giving the name followed by . property/method name. the . is called a member operator: the property or method to the right is a member of the object on the left. you can also access things inside properties by using square bracket syntax. 

# Chapter 5: “Document Object Model” (pp.183-242)
the DOM is not Javescript or HMTL it has its own set of rules, it makes a model of the HTML page and accesses and changes the htmlk page. the dom is often reffered to as an API application programming interface, which lets humans interact with the programs. 

# code
### object 

var hotel = {
    name:'quay',
    rooms: 40,
    booked: 25,
    gym: true, 
    roomTypes: ['twin', 'double', suite'],

    checkAvailability: function(){
        return this.rooms - this.booked;
    }
};

### dot notation
var hotelName = hotel.name;
var roomsFree = hotel.checkAvailability();

### square bracket syntax
var hotelName = hotel['name'];
var roomsFree = hotel['checkAvailability'];

use for:
- name of property contains special character like dash
- name of property is a number (avoid)
- variable being used in place of property name