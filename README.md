# sass-sprintf
sprintf function for Sass. Stolen directly from https://github.com/cahnory

### Usage
```scss
@import 'mixins/_sprintf';

$sizes: 1/4 200px auto;
$gutter: 45px;
$args: $sizes, $gutter;

.column {
  @for $i from 1 through 12 {
    width: sprintf(
      ('ant(', 1, ')[', 2, ']'),
      ($args, $i)
    );
  }
}
```
