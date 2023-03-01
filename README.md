<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# any

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Test whether at least one element in a collection is truthy.

<!-- Section to include introductory text. Make sure to keep an empty line after the intro `section` element and another before the `/section` close. -->

<section class="intro">

</section>

<!-- /.intro -->

<!-- Package usage documentation. -->



<section class="usage">

## Usage

To use in Observable,

```javascript
any = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/utils-any@umd/browser.js' )
```

To vendor stdlib functionality and avoid installing dependency trees for Node.js, you can use the UMD server build:

```javascript
var any = require( 'path/to/vendor/umd/utils-any/index.js' )
```

To include the bundle in a webpage,

```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/utils-any@umd/browser.js"></script>
```

If no recognized module system is present, access bundle contents via the global scope:

```html
<script type="text/javascript">
(function () {
    window.any;
})();
</script>
```

#### any( collection )

Tests whether at least one element in a `collection` is truthy.

```javascript
var arr = [ 0, 0, 0, 0, 1 ];

var bool = any( arr );
// returns true
```

If provided an empty `collection`, the function returns `false`.

```javascript
var bool = any( [] );
// returns false
```

</section>

<!-- /.usage -->

<!-- Package usage notes. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="notes">

## Notes

-   A `collection` may be either an [`Array`][mdn-array], [`Typed Array`][mdn-typed-array], or an array-like [`Object`][mdn-object] (excluding `strings` and `functions`).
-   The function does **not** skip `undefined` elements and is thus not optimized for sparse collections.

</section>

<!-- /.notes -->

<!-- Package usage examples. -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/random-base-randu@umd/browser.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/utils-any@umd/browser.js"></script>
<script type="text/javascript">
(function () {

var bool;
var arr;
var i;

arr = [];
for ( i = 0; i < 100; i++ ) {
    arr.push( ( randu() > 0.95 ) );
}

bool = any( arr );
// returns <boolean>

})();
</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- Section to include cited references. If references are included, add a horizontal rule *before* the section. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="references">

</section>

<!-- /.references -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/utils-any-by`][@stdlib/utils/any-by]</span><span class="delimiter">: </span><span class="description">test whether at least one element in a collection passes a test implemented by a predicate function.</span>
-   <span class="package-name">[`@stdlib/utils-every`][@stdlib/utils/every]</span><span class="delimiter">: </span><span class="description">test whether all elements in a collection are truthy.</span>
-   <span class="package-name">[`@stdlib/utils-for-each`][@stdlib/utils/for-each]</span><span class="delimiter">: </span><span class="description">invoke a function for each element in a collection.</span>
-   <span class="package-name">[`@stdlib/utils-none`][@stdlib/utils/none]</span><span class="delimiter">: </span><span class="description">test whether all elements in a collection are falsy.</span>
-   <span class="package-name">[`@stdlib/utils-some`][@stdlib/utils/some]</span><span class="delimiter">: </span><span class="description">test whether a collection contains at least `n` elements which are truthy.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2023. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/utils-any.svg
[npm-url]: https://npmjs.org/package/@stdlib/utils-any

[test-image]: https://github.com/stdlib-js/utils-any/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/utils-any/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/utils-any/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/utils-any?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/utils-any.svg
[dependencies-url]: https://david-dm.org/stdlib-js/utils-any/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/utils-any/tree/deno
[umd-url]: https://github.com/stdlib-js/utils-any/tree/umd
[esm-url]: https://github.com/stdlib-js/utils-any/tree/esm
[branches-url]: https://github.com/stdlib-js/utils-any/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/utils-any/main/LICENSE

[mdn-array]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array

[mdn-typed-array]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/TypedArray

[mdn-object]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object

<!-- <related-links> -->

[@stdlib/utils/any-by]: https://github.com/stdlib-js/utils-any-by/tree/umd

[@stdlib/utils/every]: https://github.com/stdlib-js/utils-every/tree/umd

[@stdlib/utils/for-each]: https://github.com/stdlib-js/utils-for-each/tree/umd

[@stdlib/utils/none]: https://github.com/stdlib-js/utils-none/tree/umd

[@stdlib/utils/some]: https://github.com/stdlib-js/utils-some/tree/umd

<!-- </related-links> -->

</section>

<!-- /.links -->
