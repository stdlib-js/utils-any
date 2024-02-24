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


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

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

```javascript
import any from 'https://cdn.jsdelivr.net/gh/stdlib-js/utils-any@deno/mod.js';
```
The previous example will load the latest bundled code from the deno branch. Alternatively, you may load a specific version by loading the file from one of the [tagged bundles](https://github.com/stdlib-js/utils-any/tags). For example,

```javascript
import any from 'https://cdn.jsdelivr.net/gh/stdlib-js/utils-any@v0.2.1-deno/mod.js';
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

```javascript
import randu from 'https://cdn.jsdelivr.net/gh/stdlib-js/random-base-randu@deno/mod.js';
import any from 'https://cdn.jsdelivr.net/gh/stdlib-js/utils-any@deno/mod.js';

var bool;
var arr;
var i;

arr = [];
for ( i = 0; i < 100; i++ ) {
    arr.push( ( randu() > 0.95 ) );
}

bool = any( arr );
// returns <boolean>
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

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/utils-any.svg
[npm-url]: https://npmjs.org/package/@stdlib/utils-any

[test-image]: https://github.com/stdlib-js/utils-any/actions/workflows/test.yml/badge.svg?branch=v0.2.1
[test-url]: https://github.com/stdlib-js/utils-any/actions/workflows/test.yml?query=branch:v0.2.1

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/utils-any/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/utils-any?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/utils-any.svg
[dependencies-url]: https://david-dm.org/stdlib-js/utils-any/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/utils-any/tree/deno
[deno-readme]: https://github.com/stdlib-js/utils-any/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/utils-any/tree/umd
[umd-readme]: https://github.com/stdlib-js/utils-any/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/utils-any/tree/esm
[esm-readme]: https://github.com/stdlib-js/utils-any/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/utils-any/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/utils-any/main/LICENSE

[mdn-array]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array

[mdn-typed-array]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/TypedArray

[mdn-object]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object

<!-- <related-links> -->

[@stdlib/utils/any-by]: https://github.com/stdlib-js/utils-any-by/tree/deno

[@stdlib/utils/every]: https://github.com/stdlib-js/utils-every/tree/deno

[@stdlib/utils/for-each]: https://github.com/stdlib-js/utils-for-each/tree/deno

[@stdlib/utils/none]: https://github.com/stdlib-js/utils-none/tree/deno

[@stdlib/utils/some]: https://github.com/stdlib-js/utils-some/tree/deno

<!-- </related-links> -->

</section>

<!-- /.links -->
