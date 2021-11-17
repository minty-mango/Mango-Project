# CSS Introduction

## Learning Outcomes

* Add styles to HTML and CSS
* Understand how to use the class and ID attributes
* Add styles to specific elements using the correct selectors
* Understanding wha the cascade does


## Basic Syntax

CSS is made up of various rules. These are:
* selector
* property
* value

![alt text](https://user-images.githubusercontent.com/70952936/130702428-4808becb-cbc4-4a4d-8fa7-f9aa5409768d.jpg 'CSS rules')

## Selectors

These refer to HTML elements which CSS rules apply.

### Universal Selector

These will universially select all elements of any type.

```css
* {
    color: purple;
}
```

### Type Selectors

These will select all elements of a given type.

```css
div {
    color: white;
}
```

### Class Selectors

These will select all elements with a given class.

```css
.alert-text {
    color:red;
}
```
Notice the syntax for this is a period immediately folowed by a case-sensitive value of the class atribute.

Another good note is that you can put multiple classes in a single element. For example: `class='alert-text severe-alert`.

### ID Selectors

ID are similar to classes. They select elements with a given ID.

```css
#title {
    background-color: red;
}
```

We use a hashtag instead of a period for these types. You should use IDs __sparingly__. Main difference between the two is that elements can only have one ID.

### Group Selector

If there are same features in both elements we can use a comma and combine them together.

```css
.read,
.unread {
    color:white;
    background-color: black;
}
```
### Chaining Selectors

If we have two elements both with .subsection class but we want distinct features on one we can chain the two class selectors together

```css
{
    .subsection.header{
        color: red;
    }
}
```

### Descendant Combinator
Combinator allows use to combine multiple selctors differently than grouping or chaining them. There is a total of four types.

```css
.ancestor .contents{
    /* some declarations */
}
```
There is no limit to the amount of combinators you can add to the rule.

## Properties to Get Started With

### Colors

* `color` and `background-color`

### Fonts
* `font-family`
    * For these you want to try and include multiple fonts
* `font-size`: Changes the size of the font
* `font-weight`: chages the boldness of text
* `text-align`: set the text horizontally within an element.

### Image Height and Width

* `height`
* `width`

For this if you want to keep the size of the image to proportions you need to use "auto" to the `height` property

## The Cascade of CSS

