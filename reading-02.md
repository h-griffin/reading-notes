02 march 2020

# HTML
## text ch2 p40-61
structural tags have meaning to the program with what to do with the information given, tags like <h1> and <p> are both given texts but appear on the page differently. white space collapsing makes it easier for the coder to read the code, when the browser comes across two or more spaces next to eachother it displays only one. the text inside of <em> may be audibly read different through screen readers so it is import to include those in the code. 

## introducing CSS ch10 p226-245
css associates style rules with html elements using selectors and a declaration. there selector is the html tag that you’re referring to and the declaration is telling it what to do with the information in that tag. you can select more than one tag and give it the same declaration for them to all appear the same. properties are the aspect of the element you want changed like text or color, while the value specifies the setting you want to use, such as the actual color. using inline styling uses css inside of the html tag using a style tag. there are different kinds of selectors and each is referred to differently. the children of elements with styling will inherit the parent style if not otherwise specified. 

#JS
## basic javascript instructions ch2 p53-84
a script is made of up statements, each statement is a line of code in the script of instructions, each statement ends in a semicolon. variables are continues that store information assigned to it and can be referred to later on in the code. javascript distinguishes between numbers, strings/text, and booleans which are true or false. arrays store a list of values and can be referred to as var itemThree. there are arithmatic operators that will use mathmatic order of operations to complete the problme. 

## decisions and loops ch4 145-162
decision making can respond with a different message depending on the true or false result. to determine if it is true or false, you must set a condition such as ia A greater than B, and if it is true or false it will send a message. 

# code
var itemThree;
itemThree = colors[2];

#### javascript falsey
false, 0, empty string.

#### javascript truthy
true, nubers besides 0, a string with length. ampty object/array
if a string that says false it will be true. different data type.

#### data type
string, number, boolean, null(reason), undefined(mistake)

## switch

switch(name){
    case 'jacob':
        alert('hey jaocb');
        break;
    case 'alistair':
        alert('hello alistair');
        break;
    default:
        name = prompt('who are you?')
}

switch, check one thing -case
if, more than one thing -else if