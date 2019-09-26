# Website Follow-Along
An activity to introduce JavaScript (starting with some HTML and CSS)

## Explain HTML (5m)
Start by showing an example webpage (e.g., https://en.wikipedia.org/wiki/SpongeBob_SquarePants) in Google Chrome. Talk to the students about their experience with the web. Then, right click on the page and view the source to show the HTML that builds the page.

### What is HTML
- HTML tells an internet browser what to show on a website
    - Ask students to name internet browsers (chrome, firefox, etc.)
- HTML elements are the building blocks of a webpage
- Browsers use HTML elements to display webpages
    - Examples of HTML elements are links, images, text, tables

## Create a Webpage - Starting with HTML (10m)
Students should follow along to create their own webpages! The webpage will be a "self-portrait" that has some information and a quiz.

### Basic HTML
1. Open a new CodePen: https://codepen.io/pen/ 
    - This allows developers to write HTML code and see it _render_ immediately
1. Change the view so the code appears on the left and the webpage appears on the right
1. Minimize the JS section
1. In the HTML section, add an `h1` header element saying "My Cool Website"
    - Explain that this is used for page titles, and there are also smaller header elements (`h2`-`h6`)
1. Add a `p` paragraph element with a greeting
    - Explain that this is used for regular text on the page

```html
<h1>My Cool Website</h1>
<p>Hi, I'm me.  Welcome to my cool website.</p>
```

#### _TIP: Saving Work_
Direct the students to click the "Save" button in CodePen. They can save anonymously if they do not wish to make an account. Students should make note of their pen's URL so they can recover their code and share it!

### Lists
1. Add an `h2` for "My Favorite Foods" beneath the `p`
1. Add a `ul` that will contain a list of foods beneath the `h2`
    - Pause to ask students if they can guess what the `ul` will be
1. Add `li` elements as children of the `ul`
    - Ask them if they can guess what `li` means
1. Give the students a chance to add some additional foods to their lists
1. Show them that there are both unordered _and_ ordered lists in HTML (`ol`)

```html
<h2>My Favorite Foods</h2>
<ul>
  <li>Pizza</li>
  <li>Burritos</li>
</ul>
```

### Buttons
1. Add a `button` with the text "Quiz Me"
    - This button will start the quiz
1. Add the `onclick` attribute and have it call a function called `quiz()`
    - Explain that **JavaScript** to make the button do something
    - We will come back to this shortly

## Create a Webpage - Styles with CSS (5m)
The current webpage looks fairly boring. Explain that developers use CSS to make their webpages look fun and exciting. HTML is like the skeleton, just the structure of the webpage, and CSS is like the clothes that it wears, giving it style.

1. In the CSS section, add a ruleset to select `body`
1. Add some declarations to update the text color, background color, and font of the page
1. See what would happen if `body` changed to `h1`
    - It only selects the `h1` element
1. Briefly explain web colors to the students: https://en.wikipedia.org/wiki/Web_colors
    - Show them that they can search Google for "color picker" if they want to use custom colors

```css
body {
    color: pink;
    background-color: black;
    font-family: arial;
}
```

**Make sure the students save their work and copy down their URL!**

## Creating a Webpage - Interactivity with JavaScript
Explain that JavaScript is the programming language of the web, that allows webpages to be _interactive_. Developers use JavaScript to trigger events, create animations, make games, and much more.

### Functions in JavaScript - Unplugged Activity (10m)
Have the students open up Notepad. They will write instructions for a self-portrait, telling a computer how to draw them.

#### Part 1: Learn about algorithms, functions, and JavaScript syntax. (10 minutes)
Provide the students with the following definitions:
- Next, you'll see how a complex activity, like drawing a portrait, can be broken down into a series of steps that can be done by a
computer. The series of steps is an algorithm, and the individual actions are functions.
- An **algorithm** is a series of specific instructions that can be applied to many situations. For example, a step-by-step recipe or a set of directions from one place to another are two examples of algorithms you might already use!
- A **function** is one of the basic building blocks of a program. It's a type of instruction that's similar to a verb: a function does something.
- To draw your portrait, you'll create a form of **pseudocode**. Pseudocode is a way to plan a computer program using human-friendly
language instead of a computer language like JavaScript. It's not actual coding, but a written description of the key elements of an
algorithm or program. It's used as a quick way of thinking about a program without completely writing it out in code.
- As you know, in programming, the syntax must be specific, detailed, and exactly correct for a computer to understand it. For that
reason, programmers often use pseudocode to help them flesh out ideas without the burden of being too exact.
- The pseudocode you'll use to describe the key parts of your algorithm borrows its syntax from JavaScript.

Write the below function on a whiteboard or chart paper - or ask for a Senior to volunteer to do this:
drawNose();
Distribute the Code a Portrait handout to each Senior. Have the troop follow along on the handout as you share the Things to Know.
THINGS TO KNOW:
- Now, take a look at this example: drawNose();
- In coding, when you use a function, you would say you're "calling a function."
- In this case, calling the function drawNose(); makes the computer draw a nose on the computer screen.
When you want to call a function in JavaScript or another programming language, you have to follow the syntax for writing a function in
that programming language.
-
Go over the below syntax for writing functions in JavaScript:
- A function starts with a name, which can't have spaces in it, or use other special characters (except underscores '_').
- The name can include numbers - as long as they're not at the beginning.
- The name is directly followed by parentheses '()'. The parentheses tell JavaScript to run the function.
- A semicolon shows that the function has ended, just as a period ends a sentence in English. A semicolon looks like this: ';'
Share the Things to Know for the next part of the activity.
THINGS TO KNOW:
- Now, look at some code that doesn't work.
- Remember the syntax for writing functions in JavaScript and see if you can spot the mistakes.
Ask for another Senior to write the below examples of incorrect code on the whiteboard or chart paper. After she writes each code example,
discuss as a troop why the example uses incorrect syntax.
1st_eye();
make cake;
do-good ();
makeCake()again;
FOR EACH EXAMPLE, DISCUSS: Based on the JavaScript syntax we just went over, why won't the code work?
Answers: The code won't work because...
page 5
© 2018 GSUSA. All rights reserved. Not for commercial use. This material is proprietary to GSUSA and may be used, reproduced, distributed exclusively by GSUSA staff,
councils, Girl Scout volunteers, service units and/or troops solely in connection with Girl Scouting.
1st_eye(); starts with a number.
make cake; has a space and no parentheses.
do-good (); uses a hyphen (or minus sign), which JavaScript doesn't allow, and a space between the name and the ().
makeCake()again; has text after the parentheses.
Part 2: Practice writing pseudocode to draw a smiley face. (5 minutes)
Next, work together as a troop to write pseudocode that describes the steps to draw a smiley face.
Walk Seniors through this process by sharing Things to Know.
THINGS TO KNOW:
Before we get started writing pseudocode, here's an important thing to know. In the Coding for Good badges, you'll experience what it's
like to be BOTH a programmer and a computer.
-
- When you create instructions for a computer, you're called a "programmer" because you're developing code.
When you follow someone else' instructions, you're called a "computer" because you're acting as if you were a computer running the
code.
-
- Now, work as a team of "programmers" to create a short program with three or more tasks (the functions).
- Together, the functions should make up an algorithm that could tell someone how to draw a smiley face.
Work together to describe the steps to draw a smiley face. Ask for Senior to volunteer and write the steps on the whiteboard or chart paper.
Note to Volunteers: As the troop lists the steps to draw a smiley face, they may notice that there are many ways to do it! This is good
thinking.
DISCUSS:
- What shapes do you need to make a smiley face? (Possible answers: the shape of the face, eyes, nose, mouth, etc.)
What are the steps you would use to tell someone how to draw a smiley face?(Possible answers: draw a circle, draw two dots inside
the circle for the eyes, draw an upward semi-circle inside the circle for the smile, etc.)
-
- Is there more than one way to do it? (Answer: Yes.)
- Does the order of steps matter? (Answer: No.)
- Is the size or placement of the shapes important? (Answer: Yes.)
Part 3: Write code to draw a self-portrait. (5 minutes)
Divide into pairs for the next part of the activity. Seniors will start in the role of "programmer" to write code for their self-portrait. In Part 4,
they'll switch to the role of "computer" when they follow their partner's code to draw her portrait.
Walk the troop through the activity by sharing Things to Know. Hand out the paper and pencils and review the "List of simple functions" on
the Code a Portrait handout.
THINGS TO KNOW:
- Now, you'll use functions to write code for a computer to draw a self-portrait of you.
You'll start as a "programmer" and write code for the program for your self-portrait. Then, you'll exchange programs with your partner
and work as a "computer" to make a drawing based on the program she wrote for her self-portrait.
-
The "List of simple functions" on the Code a Portrait handout has some examples of functions you can use to create a portrait
algorithm. You can use these functions or write your own.
-
For this activity, you can use pseudocode or even make up your own functions that use the correct syntax for JavaScript. Remember,
though, once you hand over your algorithm to your partner, you cannot give her any additional instructions for her to "compute" your
portrait.
-
- Now, write an algorithm for a self-portrait of your face.
- For now, keep your algorithm simple.
Give Seniors 5 minutes to write their self-portrait algorithms. Try to keep it to no more than 5 minutes if possible, but make sure to allow time
for questions and clarifications.
If the troop needs an example, you can write the "Pseudocode and Simple Functions Example" below on the whiteboard or chart paper. It
may help to write to the sections (the lines of pseudocode and the lines of functions) side by side.
Pseudocode and Simple Functions Example
This pseudocode:
Get marker 
page 6
© 2018 GSUSA. All rights reserved. Not for commercial use. This material is proprietary to GSUSA and may be used, reproduced, distributed exclusively by GSUSA staff,
councils, Girl Scout volunteers, service units and/or troops solely in connection with Girl Scouting.
Draw circle in the middle of grid
Draw right eye
Draw left eye
Draw nose in center of face
Draw smile under nose
Can be written as these functions:
useMarker();
drawFace();
drawEye();
drawEye();
drawNose();
drawSmile();


## Final
https://codepen.io/jmaxwell/pen/BaBVVrO