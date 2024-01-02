# DOM Attribute Modification

#### *** If you are having trouble with your code some computers will allow you to inspect elements. Pop your website out into a full tab and then right click on an html element. Then select inspect. If you look at the tabs `elements` and `console` it will give you hints to fix any issues

Given this HTML/CSS you are going to modify the elements `attributes` through JS. Your JS won't do anything unless you attach it to `index.html`

## Task 1
Add `<script src="script.js"></script>` to line 44 in the index.html file.
#

Now you can use JS to modify attributes. You will start with style attributes.

```javascript
const pElements = document.getElementsByTagName("p") //grabs all the p elements
const ingredients = pElements[2]// grabbing the third p element in the body
ingredients.style.color = "red"//change the words to the color red
```

## Task 2
Change the color of html line 33 to blue.
#

When you look at `style.css` you will see some of this:
```css
body { background-color: gold;
}
p {color: black;
   font-family: Helvetica
}
h1 {
  color: blue;
  text-align: center;
  font-size: 36px;
  font-style: Helvetica;
}
```

These are all style attributes that you can change with JS. It is really easy once you see the conversion from CSS to JS.

background-color = style.backgroundColor

text-align = style.textAlign

So to make the rule generic you take out the dash and capitalize the first letter in the next work. This is called `camel case`. Unfortunatly, this is just a generic rule and does not work in all conditions

css-word = style.cssWord

## Task 3
1. Change the bodies background color to pink
2. Change line 13 font size to `50px` and text align to `left`
3. Change line 13 font family to `Impact`
#

You can also change the attributes to an image element. Some elements don't require `.style`. It can be hard to know which does and which does not. You may need to search for proper usage.

https://www.w3schools.com/jsref/prop_img_src.asp

Each element has different properties that you can manipulate. You can find them all on the left column under html elements

https://www.w3schools.com/jsref/dom_obj_image.asp

```javascript
const img = document.getelementById("video")
img.src = "https://theultimatecheesesandwich.com/wp-content/uploads/2016/10/Ultimate-Grilled-Cheese-2-1.jpg"

img.height = "75"
```

## Task 4
1. Get the image on line 41 using getElementById. Don't forget you will need to add the id to the html document
2. Change the image to `https://www.thespruceeats.com/thmb/xSiJi_UwbRoI3ce7_Ilfk4SkLfU=/2860x2860/filters:no_upscale():max_bytes(150000):strip_icc()/how-to-make-a-giant-grilled-cheese-4784131-hero-02-6cf82fe3ec1c47b79305c855fca8a9d8.jpg`
3. Change the height to `250`
#

