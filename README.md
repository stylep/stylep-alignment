# stylep-alignment

Everything you need to get started making a new style pattern.

## Install
``` shell
npm i --save-dev stylep-alignment
```

## Usage
``` css
/* name.css */

@import “stylep-alignment”;

.element-start {
  @extend %start;
}

.text-center {
  @extend %text-center;
}
```

## Utilities

### Horizontal

`%start` Aligns the object to the left-hand side of the parent object.

`%center` Aligns the object to the center of the parent object.

`%end` Aligns the object to the right-hand side of the parent object.

`%text-center` Aligns all text in the object this is applied to.

### Vertical

`%top` Aligns the object to the left-hand side of the parent object.

`%middle` Aligns the object to the left-hand side of the parent object.

`%bottom` Aligns the object to the left-hand side of the parent object.

`%text-middle` Vertical align all text in the object this is applied to.

### Distribution

`%around` Places a group of objects with more space surrouding them than in-between them.

`%between` Places a group of objects with more space between them than arround them.

## Mixins

#### `@mixin align;`
This mixin controls the alignment of the object it is applied to.

##### Options

* `$x` Controls the horizontal alignment.
* `$y` Controls the vertical alignment.

##### Example
```css
/* align this object to the beginning left of the parent element */
@mixin align flex-start, start;
```

#### `@mixin text-align;`
This mixin controls the alignment of text objects it is applied to.

##### Options

* `$x` Controls the horizontal alignment.
* `$y` Controls the vertical alignment.

##### Example
```css
/* align text to the left of the parent element  */
@mixin text-align flex-start, center;
```

