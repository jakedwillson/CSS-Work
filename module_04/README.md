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
