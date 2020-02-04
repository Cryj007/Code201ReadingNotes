# Read: 02 - HTML Text, CSS Introduction, and Basic JavaScript Instructions

## Chapter 2: “Text” (pp.40-61)

#### Notes

-tags are markups

-HTML has 6 headings

#### Vocab

- STRUCTURAL MARKUP= the elements that you can use to
describe both headings and paragraphs

- SEMANTIC MARKUP= which provides extra information; such
as where emphasis is placed in a sentence, that something
you have written is a quotation (and who said it), the
meaning of acronyms, and so on

- WHITE SPACE COLLAPSING= when browsers come across 2 or more spaces it will display it as 1

- EMPTY ELEMENTS= elements that do not  have any words between the opening or colsing tags

- VISUAL EDITORS= resemble word processors

- CODE VIEWS= shows you the code so you can edit it

## Chapter 10: Ch.10 “Introducing CSS” (pp.226-245)

#### Notes

-will make your web page more attractive

-imagine there is an invisible box around every HTML element

-helps create rules for every box

-unless specified, whatever rule is applied, it is applied to the whole page 

-always put CSS in a different file, so it looks clean.

#### Vocab

- SELECTORS= indicate which element the rule applies to

- DECLARATIONS= indicate how the elements referred to in the selector should be styled

- PROPERTIES= indicate the aspects of the elements you want to change 

- VALUES= specify the settings you want to use for the chosen properties

## Chapter 2: “Basic JavaScript Instructions” (pp.53-84)

#### Notes

-statements should end eith a semicolon

-be consistant with qoute marks

-gotta announce that a variable is being used

-booleans can only be yes/no

-booleans used when the vaue the code can have multiple paths

-consider using an array when working with a set of values that related to each other

-2 types of expressions
1. expressions that will just assign a value to a variable
2. expressions that will use two oe more values to return a single value

-6 rules to naming a variable:
1. Must not begin with a number only a letter, sollar sign, or underscore
2. cannot have a dash or a period
3. cannot use keywords
4. variables are sensitive. s is different than S
5. use a name that describes that info that the variable is storing
6. if more than two words capitalize the first letter of the second word. firstName

#### Code
*array literal is perfered
example

ARRAY LITERAL= 
var colors;
colors = ['white'.'black'.'custom'];

var el = document.getElementById('colors');
el.textContent = colors[0];

ARRAY CONSTUCTOR= 
var colors;
colors = new Array('white',
		   'black',
		   'custom');

var el = document.getElementById('colors');
el.textContent = colors[0];

#### Vocab

- STATEMENT= each individual step

- CODE BLOCKS= statements that re surrounded by curly braces

- MULTI-LINE COMMENT= a comment that stretches over more than one line /*

- SINGL-LINE COMMENT= anything that follows th eteo forward slash // on that line will no be processed by JS

- VAIABLES= a script that can temporarily store bits of info it needs to do its job

- KEYWORD= used to create a variable

- ASSIGNMENT OPERATOR=  equals sign(=) used to assign a value to a vairable and update the value given

- UNDEFINED= variable that has no value yet 

- NUMERIC DATA TYPE= handles numbers

- STRING DATA TYPE= consists of letters and other characters

- BOOLEAN DATA TYPE= can have one of the two values: true or false

- BACKWARDS SLASH= tells the interpreterr that the folloeing character is part of the string, rather than ending it

- ARRAY= stores a list of values

- INDEX= each item in an array automatically given a number

- EXPRESSION= evaluates into a single value

- OPERATORS= allow programmers to create a single value from one or more values

## Chapter 4: “Decisions and Loops” (pp.145-162)

#### Notes

-flow charts can help plan what lines of code should be next

-2 componenets to a decision
1. an experssion is evaluated, which returns a value
2. a condition statement says what to do in a given situation

-usually one operator and two operands in a condition

-operands can be values ior variables; on each side of the operator

-operand can be an expression, because each expression evaluates into a single value

-logical operators allows to compare the results of more than one comparison operator 

-If statement evaluates a conition, or checks it

-If...else statement checks a condition


#### Vocab

- COMPARISON OPERATORS= allow to compare values and test whether a condition is met or not

- IS EQUAL TO(==)= compares two values to see if they are the same

- IS NOT EQUAL TO(!=)= compares two values to see if they are not the same

- STRICT EQUAL TO(===)= compares two values to check that both the data type and value are the same

- STRICT NOT EQUAL TO(!==)= compares two values to check that both the data type and values are not the same

- GREATER THAN(>)= checks if the number on the left is greater than the number on the right 

- LESS THAN(<)= checks if the number on the left is less than the number on the right

- GREATER THAN OR EQUAL TO(>=)= checks if the number on the left is greater than or equal the number on the right

- LESS THAN OR EQUAL TO(<=)= checks if the number on the left is less than or equal to the number on the right

-LOGICAL AND(&&)= tests more than one condition ((2<5)&&(3>=2)) 

- LOGICAL OR(||)= tests at least one condition ((2<5)||(2<1))

- LOGICAL NOT(!)=takes a single boolean value and inverts it !(2<1) 
