# JS
## functions methods and objects ch3 p106-144

a keyword and object constructor create a blank object which you then add properties and methods to. using dot notation (this.property1;) the method is the action given to the object through a function, and the properties hold the values for the function. you can create an object using obect() or var varObject = {} using a function as a template you can create many objects that are similar constructor functions begin with a capital letter 

# HTML & CSS 
## Chapter 6: “Tables” (pp.126-145)
html tables contain rows<tr> 'table row' and cells<td> 'table data'. <th> for table headings. use colspan =# to tell a td or th how many columns it should run across. rowspan can be used on a row to tell th or td how many rows it should go down. section the tables with <thead> <tbody> <tfoot>. you can give each cell and row a boarder to clarify the table data, or previde whitespace

# code
keyWord object() 
     empty object 
this.property1;
     dot notation for property 
function Hotel(name, rooms, booked) {
this.name;
this.room;
this.booked;
this.check availability = function () {
     return this. rooms - this. booked;
};
