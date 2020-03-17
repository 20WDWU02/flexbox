# Flexbox
> Flexbox is a module of multiple CSS properties that can be used to help design our websites layouts in a more flexable way which also makes responsive design easier.

## Learning Flexbox
There are multiple places which are great resources on how to learn flexbox. Bellow is a link to 3 places I would recommend having a read through.  
* [W3Schools](https://www.w3schools.com/css/css3_flexbox.asp)
* [CSS Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) (has some really good pictures which explains what is going on)
* [Flexbox Froggy](https://flexboxfroggy.com/) (a fun interactive game for learning flexbox)

## Flex Containers

Flexbox is quite easy to understand once you get the core principles behind it.  
The major thing to remember is that for flexbox to work, your elements need to be inside of a **container that has been flexed**. To do this you need to give it `display: flex`. This wil allow all items inside of the container to be flexed. If you don't do this then it won't behave any differently.

```css
.flex-container {
    display: flex;
}
```

## Flexbox Properties
As there are multiple flexbox properties which you can use, this readme won't be able to go over all of them.  
Bellow are just some of the key ones which you would probably use.

* flex-direction
* flex-wrap
* justify-content
* align-items
* align-content

### flex-direction

Using `flex-direction`, you can change the which direction the elements inside will be flexed. By default it uses row, which will mean the items inside will line up side by side horizontally. If you change it to `column`, then they will be stacked up on top of each other vertically. Adding in `-reverse` will also flip the order in which they are written in your html.
```css
.flex-container {
    display: flex;
    flex-direction: row (default) | column | row-reverse | column-reverse;
}
```

### flex-wrap

`flex-wrap` will effect how the container handles the items inside of it when the overall content is larger than the width of its container. If you say `nowrap` (which is the default), items inside of the container will automatically shrink so that they all can fit inside of the container in one row. This will cause items to get really small and often unreadable. If you say `wrap` then items will wrap onto a extra row if there isn't enough space for them to go. Adding in `-reverse` will also flip the order in which they are written in your html.
```css
.flex-container {
    display: flex;
    flex-wrap: nowrap (default) | wrap | wrap-reverse
}
```

### justify-content
`justify-content` will manage how the content inside of the container will be positioned along the `flex-direction`. So if you are using row, `justify-content` will position its elements horizontally. If you change that to `column`, then it would position the elements vertically.

```css
.flex-container {
    display: flex;
    justify-content: flex-start (default) | flex-end | center | space-between | space-around;
    /* there are other options you could look at too but these are the most common */
}
```
* `flex-start` - (Default) The start of the flex directon 
* `flex-end` - The end of the flex directon
* `center` - All items are placed in the center of the direction
* `space-between`- The items are evenly distributed with space between all the items
* `space-around` - The items are evenly distributed with space around all the items

### align-items
`align-items` is very similar to `justify-content` but for the opposite axis. So by default it is for vertically aligning your items.
```css
.flex-container {
    display: flex;
    align-items: stretch (default) | flex-start | flex-end | center;
    /* there are other options you could look at too but these are the most common */
}
```
* `stretch` - (Default) Will stretch/grow the elements to fill the container
* `flex-start` - Will position items at the start of the axis
* `flex-end` - Will position items at the end of the axis
* `center` - Will position items in the center of the axis

### align-content
`align-content` once again behaves the same way as `justify-content` but just for the opposite axis, and takes in the same values.
```css
.flex-container {
    display: flex;
    align-content: flex-start (default) | flex-end | center | space-between | space-around;
    /* there are other options you could look at too but these are the most common */
}
```
## Flex Items
