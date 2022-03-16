# Layouts

## The Three Types of Layouts

### Float Layouts

- The old way of building layouts of all sizes
- Uses the float property
- Still used, but getting outdated fast

### Flexbox

- Modern way of laying out elements in a 1-dimensional row without using floats
- Perfect for component layouts

### CSS Grid

- For laying out elements in a fully-fledged 2-dimensional grid
- Perfect for page layouts and complex components

## Float Layouts in Details

- Element is removed from the normal flow (out of flow)
- Text and inline elements will wrap around the floated element
- The container will not adjust its height to the element

### Clearfix Hack

```
/* Clearfix hack.
   The `after` element inserts a new element at the end of the container.
   The `after` element only appears if we define something for the content property,
   even if it is just empty text.
   We must set display to block because clearing floats only works on a block-level element.
   Then clearfix should be added to the top level element that contains both float elements
   (header in this case).
*/
.clearfix::after {
  clear: both;
  content: "";
  display: block;
}
```

## Flexbox Layouts in Detail

### Properties

- The container is as tall vertically as the tallest item, or tall enough to contain the content
- Adding `align-items: center` will center the elements vertically. To put them at the top, you can use `align-items: flex-start` and to put them at the bottom, you can use `algin items: flex-end`. The default is `align items: stretch`, which makes them all take up the full space
- The `align-items: center` property is important because it would be extremely difficult to do that without flexbox
- To center horizontally, add `justify-content: center` to the container. To distribute space evenly between all elements, add `justify-content: space-between`.

### Benefits

- Flexbox makes it easy to automatically align items to one another inside a parent container, both horizontally and vertically.
- It solves common problems such as vertical centering and creating equal-height columns.

### Terminology

- The element in which we want to use flexbox is called the Flex container. To set a flex container, set the container's property to `display: flex`. Then, all children of the container will become the flex items.
- The "Main Axis" is the direction in which the flex items are laid out (horizontal). Then, the perpendicular (vertical) axis is called the "Cross Axis".

### Flex Container Properties

1. `gap: 0`. To create space between items without using margin.
1. `justify-content: flex-start`. To align items along the main axis (horizontal by default). There is also flex-end, center, space-between, space-around, space-evenly.
1. `align-items: stretch`. To align items across the cross axis (vertical by default). There is also flex-start, flex-end, center and baseline.
1. `flex-direction: row`. To define which is the main axis (row by default). There is also row-reverse, column and column-reverse.
1. (ADVANCED) `flex-wrap: nowrap`. To allow items to wrap into a new line if they are too large. There is also wrap and wrap-reverse.
1. (ADVANCED) `align-content: stretch`. Only applies when there are mutliple lines (flex-wrap: wrap). There is also flex-start, flex-end, center, space-between and space-around.

### Flex Items Properties

1. `align-self: auto`. To overwrite align-items for individual flex items. There is also stretch, flex-start, flex-end, center and baseline.
1. `flex-grow: 0`. To allow an element to grow (0 means no, 1+ means yes)
1. `flex-shrink: 1`. To allow an element to shrink (0 means no, 1+ means yes)
1. `flex-basis: auto`. To define an item's width, instead of the width property. The value is the length (or auto).
1. `flex: 0 1 auto`. Recommended shorthand for flex-grow, flex-shrink and flex-basis.
1. `order: 0`. Controls order of items. -1 makes the item first, 1 makes it last.

## CSS Grid in Detail

### About CSS Grid

- It is the most modern, and easiest, way of building layouts.
- The grid items are placed in the columns, and as many rows as necessary are created to hold them.

### Example of CSS Grid

````
.container--1 {
  /* Creates a grid of 250px on the left side and 150px right next to it on the left */
  /* The grid template column sizes can be set, and so can the row sizes */
  /* The `gap` or `grid-gap` property can define a gap in between all elements, both 
     in terms of columns and rows. We can use `column-gap` and `row-gap` to separate
     out these values, alternatively. */
  display: grid;
  grid-template-columns: 200px 200px 100px 100px;
  grid-template-rows: 300px 200px;

  /* gap: 30px; */
  column-gap: 30px;
  row-gap: 60px;
}
````

### CSS Grid Overview

1. It is a set of CSS properties for building 2-dimensional layouts
1. The main idea is that we can divide a container element into rows and columns that can be filled with child elements
1. CSS Grid (2-D) is not meant to replace Flexbox (1-D). You simply use them in different situations.

### CSS Grid Terminology

1. The Grid Container is where everything happens, and we set a grid container by setting the `display: grid` property on a container.
1. The child elements of the Grid Container are called the Grid Items.
1. There is a row axis and column axis of a grid, like in flexbox. However, unlike flexbox, we cannot change the directions of the axes.
1. `Grid Lines` are the lines that separate the grid items into boxes (they are numbered from 1 to the number of rows + 1, and 1 to the number of columns + 1).
1. The Grid Lines outline all `Grid Cells` (may or may not be filled by the `Grid Item`).
1. The spaces between the Grid Items are called "gutters" (gaps).
1. A `Grid Track` can be a row or column of grid cells.

### CSS Grid Container Properties

1. `grid-template-rows: (track-size)`; and `grid-template-columns: (track-size); To establish the grid row and column tracks. One length unit for each track. Any unit can be used, new FR fills unused space.
1. `row-gap: 0` and `column-gap: 0`. Or `gap: 0`. Specifying length. To create empty space between tracks.
1. `justify-items: stretch` and `align-items: stretch`. To align items inside rows/columns, horizontally or vertically. Other values are "start", "center" and "end".
1. `justify-content: start` and `align-content: start`. To align entire grid inside grid container. Only applies if container is larger than the grid. Other values are "center" and "end".

### CSS Grid Item Properties

1. `grid-column: (start line/end line)`; and `grid-row: (start line/end line)`. To place a grid item into a specific cell, based on numbers. Span keyword can be used to span an item across more cells.
1. `justify-self: stretch` and `align-self: stretch`. To overwrite justify-items/align-items for single items. Other values are "start", "center" and "end".
