# Website Challenges
Update your code in CodePen to complete the following challenges!

#### Reference
https://codepen.io/jmaxwell/pen/BaBVVrO

## HTML Challenges
### Adding an image
1. In the HTML section, add an `h2` saying "A Cool Image"
1. Beneath the `h2`, add an `img` element to the page
    - This will not do anything
    - Ask the students what is needed to create an image (the image)
1. Search for an image of a cat using Google Images in Chrome
1. Right click and select "Copy image address"
    - Do not copy the image itself, that will not work!
1. Add a `src` attribute to the `img` element, and paste in the URL for the image
1. Finally, in the CSS section, select the `img` element and set the `height` so that it fits on the page

```html
<h2>A Cool Image</h2>
<img src="https://img.purch.com/w/660/aHR0cDovL3d3dy5saXZlc2NpZW5jZS5jb20vaW1hZ2VzL2kvMDAwLzEwNC84MTkvb3JpZ2luYWwvY3V0ZS1raXR0ZW4uanBn">
```

```css
img {
    height: 200px;
}
```