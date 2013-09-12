# Math [![Build Status](https://secure.travis-ci.org/css-recipes/math.png?branch=master)](http://travis-ci.org/css-recipes/math)

> Some Math functions for Sass using plain Sass

## Getting Started

If you haven't used [css-recipes](http://css-recipes.putaindecode.io/) before, be sure to check out the [Getting Started](http://css-recipes.putaindecode.io/getting-started) guide, as it explains consume the recipes using Bower. Once you're familiar with that process, you may install this recipe with this command:

```shell
bower install css-recipe-math --save
```

Once the recipe has been installed (& assuming `bower_components` folder is in your Sass import paths), it may be enabled inside your Sass file with this line:

```scss
@import "css-recipe-math/index"
```

Read more below to find alternative way to use this recipe.


## Component purpose

**`/!\` This recipe is available as Sass (scss) only.**

It brings you some math functions like pow, sqrt, cos, sin etc.

## Sass mixin(s)

### Available functions

+ `crp-Math-pow($x, $exponent)`
+ `crp-Math-factorial($x)`
+ `crp-Math-exp($x)`
+ `crp-Math-ln($x)`
+ `crp-Math-sqrt($x)`

_Note: Due to a Sass limitation, some functions (exp) return approximations according to the limit `$crp-Math-approximationLimit` (default to 25) to avoid infinite calculations. That said, it should be enough for playing with pixels._

### Usage examples

#### Sass use

_This recipes requires Sass `~3.2.0` or libsass `~0.?`_

##### Mixins use

```sass
.org-Component {
    @include crp-Math(...);
}
```

## Release History

 * 2013-09-12   v0.1.1   Change sqrt() algorithm + faster ln().
 * 2013-09-10   v0.1.0   First release with everything needed for sqrt().

---

Recipe submitted by ["MoOx" Maxime Thirouin](http://moox.io)
