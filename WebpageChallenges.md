# Webpage Challenges
Update your code in CodePen to complete the following challenges!

#### Reference
[https://codepen.io/jmaxwell/pen/BaBVVrO](https://codepen.io/jmaxwell/pen/BaBVVrO)

## HTML Challenge: Add an Image
1. In the HTML section, add an `h2` saying "A Cool Image"
1. Beneath the `h2`, add an `img` element to the page
    - This will not do anything yet...
1. Search for an image of a cat using Google Images in Chrome
1. Right click and select **Copy image address**
    - Do not click **Copy image**, that will not work!
1. Add a `src` attribute to the `img` element, and paste in the URL for the image

```html
<h2>A Cool Image</h2>
<img src="your_url_here">
```

## HTML Challenge: Add a Video
1. Go to YouTube and find a video
1. Under the video, click the "SHARE" button  
    ![](https://i.imgur.com/6rOqJb3.png)  
1. Click "Embed"  
    ![](https://i.imgur.com/OPzkSc2.png)  
1. Click "COPY"  
    ![](https://i.imgur.com/barvOys.png)
1. In the HTML section of the CodePen, paste the video code!
    - Use `Ctrl`+`v` or right-click and select Paste

It should look something like this:
```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/7zkX6kfnWbk" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```

## CSS Challenge: Header Text Shadow
1. In the CSS section, under the `}` from the "body" ruleset, make some new lines
1. Create a new ruleset for "h1" by adding `h1` and `{` and `}`
    - This will mean that all styles apply to each `h1` HTML element
    - Note that when adding the opening bracket (`{`), CodePen adds the closing bracket (`}`) automatically
    - With the cursor between the two brackets, press the "Enter" key to properly format the ruleset
1. Within the brackets, add a new declaration: `text-shadow: red -1px 1px`
1. Update the numbers and the color to see how it changes the effect!
1. For more information, check out this article: [https://developer.mozilla.org/en-US/docs/Web/CSS/text-shadow](https://developer.mozilla.org/en-US/docs/Web/CSS/text-shadow)

```css
h1 {
    text-shadow: red -1px 1px;
}
```

## CSS Challenge: Button Color
1. At the bottom of the CSS section, make some new lines
1. Create a new ruleset for "button" by adding `button` `{` and `}`
    - This will mean that all styles apply to each `button` HTML element
1. Within the brackets, add a new declaration: `background-color: yellow;`

### Button Color on Hover
To make the button turn yellow on _hover_, update the `button` in the CSS so it is `button:hover` instead. This will mean that the styles **only apply** when the user hovers over the button.

```css
button:hover {
  background-color: yellow;
}
```

## JavaScript Challenge: Add a Question
1. In the JavaScript section, update the value of the `numberOfQuestions` variable to be `3` instead of `2`
1. Underneath the `}` for the second `if` statement, add a new line
1. Ask the user a third question using `prompt`, and store the user's answer in a variable named `answer3`
    - Ask any appropriate question!
1. Add an `if` statement checking if the user entered the correct answer
1. If the user _did_ enter the correct answer, increase their points!
1. Add more additional questions if desired!

_HINT: Use the existing questions in the code as a guide for creating new questions._

## JavaScript Challenge: Final Message
Instead of simply showing the final score to the user, display a message about the score. For example, if they score 100%, display a message that says "Good Job!"

Under the `alert` at the bottom of the JavaScript `startQuiz` function, create an `if` statement:
1. Start with `if`
1. Add parentheses (`()`)
1. Within the parentheses, compare the `finalScore` to `100` with a double-equals sign
1. After the parentheses, add curly brackets (`{` and `}`) and make a new line between them
1. In the _body_ of the `if`, use an `alert` to display a message of "Good Job!"
    - Note that the program will only display this message _if_ `finalScore` is equal to `100`!

_HINT: Use the existing `if` statements in the code as a guide for creating this `if` statement._

## Share your webpage and quiz
Send your URL to others (or have them sit at your computer) so they can view your webpage and take your quiz!
