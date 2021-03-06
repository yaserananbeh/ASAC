# This is my Reading summarize about this topic Programming with JavaScript Read 04a

### Introduction about javascript
#### how is the javascript make our website our interactive
   ###### ACCESS CONTENT
    You can use JavaScript to select any
    element, attribute, or text from an
    HTML page. For example:
    • Select the text inside all of the <hl>
    elements on a page
    • Select any elements that have a
    c1ass attribute with a value of note
    • Find out what was entered into a
    text input whose id attribute has a
    value of emai1 

###### MODIFY CONTENT
    You can use JavaScript to add
    elements, attributes, and text to the
    page, or remove them. For example:
    • Add a paragraph of text after the
    first <hl> element
    • Change the value of c 1 ass
    attributes to trigger new CSS rules
    for those elements
    • Change the size or position of an
    <img> element 

###### PROGRAM RULES
    You can specify a set of steps for
    the browser to follow (like a recipe),
    which allows it to access or change the
    content of a page. For example:
    • A gallery script could check which
    image a user clicked on and display
    a larger version of that image.
    • A mortgage calculator could collect
    values from a form, perform a
    ca lculation, and display repayments.
    • An animation could check the
    dimensions of the browser window
    and move an image to the bottom
    of the viewable area (also known as
    the viewport)

##### REACT TO EVENTS
    You can specify that a script should run
    when a specific event has occurred. For
    example, it could be run when:
    • A button is pressed
    • A link is clicked (or tapped) on
    • A cursor hovers over an element
    • Information is added to a form
    • An interval of time has passed
    • A web page has finished loading   


##### here some Examples of javascript 
    SLIDESHOWS
    FORMS
    RELOAD PART OF PAGE 
    FILTERING DATA



#### Define some main concept 
##### What is the script 
    A script is a series of instructions that a
    computer can follow to achieve a goal.
    You could compare scripts to any of the following : RECIPES / HANDBOOKS / MANUALS
###### how to write it
    To write a script, you need to first
    state your goal and then list the
    tasks that need to be completed in
    order to achieve it. 
    Start with the big picture of what
    you want to achieve, and break
    
    **Follow these steps**
    1: DEFINE THE GOAL
        First, you need to define the task you want to
        achieve. You can think of this as a puzzle for the
        computer to solve.
    2: DESIGN THE SCRIPT
        To design a script you split the goal out into a series
        of tasks that are going to be involved in solving this
        puzzle. This can be represented using a flowchart.
        You can then write down individual steps that the
        computer needs to perform in order to complete
        each individual task (and any information it needs to
        perform the task), rather like writing a recipe that it
        can follow.
    3: CODE EACH STEP
        Each of the steps needs to be written in a
        programming language that the compu ter
        understands. In our case, this is JavaScript.
#### To design it 
        every task should be broken into sequence of steps
#### After the steps we need to move to code what we worked before
    For example, when you look at the picture on the
    left how do you tell which person is the tallest?
    A computer would need explicit, step-by-step
    instructi0ns, such as:
        1. Find the height of the first person
        2. Assume he or she is the "tallest person"
        3. Look at the height of the remaining people oneby-one and compare their height to the "tallest
        person" you have found so far
        4. At each step, if you find someone whose height is
            greater than the current "tallest person", he or she
            becomes the new "tallest person"
        5. Once you have checked all the people, tell me
           which one is the tallest  


##### lastly the script should have a Main goal to define 



# Second section talk about 

## Expressions Operators

# Experessions is 
##### An expression evaluates into (results in) a single value. Broadly speaking there are two types of expressions. 
    EXPRESSIONS THAT JUST ASSIGN A
    VALUE TO A VARIABLE Like this : var color = 'beige'; 
    And EXPRESSIONS THAT USE TWO OR
    MORE VALUES TO RETURN A 
    SINGLE VALUE For Example : var area = 3 * 2;

# Operators is 
#### Expressions rely on things called operators; they allow programmers to create a single value from one or more values. 
 #### Types of the operators 
    ASSIGNMENT OPERATORS Like this : color = 'beige'; 
    ARITHMETIC OPERATORS like this : area = 3 * 2; 
    STRING OPERATORS like this : greeting= 'Hi 1 + 'Mol ly'; 
    COMPARISON OPERATORS like : buy = 3 > 5;
    LOGICAL OPERATORS like this : buy= (5 > 3) && (2 < 4); 

# Third section talk about
## Function
    Functions let you group a series of statements together to perform a
    specific task. If different parts of a script repeat the same task, you can
    reuse the function (rather than repeating the same set of statements)

##### we should firstly to do the function make a decleration to it 

    function fuctionName(here we add parameters between them we add a colun , , ,) {
        statment or execution code here
        REturn statment that return some data from the function after make some process on it 
    }
#### then call it using this statment 
    functionName(here the parameters ,,,,);