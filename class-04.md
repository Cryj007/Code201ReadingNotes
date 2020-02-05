# Chapter 4: Ch.4 “Links” (pp.74-93)

#### Notes

-links are created using th <a> element
-to specify the link use href
-first part is the link, right after is the name that will show up on the webpage
-family trees describe the relationship between files and folders on a website
-emails can be made the same way as links
-can use the id element to taget and locate a specific location that is being linked to



 #### Vocab

- ABSOLUTE URL= the value of a href, to a different website, will be the web address for the site

- RELATIVE URL= linking pages within the same site

- ROOT FOLDER= top-level folder



# Chapter 15: “Layout” (pp.358-404)

####Notes

-HTML is its own box according to CSS
-becareful with floats, gotta individually move all floats
-move one float, it moves the whole page

float solution
 	-The overflow property is given a value auto.
	-The width property is set to 100%.
-mobile phones and tablets have higher resolution than computers, so the page on screen is smaller

Advantages of fixed layouts
	-Pixel values are accurate at controlling size and positioning of elements.
	-The designer has far greater control over the appearance and position of items on the page than with liquid layouts.
	-You can control the lengths of lines of text regardless of the size of the user's window.
	-The size of an image will always remain the same relative to the rest of the page.

Disadvantages of fixed layouts
	-You can end up with big gaps around the edge of a page.
	-If the user's screen is a much higher resolution than the designer's screen, the page can look smaller and text can be harder to read.
	-If a user increases font sizes, text might not fit into the allotted spaces.
	-The design works best on devices that have a site or resolution similar to that of desktop or laptop computers.
	-The page will often take up more vertical space than a liquid layout with the same content.
-pages usually 960-1000 px wide

Liquid Layout Advantage
	-Pages expand to fill the entire browser window so there are no spaces around the page on a large screen.
	-If the user has a small window, the page can contract to fit it without the user having to scroll to the side.
	-The design is tolerant of users setting font sizes larger than the designer intended (because the page can stretch).

Liquid Layout Disadvantages
	-If you do not control the width of sections of the page then the design can look very different than you intended, with unexpected gaps around certain elements or items squashed together.
	-If the user has a wide window, lines of text can become very long, which makes them harder to read.
	-If the user has a very narrow window, words may be squashed and you can end up with few words on each line.
	-If a fixed width item (such as an image) is in a box that is too small to hold it (because the user has made the window smaller) the image can overflow over the text.

Layout Grids
	-Creates a continuity between different pages which may use different designs
	-Helps users predict where to find information on various pages
	-Makes it easier to add new content to the site in a consistent way
	-Helps people collaborate on the design of a site in a consistent way

CSS Framework Advantages
	-They save you from repeatedly writing code for the same tasks.
	-They will have been tested across different browser versions (which helps avoid browser bugs).

CSS Framework Disadvantages
	-They often require that you use class names in your HTML code that only control the presentation of the page (rather than describe its content).
	-In order to satisfy a wide variety of needs, they often contain more code than you need for your particular web page (commonly referred to as code “bloat”).

#### Vocab

- BLOCK-LEVEL ELEMENTS= start on a new line 

- INLINE ELEMENTS= flow in between surrounding text 

- PARENT ELEMENT= outer box of a block-level box inside a block-level box

- 960 PIXEL GRID= a set of thick vertical lines superimposed, and designed according to a grid


# Chapter 3 (first part): “Functions, Methods, and Objects” (pp.86-99 ONLY)

#### Notes
-used to organize code
- once declaring thr function is done, you can bring it up again only typing thr function name
ex. sayHello();
-functions store instructions
-expressions produce value

when to use anonymous functions and iffes
	-as an arguement is being called
	-to assign the value of a property to an object
	-if handlers and listeners to perfrom a task when an event occurs
	-to prevent conflicts between two scripts that might use the same variable names
when local variables are made then removed when the function has done its part
	-if the function runs twice, the variable can have different values each time
	-two different functions can use variables with the same name without any kind of naming conflict

#### Code

function sayHello() {
	document.write('Hello!');
}

#### Vocab

- FUNCTIONS= group a series of statements together to perform a specific task

- PARAMETERS= pieces of info passed to a function 

- CALLING= asking a function to perform its task

- RETURN VALUE= writing a function and expecting it to provide you with an answer

- FUNCTIONN DECLARATION= giving a name to a function the writing statements needed to achieve its task inside the curly brackets

- STATEMENTS= perform the task that sit in a code block

- ARGUEMENTS= calling a function that has peremeters, to specify the values it should use in the parentheses that follow its name

- FUNCTION DECLARATION= creates a function that can call later in your code

- NAMED FUNCTIONS= name of the function

- FUNCTION EXPRESSION= putting a function where you expect to see an expression and is treates as an expression

- ANONYMOUS FUNCTION= a function with no name

- FINAL PARENTHESES= after the closing curly brace of the code block and tell the interpreter to call the function immediately

- GROUPING OPERATORS= parentheses to ensure the interpreter treats this as an expression

- FUNCTION-LEVEL VARIABLE= a variable created inside a function using var keyward, only used in that function

- SCOPE= if a variable is declared within a function, it can only be used within that function

- GLOBAL VARIABLE= creating a variable outside a function then used anywhere within the script 


# Article: “6 Reasons for Pair Programming”

#### Notes

-driver is the programmer who is doing the work (the body)
-navigator guides the programmer but doesn't put anything into the computer (the brain)
-Pair programming touches on all four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves

1. GREATER EFFICIENCY
-better to work with others, its faster
-makes the workspace more enjoyable
-communication gets better
-skills improve

2. ENGAGED COLLABORATION
-programming with someone else is more engaging
-working with someone else allows the programmers to be more focused
-if stuck on a problem for 15 minutes ask for help
-a confidence booster 

3. LEARNING FROM FELLOW STUDENTS
-new techniques to problem solving
-programmers who are more experienced can fully understand their own work
-programmers who are less experienced benefit gaining knowledge 

4. SOCIAL skills
-communication is key
-pair programming helps develop interpersonal skills
-has long-term career impacts
-people will hire those who can work well with others
