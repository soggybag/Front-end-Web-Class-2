# Front-end Web: Lesson 2

Web design with CSS an introduction

## Class objectives

students will: 

- Identify Selectors, properties, and values
- Write CSS rules
- Modify tags with class names
- Formulate selectors to select anything in a page

## Schedule 

|   | Time   |    | Activity | Description|
|---|--------|----|----------|------------|
| 1 | 5 min  |   5| TT       | What is CSS? |
| 2 | 5 min  |  10| I do, we do | Create a style sheet, link it to a document |
| 3 | 5 min  |  15| TT       | CSS syntax, Selectors, Properties, and values |
| 4 | 5 min  |  50| I do, we do | Adding styles |
| 5 | 10 min |  60| Break    |   |
| 6 | 10 min |  70| Pair     | CSS Diner quiz |
| 7 | 5 min  |  75| TT       | Using selectors effectively |
| 8 | 30 min | 105| work     |   |
| 9 | 5 min  | 110| TT       | Some design tips |

### 1 - What is CSS? 

- CSS enforces the separation of content and presentation. 
- CSS is a language of visual description. 
- CSS is super powerful it can: 
  - Set the font, size, color, line spacing, etc
  - Set the size, position and layout of elements in a page
  - Set image and color fills, border styles, size and position
  - Animate elements on a page
  - Apply styles for interactive states
  - and more...
  
#### How do you use CSS?

CSS is written in a plain text document with the .css file extension.
Link your css files to you HTML documents by adding the following to the head tag: 

`<link rel="stylesheet" href="styles.css">`

You can also write CSS inside the  `<style>` tag: 

```
<style>
  /* Your CSS styles here... */
</style>
```

Styles can also be added to any tag with the style attribute: 

`<h1 style="color: red">hello World</h1>`

Linking to a file (first example) is the preferred method. 

#### How do write CSS?

CSS is defined as a collection of rules. Each rule is made up of a selector followed by a block:

```
selector { ...block... }
```

Inside the block you will define property and value pairs that set styles for the elements that match the selector. 
The following  sets the H1 to red, 36px, and Helvetica.

```
h1 {
  font-family: Helvetica;
  font-size: 36px;
  color: red;
}
```

The selector `h1` in this case targets all tags named h1. 

#### Exercise:  Style the sample document

sample-1.html

Use the  list of styles here to look up  each of the styles  below as you apply them. 

- Set the font of the h1 to Helvetica
- set the font-size of  the body tag to  18px
- Set the  color of the body tag to 

### 4 - CSS syntax, Selectors, Properties, and Values

- Not case sensitive, you should stick with lowercase
- A CSS Rule is built from:
  - A selector
  - declaration with one or more property value pairs
- CSS can live in
  - CSS file with the extension .css
  - In the style tag
  - In the style attribute
    - This is the least useful save it for special occasions
    - The selector is implied 
    
### 5 - Example Style

There are hudnereds of CSS style properties. See the list for yourself: 
[https://developer.mozilla.org/en-US/docs/Web/CSS/Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference). 
Don't feel you need to know all of these yet. We will be looking at important CSS properties in future classes. 

Markup [index.html](index.html)

### 6 - Take a Break

### 7 - Learn the power of selectors take the Test: https://flukeout.github.io

### 8 - Use selectors effectively

There are many many selectors. Don’t feel you have use them all. 
Here are the most common selectors that you will use often:

- Tag selector
- Class selector
- Descendant selector
- Child selector

There are many pseudo selectors that are useful for special occasions. For now it's probably best to familiarize yourself
with: 

- :link
- :visited
- :hover
- :active

### 9 - Style your work

- Style the HTML meta doc example 4
  - Challenge: Use only tag selectors along with descendant and child selectors
- Style your App page
  - Challenge: Use only class names
- Try these CSS style properties:
  - font-size
  - font-family
  - color (sets the color of text)
  - line-height
  - font-weight
  - background-color
  - background-image
  - background-size
  - Find some other properties and have fun!
  
#### Units

Except for a couple exceptions every value you declare must include a unit. Typical units are: 

- px - pixels
- pt - points (1/72 in)
- mm - millimeters
- cm - centimeters
- in - inches
- em - A unit equal to the current font size 
- % - Percent

#### Colors 

There are several ways to sepcify a color in CSS. 

Hex colors: 

#57c409 - a mild green

#dddddd - light gray

When the pairs repeat can be written as: 

#ddd

Hex colors begin with the # followed by 3 or 6 digits. With each digit being a number between 0 and f. The first two 
digits represent the red component, the second two digits represent the green component, and the last two represent 
the blue component. 

RGB values can be used in this form: 

rgb(74, 144, 226) -  a friendly  blue

RGBA  rgb with an alpha component: 

rgba(224, 67, 67, 0.5) -  red  50% transparent

####  Simple rules for creating good typography

Have a clear typographic hierarchy. Visitors should know where to begin and what to do next. 
Choices should be clearly laid out. 

Make type that is comfortable to read.  Use line spacing, and  constrast  to make your type more legible. 
Avoid overly saturated  colors and harsh constrast. 

Avoid center aligned text. 

Limit the number of fonts to one, two, maybe three at most. 

## Projects and Challenges

The style guide is something we will continue to work on and improve. At this stage you will not have enough information 
to do all of the things you may think of, that’s okay. We will be talking about new things you can add to your style guide 
as the class progresses. 

- Make a style guide (chose one or more the markup examples)
  - Identify each of the uniquely styled elements in your HTML document
    - Use one or more of the projects from the previous class
    - Separate the elements and create specimens in an HTML file
      - Colors
      - Default font style
      - Heading
      - Sub headings
      - Call outs
      - Block quote
      - Image
      - Header
  - Define styles for common text content tags: 
    - p, h1-6, blockquote, strong, em, a
  - Challenge: Style form elements
  - Challenge: Create a sample style guide page with code samples and specimens
    - In order to create code samples in HTML you will to understand 
      - HTML entities
      - Code and pre tags
- Create a style guide for the screenplay. 
  - The best approach here is to use class names for things like: voice-over, screen direction, character name and other things that are specific to screen plays and don’t have an existing tag. 
- Make some really great buttons
  - Use the <button> tag and set the styles to make it look really cool
  - Take a look at the button examples here and see if you can recreate them or make your own version: [https://www.freshdesignweb.com/css3-buttons/](https://www.freshdesignweb.com/css3-buttons/) to recreate these you will need more CSS than we have covered so far, that’s okay, try it on your own and push yourself.  

## Resources

- [http://styleguides.io](http://styleguides.io)
- [http://alistapart.com/article/creating-style-guides](http://alistapart.com/article/creating-style-guides)
- [https://www.youtube.com/watch?v=x_0rE6ovWCI&list=PLoN_ejT35AEj4HJOkJK7nr4prSN0ZRT3H][https://www.youtube.com/watch?v=x_0rE6ovWCI&list=PLoN_ejT35AEj4HJOkJK7nr4prSN0ZRT3H]
- Investigate font pairs that work together: [http://fontpair.co](http://fontpair.co)
- Google Fonts: [https://fonts.google.com/](https://fonts.google.com/)

