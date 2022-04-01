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

# Path Separator

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Platform-specific path segment separator.



<section class="usage">

## Usage

To use in Observable,

```javascript
PATH_SEP = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/constants-path-sep@umd/bundle.js' )
```

To include the bundle in a webpage,

```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/constants-path-sep@umd/bundle.js"></script>
```

If no recognized module system is present, access bundle contents via the global scope:

```html
<script type="text/javascript">
(function () {
    window.PATH_SEP;
})();
</script>
```

#### PATH_SEP

Platform-specific path segment separator.

```javascript
var IS_WINDOWS = require( '@stdlib/assert-is-windows' );

var bool;
if ( IS_WINDOWS ) {
    bool = ( PATH_SEP === '\\' );
    // returns true
} else {
    bool = ( PATH_SEP === '/' );
    // returns true
}
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/assert-is-windows@umd/bundle.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/constants-path-sep@umd/bundle.js"></script>
<script type="text/javascript">
(function () {

var parts;
var path;

if ( IS_WINDOWS ) {
    path = 'foo\\bar\\baz';
} else {
    path = 'foo/bar/baz';
}
parts = path.split( PATH_SEP );
console.log( parts );
// => ['foo','bar','baz']

})();
</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/constants/path/sep-posix`][@stdlib/constants/path/sep-posix]</span><span class="delimiter">: </span><span class="description">POSIX path segment separator.</span>
-   <span class="package-name">[`@stdlib/constants/path/sep-win32`][@stdlib/constants/path/sep-win32]</span><span class="delimiter">: </span><span class="description">Windows path segment separator.</span>

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

Copyright &copy; 2016-2022. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/constants-path-sep.svg
[npm-url]: https://npmjs.org/package/@stdlib/constants-path-sep

[test-image]: https://github.com/stdlib-js/constants-path-sep/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/constants-path-sep/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/constants-path-sep/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/constants-path-sep?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/constants-path-sep.svg
[dependencies-url]: https://david-dm.org/stdlib-js/constants-path-sep/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/constants-path-sep/tree/deno
[umd-url]: https://github.com/stdlib-js/constants-path-sep/tree/umd
[esm-url]: https://github.com/stdlib-js/constants-path-sep/tree/esm

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/constants-path-sep/main/LICENSE

<!-- <related-links> -->

[@stdlib/constants/path/sep-posix]: https://github.com/stdlib-js/constants-path-sep-posix/tree/umd

[@stdlib/constants/path/sep-win32]: https://github.com/stdlib-js/constants-path-sep-win32/tree/umd

<!-- </related-links> -->

</section>

<!-- /.links -->
