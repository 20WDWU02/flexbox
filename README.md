# Flexbox
> Flexbox is a module of multiple CSS properties that can be used to help design our websites layouts in a more flexable way which also makes responsive design easier.

## Learning Flexbox
There are multiple places which are great resources on how to learn flexbox. Bellow is a link to 3 places I would recommend having a read through.  
* [CSS Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
* [W3Schools](https://www.w3schools.com/css/css3_flexbox.asp)
* [Flexbox Froggy](https://flexboxfroggy.com/)

## Flex Container

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
* flex-flow
* justify-content
* align-items
* align-content

### flex-direction
