# Flexbox
 Flexbox is a layout model in CSS designed for creating more flexible and efficient layouts. It provides a more efficient way to lay out, align, and distribute space among items in a container, even when their size is unknown or dynamic. 
 Sure! Flexbox is a layout model in CSS designed for creating more flexible and efficient layouts. It provides a more efficient way to lay out, align, and distribute space among items in a container, even when their size is unknown or dynamic. Here's a basic overview of how to use Flexbox:

 <img src="./Img/01.png" width="400px" height="400px">

1. **Container and Items**: In Flexbox, you have a container element (parent) and the items inside it (children) that you want to lay out.

2. **Display Property**: To use Flexbox, set the display property of the container element to `flex`:

   ```css
   .container {
     display: flex;
   }
   ```

3. **Flex Direction**: By default, items in a flex container will be laid out in a row. You can change the direction using the `flex-direction` property:

   ```css
   .container {
     display: flex;
     flex-direction: row | row-reverse | column | column-reverse;
   }
   ```

4. **Justify Content**: This property aligns flex items along the main axis of the container. It helps in distributing space between and around items:

   ```css
   .container {
     display: flex;
     justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly;
   }
   ```

5. **Align Items**: This property aligns flex items along the cross axis of the container:

   ```css
   .container {
     display: flex;
     align-items: flex-start | flex-end | center | baseline | stretch;
   }
   ```

6. **Flex Wrap**: This property specifies whether flex items should wrap or not if there's not enough space in the flex container. The values are `nowrap`, `wrap`, or `wrap-reverse`.

   ```css
   .container {
     flex-wrap: nowrap | wrap | wrap-reverse;
   }
   ```

7. **Align Content**: This property aligns a flex container's lines within the flex container when there's extra space on the cross-axis. It's similar to `justify-content`, but instead of aligning items, it aligns the lines:

   ```css
   .container {
     align-content: flex-start | flex-end | center | space-between | space-around | stretch;
   }
   ```
8. **Gap**: This property is part of the newer CSS Grid Layout Module Level 1, not specifically part of Flexbox. It sets the gaps (gutters) between grid items. However, you can simulate a gap between flex items using margin or padding:

   ```css
   .container {
     gap: 10px; /* Any length value. */
   }
   ```

9. **Flex Grow**: This property defines the ability for a flex  item to grow if necessary. It specifies the flex grow factor, which determines how much of the available space in the flex container the item should take up:

   ```css
   .item {
     flex-grow: 1; /* Any positive number. Default is 0. */
   }
   ```

10. **Flex Shrink**: This property defines the ability for a  flex item to shrink if necessary. It specifies the flex shrink factor, which determines how much the item should shrink relative to other flex items:

     ```css
    .item {
     flex-shrink: 1; /* Any positive number. Default is 1. */
    }
    ```

11. **Flex Basis**: This property specifies the initial main size of a flex item before any free space is distributed according to the `flex-grow` and `flex-shrink` properties. It sets the initial size of the flex item:

     ```css
    .item {
     flex-basis: 100px; /* Any length value or percentage. Default is auto. */
    }
     ```
12. **Flex**: The `flex` property is a shorthand for `flex-grow`, `flex-shrink`, and `flex-basis`. It specifies how a flex item will grow or shrink to fit the available space:
  
    ```css
    .item {
        flex: 1; /* flex-grow: 1, flex-shrink: 1, flex-basis: 0% */
    }
    ```

13. **Align Self**: This property allows you to override the `align-items` property for individual flex items:

    ```css
    .item {
        align-self: auto | flex-start | flex-end | center | baseline | stretch;
    }
    ```

6. **Order**: This property specifies the order in which a flex item appears in the flex container, overriding its order in the HTML source code. It's an integer value that determines the order:

   ```css
   .item {
     order: 1; /* Any integer value. Default is 0. */
   }
   ```







