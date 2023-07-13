# CSS Cheatsheet [![My Skills](https://skillicons.dev/icons?i=css&theme=dark)](https://skillicons.dev)

Welcome to the CSS Cheatsheet repository! This repository is a comprehensive reference guide for CSS (Cascading Style Sheets), covering a wide range of CSS properties, selectors, and techniques. Whether you're a beginner learning CSS or an experienced developer seeking a quick reference, this cheatsheet has you covered.

The cheatsheet includes various sections dedicated to fundamental CSS concepts, such as selectors, box model, typography, colors, backgrounds, positioning, flexbox, grid, and more. Each section provides clear explanations, examples, and usage guidelines to help you create visually appealing and responsive web designs.

Feel free to explore this cheatsheet to enhance your CSS skills, streamline your styling process, and create stunning web layouts. The cheatsheet is written in Markdown format, making it easy to view, copy, and paste into your own projects.

If you have any suggestions or would like to contribute to this cheatsheet, please feel free to open an issue or submit a pull request. Let's collaborate and make this cheatsheet a valuable resource for the CSS community!

Happy styling!


## Table of Contents

1. [Introduction](#introduction)
2. [CSS Structure](#css-structure)
3. [Selectors](#selectors)
4. [Box Model](#box-model)
5. [Typography](#typography)
6. [Backgrounds](#backgrounds)
7. [Layout](#layout)
8. [Flexbox](#flexbox)
9. [Transitions and Animations](#transitions-and-animations)
10. [Media Queries](#media-queries)
11. [Miscellaneous](#miscellaneous)
12. [Resources](#resources)

## Introduction

CSS (Cascading Style Sheets) is a styling language used for designing the appearance of web pages. It works hand in hand with HTML to add visual styles and layout to your content. Understanding CSS is essential for creating attractive and engaging websites.

### Including CSS in HTML

To apply CSS styles to your HTML document, you need to include the CSS code in one of the following ways:

1. **Inline Styles**: Inline styles are defined directly within HTML elements using the `style` attribute. Here's an example:

    ```html
    <h1 style="color: blue;">Hello, World!</h1>
    ```

2. **Internal Stylesheet**: Internal stylesheets are defined within the `<style>` tags in the `<head>` section of an HTML document. Here's an example:

    ```html
    <head>
      <style>
        h1 {
          color: blue;
        }
      </style>
    </head>
    <body>
      <h1>Hello, World!</h1>
    </body>
    ```

3. **External Stylesheet**: External stylesheets are created as separate CSS files with a `.css` extension. You link the external stylesheet to your HTML document using the `<link>` tag within the `<head>` section. Here's an example:

    ```html
    <head>
      <link rel="stylesheet" href="styles.css">
    </head>
    <body>
      <h1>Hello, World!</h1>
    </body>
    ```

### Cascading and Specificity

CSS follows a cascading model, meaning that multiple styles can be applied to the same element, and the final style is determined by a set of rules. The specificity of a selector also plays a role in determining which styles are applied. Understanding these concepts is important for managing and troubleshooting CSS styles.

With this introduction, you now have a basic understanding of CSS and how to include it in your HTML documents. Let's explore various CSS properties, selectors, and techniques in the following sections.

## CSS Structure

CSS (Cascading Style Sheets) is a language used for styling web pages. It follows a specific structure to define styles for HTML elements. Understanding the basic structure of CSS will help you write clean and organized code. Here's an overview of the CSS structure:

### Selector

A selector is used to target HTML elements and apply styles to them. It can be an element selector, class selector, ID selector, attribute selector, or a combination of these. Here's an example of a selector:

```css
h1 {
  /* CSS styles for h1 element */
}
```

### Property and Value

Once you have selected an element, you can define one or more CSS properties and their corresponding values. Properties determine the aspect of an element you want to modify, such as its color, size, or position. Values specify the specific settings for the chosen property. Here's an example:

``` css
h1 {
  color: red;
  font-size: 24px;
}
```
### Declaration Block

The declaration block contains one or more property-value pairs enclosed in curly braces {}. Each property-value pair is separated by a semicolon ;. Here's an example:

``` css
h1 {
  color: red;
  font-size: 24px;
}

```

### Comments

Comments are used to add explanatory notes to your CSS code. They are not rendered in the browser but are useful for documenting your styles or leaving reminders for yourself or other developers. Here's an example:

``` css
/* This is a comment */
h1 {
  color: red; /* Set the text color to red */
}
```

### CSS Rule

A CSS rule consists of a selector and a declaration block. It defines the styles to be applied to the selected elements. Here's an example:

``` css
h1 {
  color: red;
  font-size: 24px;
}
```

Understanding the structure of CSS will help you write organized and maintainable code. Use this structure as a guide when working with CSS styles.


## Selectors

CSS selectors are used to target specific HTML elements and apply styles to them. Understanding different types of selectors is essential for effectively styling your web pages. Here are some commonly used CSS selectors:

### Element Selector

An element selector targets HTML elements by their tag name. It applies styles to all elements of the specified tag. Here's an example of an element selector targeting all `<h1>` elements:

``` css
h1 {
  color: blue;
}
```

### Class Selector

A class selector targets elements with a specific class attribute. It allows you to style multiple elements with the same class. Here's an example of a class selector targeting elements with the class name highlight:

``` css
.highlight {
  background-color: yellow;
}
```

### ID Selector

An ID selector targets a single element with a unique ID attribute. It is used when you want to style a specific element on the page. Here's an example of an ID selector targeting an element with the ID header:

``` css
#header {
  font-size: 24px;
}
```

### Attribute Selector

An attribute selector targets elements based on their attribute values. It provides flexibility in selecting elements with specific attribute criteria. Here's an example of an attribute selector targeting all <a> elements with the target="_blank" attribute:

``` css
a[target="_blank"] {
  color: red;
}
```

### Pseudo-class Selector

A pseudo-class selector targets elements based on their state or position in the document. It allows you to style elements in specific scenarios. Here's an example of a pseudo-class selector targeting all <a> elements when hovered:

``` css
a:hover {
  text-decoration: underline;
}
```

CSS selectors provide powerful ways to target and style HTML elements. Use them wisely to apply styles to the desired elements in your web pages.


## Box Model

The CSS box model describes the structure of an HTML element, which consists of the content area, padding, border, and margin. Understanding the box model is crucial for controlling the layout and spacing of elements on a web page.

### Content Area

The content area refers to the actual space occupied by the element's content, such as text or images.

### Padding

Padding is the space between the content area and the element's border. It provides extra space inside the element, helping to create breathing room around the content. Here's an example of setting equal padding on all sides:

```css
.box {
  padding: 10px;
}
```

### Border

The border is a line that surrounds the element's content and padding. It separates the element from its neighboring elements. You can control the width, style, and color of the border. Here's an example of setting a border with a solid line style and red color:

``` css
.box {
  border: 2px solid red;
}
```

### Margin

Margin is the space outside the element, creating separation between the element and other elements on the page. It defines the invisible area around the element. Here's an example of setting equal margin on all sides:

``` css

.box {
  margin: 20px;
}
```
### Shorthand

CSS provides shorthand properties to set multiple box model properties at once. The shorthand order is margin, padding, border, where individual properties are separated by spaces. Here's an example of using the shorthand property to set margin, padding, and border:

``` css
.box {
  margin: 10px;
  padding: 20px;
  border: 2px solid blue;
}
```
Understanding the CSS box model enables you to control the spacing and layout of elements effectively. Experiment with different values for padding, border, and margin to achieve the desired visual effects in your web pages.


## Typography

Typography plays a vital role in web design, influencing the readability and visual appeal of your content. CSS provides a range of properties to control various aspects of typography.

### Font Family

The `font-family` property specifies the typeface or font to be used for text content. You can provide a list of font names as fallback options. Here's an example of setting a font family:

```css
body {
  font-family: "Helvetica Neue", Arial, sans-serif;
}
```

### Font Size

The font-size property determines the size of the text. You can set it using various units such as pixels, percentages, or ems. Here's an example of setting the font size to 18 pixels:

``` css
h1 {
  font-size: 18px;
}
```

### Font Weight

The font-weight property controls the thickness or boldness of the text. Common values include normal, bold, lighter, and numeric values ranging from 100 to 900. Here's an example of setting a bold font weight:

``` css
h2 {
  font-weight: bold;
}
```
### Text Color

The color property determines the color of the text. You can specify the color using named colors, hexadecimal codes, RGB values, or HSL values. Here's an example of setting the text color to red:

``` css

p {
  color: red;
}
```
### Text Alignment

The text-align property controls the horizontal alignment of text within its container. Common values include left, right, center, and justify. Here's an example of center aligning the text:

``` css
p {
  text-align: center;
}
```
### Text Decoration

The text-decoration property is used to add or remove decorations from text, such as underlines, overlines, or line-through. Here's an example of adding an underline to a link:

``` css
a {
  text-decoration: underline;
}
```
CSS provides many more typography-related properties, allowing you to fine-tune the appearance of your text. Experiment with different font families, sizes, weights, and styles to create visually appealing typography in your web pages.


## Backgrounds

CSS provides various properties to control the backgrounds of elements. Backgrounds can be styled with colors, images, and additional effects.

### Background Color

The `background-color` property sets the background color of an element. You can specify colors using named colors, hexadecimal codes, RGB values, or HSL values. Here's an example of setting a blue background color:

```css
body {
  background-color: blue;
}
```

### Background Image

The background-image property allows you to set an image as the background of an element. You can specify the path to the image using the url() function. Here's an example of setting a background image:

``` css

div {
  background-image: url("image.jpg");
}
```


### Background Repeat
The background-repeat property controls how a background image is repeated within an element. Common values include repeat, no-repeat, repeat-x, and repeat-y. Here's an example of preventing the background image from repeating:

``` css
div {
  background-repeat: no-repeat;
}
```

### Background Position

The background-position property determines the starting position of a background image within an element. You can specify positions using keywords like left, right, center, or precise coordinates. Here's an example of positioning the background image to the top right:

``` css

div {
  background-position: top right;
}
```

### Background Size

The background-size property sets the size of a background image within an element. You can specify sizes using keywords like cover or contain, or specific length values. Here's an example of making the background image cover the entire element:

``` css
div {
  background-size: cover;
}
```

CSS provides additional properties and techniques for working with backgrounds, such as gradients and background attachment. Experiment with different background colors, images, repeats, positions, and sizes to create visually appealing backgrounds for your elements.


## Layout

CSS provides several techniques for controlling the layout of elements on a web page. Understanding these layout techniques is essential for creating effective and responsive designs.

### Display

The `display` property determines how an element is rendered on the page. Common values include `block`, `inline`, and `flex`. Here's an example of setting an element as a block-level element:

```css
div {
  display: block;
}
```

### Positioning

The position property allows you to control the position of an element on the page. Common values include static, relative, absolute, and fixed. Here's an example of positioning an element absolutely:

``` css
div {
  position: absolute;
  top: 50px;
  left: 50px;
}
```
### Floating

The float property allows an element to float to either the left or right side of its container. This property is often used for creating multi-column layouts or for positioning elements within text. Here's an example of floating an element to the left:

``` css
img {
  float: left;
}
```

### Clearing Floats

The clear property is used to control the behavior of elements that come after floated elements. It determines whether an element should be allowed to float alongside previously floated elements. Common values include both, left, right, and none. Here's an example of clearing floats:

``` css
div {
  clear: both;
}
```

### Box Sizing

The box-sizing property controls how the total width and height of an element is calculated. By default, the content-box value includes only the content area, while the border-box value includes the content, padding, and border. Here's an example of using the border-box value:

``` css
div {
  box-sizing: border-box;
}
```

CSS provides additional layout techniques, such as flexbox and grid, which offer more advanced and flexible layout capabilities. Experiment with different display values, positioning techniques, floating, clearing floats, and box-sizing to create effective layouts for your web pages.



## Flexbox

Flexbox is a powerful layout module in CSS that allows you to create flexible and responsive layouts. It provides a one-dimensional layout model, making it easier to align and distribute space among elements within a container.

### Container

To create a flex container, you need to set the `display` property to `flex` on the parent element. Here's an example of creating a flex container:

```css
.container {
  display: flex;
}
```

### Direction

The flex-direction property determines the direction of the flex items within the container. Common values include row, column, row-reverse, and column-reverse. Here's an example of setting the direction to column:

``` css
.container {
  flex-direction: column;
}
```

### Justify Content

The justify-content property is used to align flex items along the main axis of the flex container. It controls how extra space is distributed. Common values include flex-start, flex-end, center, space-between, and space-around. Here's an example of centering the flex items:

``` css
.container {
  justify-content: center;
}
```

### Align Items

The align-items property is used to align flex items along the cross axis of the flex container. It determines how items are positioned when they don't occupy all the available space on the cross axis. Common values include flex-start, flex-end, center, baseline, and stretch. Here's an example of aligning items to the center:

``` css
.container {
  align-items: center;
}
```

### Flex Items

Flex items are the children of a flex container. They can have their own properties to control their behavior within the container. Here's an example of making a flex item grow, shrink, and have a specific basis:

``` css
.item {
  flex: 1 0 auto;
}
```
### Order

The order property controls the order in which flex items appear within the flex container. It accepts numeric values to determine the visual order. Here's an example of changing the order of a flex item:

``` css
.item {
  order: 1;
}
```

Flexbox provides numerous other properties and techniques for creating flexible and responsive layouts. Experiment with different flex container and flex item properties to achieve the desired layout for your web pages.





## Transitions and Animations

CSS transitions and animations allow you to add dynamic and interactive effects to your web pages. You can animate property changes, create smooth transitions, and even build complex animations.

### Transition Property

The `transition-property` property specifies the CSS properties to which a transition effect should be applied. It can be a single property or multiple properties separated by commas. Here's an example of applying a transition to the `color` property:

```css
.element {
  transition-property: color;
}
```

### Transition Duration

The transition-duration property determines the duration of the transition effect. It specifies how long it takes for the transition to complete, in seconds (s) or milliseconds (ms). Here's an example of setting a transition duration of 1 second:

``` css
.element {
  transition-duration: 1s;
}
```

### Transition Timing Function

The transition-timing-function property controls the speed curve of the transition effect. It allows you to specify the acceleration and deceleration of the transition. Common values include ease, linear, ease-in, ease-out, and ease-in-out. Here's an example of applying an ease-in-out timing function:

``` css
.element {
  transition-timing-function: ease-in-out;
}
```

### Transition Delay

The transition-delay property specifies a delay before the transition effect starts. It defines when the transition should begin, in seconds (s) or milliseconds (ms). Here's an example of setting a delay of 0.5 seconds:

``` css
.element {
  transition-delay: 0.5s;
}
```

### Animation Name

The animation-name property specifies the name of the keyframes animation that should be applied to an element. It references the @keyframes rule. Here's an example of applying an animation called slide-in:

``` css
.element {
  animation-name: slide-in;
}
```

### Animation Duration

The animation-duration property sets the duration of the animation in seconds (s) or milliseconds (ms). It determines how long the animation takes to complete one cycle. Here's an example of setting an animation duration of 2 seconds:

``` css
.element {
  animation-duration: 2s;
}
```

### Animation Timing Function

The animation-timing-function property controls the speed curve of the animation. It defines how the intermediate property keyframes are calculated. Common values are ease, linear, ease-in, ease-out, and ease-in-out. Here's an example of applying a linear timing function:

``` css
.element {
  animation-timing-function: linear;
}
```

### Animation Delay

The animation-delay property specifies a delay before the animation starts. It determines when the animation should begin, in seconds (s) or milliseconds (ms). Here's an example of setting an animation delay of 0.5 seconds:

``` css
.element {
  animation-delay: 0.5s;
}
```

### Animation Iteration Count

The animation-iteration-count property controls the number of times an animation should repeat. You can set it to a specific number or use the infinite keyword for infinite repetition. Here's an example of setting an animation to repeat 3 times:

``` css
.element {
  animation-iteration-count: 3;
}
```

### Animation Direction

The animation-direction property determines whether an animation plays forwards, backwards, or alternates between forwards and backwards. Common values include normal, reverse, alternate, and alternate-reverse. Here's an example of making an animation alternate between forwards and backwards:

``` css
.element {
  animation-direction: alternate;
}
```

CSS transitions and animations provide a range of possibilities for adding engaging and dynamic effects to your web pages. Experiment with different transition and animation properties to achieve the desired visual effects.

## Media Queries

Media queries are a powerful CSS feature that allows you to apply different styles based on the characteristics of the device or screen. With media queries, you can create responsive designs that adapt to various screen sizes, resolutions, and orientations.

### Syntax

Media queries are written using the `@media` rule followed by a media type and media features. The media type specifies the category of the device, such as `screen`, `print`, `speech`, or `all`. Media features define the specific characteristics you want to target, such as screen width or device orientation. Here's an example of a media query targeting screens with a maximum width of 768 pixels:

```css
@media screen and (max-width: 768px) {
  /* Styles for smaller screens */
}
```

### Media Types

Media types define the category of the device or medium being targeted. Common media types include:

`all`: Applies to all devices and media types.
`screen`: Applies to screens of all sizes, including desktops, laptops, tablets, and smartphones.
`print`: Applies to print-preview and print output.
`speech`: Applies to screen readers and other speech synthesis devices.

### Media Features

Media features allow you to target specific characteristics of the device or screen. Some commonly used media features include:

`width`: Specifies the width of the viewport.
`height`: Specifies the height of the viewport.
`orientation`: Specifies the orientation of the device, either portrait or landscape.
`aspect-ratio`: Specifies the aspect ratio of the viewport.
`color`: Specifies the number of bits per color component for the output device.
`resolution`: Specifies the pixel density of the output device.

Here's an example of a media query targeting devices with a minimum width of 1024 pixels:

``` css
@media screen and (min-width: 1024px) {
  /* Styles for larger screens */
}
```

### Breakpoints

Breakpoints are specific widths at which you define different styles for your layout. They help you create a responsive design that adapts to various screen sizes. By using media queries and breakpoints strategically, you can optimize your layout for different devices. Here's an example of setting breakpoints for common device sizes:

``` css
/* Small screens */
@media screen and (max-width: 576px) {
  /* Styles for small screens */
}

/* Medium screens */
@media screen and (min-width: 577px) and (max-width: 991px) {
  /* Styles for medium screens */
}

/* Large screens */
@media screen and (min-width: 992px) {
  /* Styles for large screens */
}
```

### Typical Device Sizes and Media Queries

Here's a table of typical device sizes and their corresponding media query sizes with example codes:

| Device                    | Media Query Size | Example Code                                                                                   |
| ------------------------- | ---------------- | ---------------------------------------------------------------------------------------------- |
| Mobile Phones (Portrait)  | `<= 576px`       | `@media screen and (max-width: 576px) { /* Styles for mobile phones */ }`                      |
| Mobile Phones (Landscape) | `<= 768px`       | `@media screen and (max-width: 768px) { /* Styles for mobile phones in landscape */ }`         |
| Tablets                   | `768px - 992px`  | `@media screen and (min-width: 768px) and (max-width: 992px) { /* Styles for tablets */ }`     |
| Small Laptops             | `992px - 1200px` | `@media screen and (min-width: 992px) and (max-width: 1200px) { /* Styles for small laptops */ }` |
| Large Laptops             | `>= 1200px`      | `@media screen and (min-width: 1200px) { /* Styles for large laptops */ }`                     |

Feel free to adjust the media query sizes and example codes based on your preferences and the specific breakpoints you want to target. This table can serve as a reference for setting up media queries for various device sizes.


By using media queries and breakpoints effectively, you can create responsive and adaptive designs that provide a better user experience across different devices and screen sizes.


## Miscellaneous

CSS provides various techniques and properties for achieving different effects and enhancing the visual appearance of your web pages. Here are some miscellaneous CSS techniques you can utilize:

### Opacity

The `opacity` property controls the transparency of an element. It accepts a value between 0 and 1, where 0 represents complete transparency and 1 represents full opacity. Here's an example of setting an element to 50% opacity:

```css
.element {
  opacity: 0.5;
}
```

### Box Shadow
The box-shadow property adds a shadow effect to an element. It allows you to specify the horizontal and vertical offsets, blur radius, spread radius, and color of the shadow. Here's an example of adding a box shadow to an element:

``` css
.element {
  box-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
}
```

### Border Radius

The border-radius property rounds the corners of an element. It accepts either a single value or four values to specify the radius of each corner individually. Here's an example of creating a rounded element with a 10-pixel radius:

``` css
.element {
  border-radius: 10px;
}
```

### Transforms
Transforms allow you to modify the shape, size, and position of elements. CSS provides several transform functions, including translate(), rotate(), scale(), and skew(). Here's an example of scaling an element to 1.5 times its original size:

``` css
.element {
  transform: scale(1.5);
}
```

### Media Queries

Media queries allow you to apply different styles based on the characteristics of the device or screen. You can use media queries to create responsive designs that adapt to different screen sizes. Here's an example of applying styles only when the screen width is less than or equal to 768 pixels:

``` css
@media (max-width: 768px) {
  .element {
    /* Styles for smaller screens */
  }
}
```

### Pseudo-classes and Pseudo-elements

CSS pseudo-classes and pseudo-elements select specific elements based on their state or position in the document. They enable you to apply styles to elements dynamically without modifying the HTML structure. Here's an example of styling the link color when it's being hovered:

``` css
a:hover {
  color: red;
}
```

These miscellaneous CSS techniques offer additional flexibility and customization options for your web pages. Experiment with these properties and techniques to enhance the visual presentation and user experience of your designs.








## Resources

- List of helpful CSS resources, tutorials, and reference websites.

Feel free to customize the sections or add additional content based on your specific needs. Happy coding!


Feel free to copy and paste this cheatsheet into your GitHub profile, and use it as a quick reference for CSS3 properties and selectors. Happy coding!

