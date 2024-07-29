<!--

@license Apache-2.0

Copyright (c) 2020 The Stdlib Authors.

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

# Special Functions

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Strided array special math functions.



<section class="usage">

## Usage

```javascript
import ns from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-strided-special@deno/mod.js';
```

You can also import the following named exports from the package:

```javascript
import { abs, abs2, abs2By, absBy, acosBy, acoshBy, acotBy, acothBy, acovercosBy, acoversinBy, ahavercosBy, ahaversinBy, asinBy, asinhBy, atanBy, atanhBy, avercosBy, aversinBy, besselj0By, besselj1By, bessely0By, bessely1By, binetBy, cbrt, cbrtBy, ceil, cosBy, dabs, dabs2, dcbrt, dcbrtBy, dceil, ddeg2rad, deg2rad, dfloor, dinv, dmskabs, dmskabs2, dmskcbrt, dmskceil, dmskdeg2rad, dmskfloor, dmskinv, dmskramp, dmskrsqrt, dmsksqrt, dmsktrunc, dramp, drsqrt, dsqrt, dtrunc, floor, inv, ramp, rsqrt, sabs, sabs2, scbrt, sceil, sdeg2rad, sfloor, sinBy, sinv, smskabs, smskabs2, smskcbrt, smskceil, smskdeg2rad, smskfloor, smskinv, smskramp, smskrsqrt, smsksqrt, smsktrunc, sqrt, sqrtBy, sramp, srsqrt, ssqrt, strunc, trunc } from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-strided-special@deno/mod.js';
```

#### ns

Namespace containing strided array special math functions.

```javascript
var special = ns;
// returns {...}
```

The namespace contains the following strided array functions:

<!-- <toc pattern="*"> -->

<div class="namespace-toc">

-   <span class="signature">[`absBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/abs-by]</span><span class="delimiter">: </span><span class="description">compute the absolute value of each element retrieved from a strided input array via a callback function and assign each result to an element in a strided output array.</span>
-   <span class="signature">[`abs( N, dtypeX, x, strideX, dtypeY, y, strideY )`][@stdlib/math/strided/special/abs]</span><span class="delimiter">: </span><span class="description">compute the absolute value for each element in a strided array.</span>
-   <span class="signature">[`abs2By( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/abs2-by]</span><span class="delimiter">: </span><span class="description">compute the squared absolute value of each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`abs2( N, dtypeX, x, strideX, dtypeY, y, strideY )`][@stdlib/math/strided/special/abs2]</span><span class="delimiter">: </span><span class="description">compute the squared absolute value for each element in a strided array.</span>
-   <span class="signature">[`acosBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/acos-by]</span><span class="delimiter">: </span><span class="description">compute the arccosine of each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`acoshBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/acosh-by]</span><span class="delimiter">: </span><span class="description">compute the hyperbolic arccosine of each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`acotBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/acot-by]</span><span class="delimiter">: </span><span class="description">compute the inverse cotangent of each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`acothBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/acoth-by]</span><span class="delimiter">: </span><span class="description">compute the inverse hyperbolic cotangent of each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`acovercosBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/acovercos-by]</span><span class="delimiter">: </span><span class="description">compute the inverse coversed cosine of each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`acoversinBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/acoversin-by]</span><span class="delimiter">: </span><span class="description">compute the inverse coversed sine of each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`ahavercosBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/ahavercos-by]</span><span class="delimiter">: </span><span class="description">compute the inverse half-value versed cosine of each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`ahaversinBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/ahaversin-by]</span><span class="delimiter">: </span><span class="description">compute the inverse half-value versed sine of each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`asinBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/asin-by]</span><span class="delimiter">: </span><span class="description">compute the arcsine of each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`asinhBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/asinh-by]</span><span class="delimiter">: </span><span class="description">compute the hyperbolic arcsine of each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`atanBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/atan-by]</span><span class="delimiter">: </span><span class="description">compute the arctangent of each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`atanhBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/atanh-by]</span><span class="delimiter">: </span><span class="description">compute the hyperbolic arctangent of each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`avercosBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/avercos-by]</span><span class="delimiter">: </span><span class="description">compute the inverse versed cosine of each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`aversinBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/aversin-by]</span><span class="delimiter">: </span><span class="description">compute the inverse versed sine of each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`besselj0By( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/besselj0-by]</span><span class="delimiter">: </span><span class="description">compute the Bessel function of the first kind of order zero for each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`besselj1By( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/besselj1-by]</span><span class="delimiter">: </span><span class="description">compute the Bessel function of the first kind of order one for each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`bessely0By( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/bessely0-by]</span><span class="delimiter">: </span><span class="description">compute the Bessel function of the second kind of order zero for each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`bessely1By( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/bessely1-by]</span><span class="delimiter">: </span><span class="description">compute the Bessel function of the second kind of order one for each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`binetBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/binet-by]</span><span class="delimiter">: </span><span class="description">evaluate Binet's formula extended to real numbers for each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`cbrtBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/cbrt-by]</span><span class="delimiter">: </span><span class="description">compute the cube root of each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`cbrt( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/cbrt]</span><span class="delimiter">: </span><span class="description">compute the cube root of each element in a strided array.</span>
-   <span class="signature">[`ceil( N, dtypeX, x, strideX, dtypeY, y, strideY )`][@stdlib/math/strided/special/ceil]</span><span class="delimiter">: </span><span class="description">round each element in a strided array toward positive infinity.</span>
-   <span class="signature">[`cosBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/cos-by]</span><span class="delimiter">: </span><span class="description">compute the cosine for each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`dabs( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/dabs]</span><span class="delimiter">: </span><span class="description">compute the absolute value for each element in a double-precision floating-point strided array.</span>
-   <span class="signature">[`dabs2( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/dabs2]</span><span class="delimiter">: </span><span class="description">compute the squared absolute value for each element in a double-precision floating-point strided array.</span>
-   <span class="signature">[`dcbrtBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/dcbrt-by]</span><span class="delimiter">: </span><span class="description">compute the cube root of each element retrieved from a double-precision floating-point strided array via a callback function.</span>
-   <span class="signature">[`dcbrt( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/dcbrt]</span><span class="delimiter">: </span><span class="description">compute the cube root of each element in a double-precision floating-point strided array.</span>
-   <span class="signature">[`dceil( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/dceil]</span><span class="delimiter">: </span><span class="description">round each element in a double-precision floating-point strided array toward positive infinity.</span>
-   <span class="signature">[`ddeg2rad( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/ddeg2rad]</span><span class="delimiter">: </span><span class="description">convert each element in a double-precision floating-point strided array from degrees to radians.</span>
-   <span class="signature">[`deg2rad( N, dtypeX, x, strideX, dtypeY, y, strideY )`][@stdlib/math/strided/special/deg2rad]</span><span class="delimiter">: </span><span class="description">convert each element in a strided array from degrees to radians.</span>
-   <span class="signature">[`dfloor( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/dfloor]</span><span class="delimiter">: </span><span class="description">round each element in a double-precision floating-point strided array toward negative infinity.</span>
-   <span class="signature">[`dinv( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/dinv]</span><span class="delimiter">: </span><span class="description">compute the multiplicative inverse for each element in a double-precision floating-point strided array.</span>
-   <span class="signature">[`dmskabs( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/dmskabs]</span><span class="delimiter">: </span><span class="description">compute the absolute value for each element in a double-precision floating-point strided array according to a strided mask array.</span>
-   <span class="signature">[`dmskabs2( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/dmskabs2]</span><span class="delimiter">: </span><span class="description">compute the squared absolute value for each element in a double-precision floating-point strided array according to a strided mask array.</span>
-   <span class="signature">[`dmskcbrt( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/dmskcbrt]</span><span class="delimiter">: </span><span class="description">compute the cube root for each element in a double-precision floating-point strided array according to a strided mask array.</span>
-   <span class="signature">[`dmskceil( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/dmskceil]</span><span class="delimiter">: </span><span class="description">round each element in a double-precision floating-point strided array toward positive infinity according to a strided mask array.</span>
-   <span class="signature">[`dmskdeg2rad( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/dmskdeg2rad]</span><span class="delimiter">: </span><span class="description">convert each element in a double-precision floating-point strided array from degrees to radians according to a strided mask array.</span>
-   <span class="signature">[`dmskfloor( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/dmskfloor]</span><span class="delimiter">: </span><span class="description">round each element in a double-precision floating-point strided array toward negative infinity according to a strided mask array.</span>
-   <span class="signature">[`dmskinv( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/dmskinv]</span><span class="delimiter">: </span><span class="description">compute the multiplicative inverse for each element in a double-precision floating-point strided array according to a strided mask array.</span>
-   <span class="signature">[`dmskramp( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/dmskramp]</span><span class="delimiter">: </span><span class="description">evaluate the ramp function for each element in a double-precision floating-point strided array according to a strided mask array.</span>
-   <span class="signature">[`dmskrsqrt( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/dmskrsqrt]</span><span class="delimiter">: </span><span class="description">compute the reciprocal square root for each element in a double-precision floating-point strided array according to a strided mask array.</span>
-   <span class="signature">[`dmsksqrt( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/dmsksqrt]</span><span class="delimiter">: </span><span class="description">compute the principal square root for each element in a double-precision floating-point strided array according to a strided mask array.</span>
-   <span class="signature">[`dmsktrunc( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/dmsktrunc]</span><span class="delimiter">: </span><span class="description">round each element in a double-precision floating-point strided array toward zero according to a strided mask array.</span>
-   <span class="signature">[`dramp( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/dramp]</span><span class="delimiter">: </span><span class="description">evaluate the ramp function for each element in a double-precision floating-point strided array.</span>
-   <span class="signature">[`drsqrt( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/drsqrt]</span><span class="delimiter">: </span><span class="description">compute the reciprocal square root for each element in a double-precision floating-point strided array.</span>
-   <span class="signature">[`dsqrt( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/dsqrt]</span><span class="delimiter">: </span><span class="description">compute the principal square root for each element in a double-precision floating-point strided array.</span>
-   <span class="signature">[`dtrunc( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/dtrunc]</span><span class="delimiter">: </span><span class="description">round each element in a double-precision floating-point strided array toward zero.</span>
-   <span class="signature">[`floor( N, dtypeX, x, strideX, dtypeY, y, strideY )`][@stdlib/math/strided/special/floor]</span><span class="delimiter">: </span><span class="description">round each element in a strided array toward negative infinity.</span>
-   <span class="signature">[`inv( N, dtypeX, x, strideX, dtypeY, y, strideY )`][@stdlib/math/strided/special/inv]</span><span class="delimiter">: </span><span class="description">compute the multiplicative inverse for each element in a strided array.</span>
-   <span class="signature">[`ramp( N, dtypeX, x, strideX, dtypeY, y, strideY )`][@stdlib/math/strided/special/ramp]</span><span class="delimiter">: </span><span class="description">evaluate the ramp function for each element in a strided array.</span>
-   <span class="signature">[`rsqrt( N, dtypeX, x, strideX, dtypeY, y, strideY )`][@stdlib/math/strided/special/rsqrt]</span><span class="delimiter">: </span><span class="description">compute the reciprocal square root for each element in a strided array.</span>
-   <span class="signature">[`sabs( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/sabs]</span><span class="delimiter">: </span><span class="description">compute the absolute value for each element in a single-precision floating-point strided array.</span>
-   <span class="signature">[`sabs2( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/sabs2]</span><span class="delimiter">: </span><span class="description">compute the squared absolute value for each element in a single-precision floating-point strided array.</span>
-   <span class="signature">[`scbrt( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/scbrt]</span><span class="delimiter">: </span><span class="description">compute the cube root of each element in a single-precision floating-point strided array.</span>
-   <span class="signature">[`sceil( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/sceil]</span><span class="delimiter">: </span><span class="description">round each element in a single-precision floating-point strided array toward positive infinity.</span>
-   <span class="signature">[`sdeg2rad( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/sdeg2rad]</span><span class="delimiter">: </span><span class="description">convert each element in a single-precision floating-point strided array from degrees to radians.</span>
-   <span class="signature">[`sfloor( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/sfloor]</span><span class="delimiter">: </span><span class="description">round each element in a single-precision floating-point strided array toward negative infinity.</span>
-   <span class="signature">[`sinBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/sin-by]</span><span class="delimiter">: </span><span class="description">compute the sine of each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`sinv( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/sinv]</span><span class="delimiter">: </span><span class="description">compute the multiplicative inverse for each element in a single-precision floating-point strided array.</span>
-   <span class="signature">[`smskabs( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/smskabs]</span><span class="delimiter">: </span><span class="description">compute the absolute value for each element in a single-precision floating-point strided array according to a strided mask array.</span>
-   <span class="signature">[`smskabs2( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/smskabs2]</span><span class="delimiter">: </span><span class="description">compute the squared absolute value for each element in a single-precision floating-point strided array according to a strided mask array.</span>
-   <span class="signature">[`smskcbrt( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/smskcbrt]</span><span class="delimiter">: </span><span class="description">compute the cube root for each element in a single-precision floating-point strided array according to a strided mask array.</span>
-   <span class="signature">[`smskceil( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/smskceil]</span><span class="delimiter">: </span><span class="description">round each element in a single-precision floating-point strided array toward positive infinity according to a strided mask array.</span>
-   <span class="signature">[`smskdeg2rad( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/smskdeg2rad]</span><span class="delimiter">: </span><span class="description">convert each element in a single-precision floating-point strided array from degrees to radians according to a strided mask array.</span>
-   <span class="signature">[`smskfloor( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/smskfloor]</span><span class="delimiter">: </span><span class="description">round each element in a single-precision floating-point strided array toward negative infinity according to a strided mask array.</span>
-   <span class="signature">[`smskinv( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/smskinv]</span><span class="delimiter">: </span><span class="description">compute the multiplicative inverse for each element in a single-precision floating-point strided array according to a strided mask array.</span>
-   <span class="signature">[`smskramp( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/smskramp]</span><span class="delimiter">: </span><span class="description">evaluate the ramp function for each element in a single-precision floating-point strided array according to a strided mask array.</span>
-   <span class="signature">[`smskrsqrt( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/smskrsqrt]</span><span class="delimiter">: </span><span class="description">compute the reciprocal square root for each element in a single-precision floating-point strided array according to a strided mask array.</span>
-   <span class="signature">[`smsksqrt( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/smsksqrt]</span><span class="delimiter">: </span><span class="description">compute the principal square root for each element in a single-precision floating-point strided array according to a strided mask array.</span>
-   <span class="signature">[`smsktrunc( N, x, sx, m, sm, y, sy )`][@stdlib/math/strided/special/smsktrunc]</span><span class="delimiter">: </span><span class="description">round each element in a single-precision floating-point strided array toward zero according to a strided mask array.</span>
-   <span class="signature">[`sqrtBy( N, x, strideX, y, strideY, clbk[, thisArg] )`][@stdlib/math/strided/special/sqrt-by]</span><span class="delimiter">: </span><span class="description">compute the principal square root for each element retrieved from an input strided array via a callback function.</span>
-   <span class="signature">[`sqrt( N, dtypeX, x, strideX, dtypeY, y, strideY )`][@stdlib/math/strided/special/sqrt]</span><span class="delimiter">: </span><span class="description">compute the principal square root for each element in a strided array.</span>
-   <span class="signature">[`sramp( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/sramp]</span><span class="delimiter">: </span><span class="description">evaluate the ramp function for each element in a single-precision floating-point strided array.</span>
-   <span class="signature">[`srsqrt( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/srsqrt]</span><span class="delimiter">: </span><span class="description">compute the reciprocal square root for each element in a single-precision floating-point strided array.</span>
-   <span class="signature">[`ssqrt( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/ssqrt]</span><span class="delimiter">: </span><span class="description">compute the principal square root for each element in a single-precision floating-point strided array.</span>
-   <span class="signature">[`strunc( N, x, strideX, y, strideY )`][@stdlib/math/strided/special/strunc]</span><span class="delimiter">: </span><span class="description">round each element in a single-precision floating-point strided array toward zero.</span>
-   <span class="signature">[`trunc( N, dtypeX, x, strideX, dtypeY, y, strideY )`][@stdlib/math/strided/special/trunc]</span><span class="delimiter">: </span><span class="description">round each element in a strided array toward zero.</span>

</div>

<!-- </toc> -->

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- TODO: better examples -->

<!-- eslint no-undef: "error" -->

```javascript
import objectKeys from 'https://cdn.jsdelivr.net/gh/stdlib-js/utils-keys@deno/mod.js';
import ns from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-strided-special@deno/mod.js';

console.log( objectKeys( ns ) );
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

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

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-strided-special.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-strided-special

[test-image]: https://github.com/stdlib-js/math-strided-special/actions/workflows/test.yml/badge.svg?branch=v0.2.2
[test-url]: https://github.com/stdlib-js/math-strided-special/actions/workflows/test.yml?query=branch:v0.2.2

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-strided-special/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-strided-special?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-strided-special.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-strided-special/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-strided-special/tree/deno
[deno-readme]: https://github.com/stdlib-js/math-strided-special/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/math-strided-special/tree/umd
[umd-readme]: https://github.com/stdlib-js/math-strided-special/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/math-strided-special/tree/esm
[esm-readme]: https://github.com/stdlib-js/math-strided-special/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/math-strided-special/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-strided-special/main/LICENSE

<!-- <toc-links> -->

[@stdlib/math/strided/special/abs-by]: https://github.com/stdlib-js/math-strided-special-abs-by/tree/deno

[@stdlib/math/strided/special/abs]: https://github.com/stdlib-js/math-strided-special-abs/tree/deno

[@stdlib/math/strided/special/abs2-by]: https://github.com/stdlib-js/math-strided-special-abs2-by/tree/deno

[@stdlib/math/strided/special/abs2]: https://github.com/stdlib-js/math-strided-special-abs2/tree/deno

[@stdlib/math/strided/special/acos-by]: https://github.com/stdlib-js/math-strided-special-acos-by/tree/deno

[@stdlib/math/strided/special/acosh-by]: https://github.com/stdlib-js/math-strided-special-acosh-by/tree/deno

[@stdlib/math/strided/special/acot-by]: https://github.com/stdlib-js/math-strided-special-acot-by/tree/deno

[@stdlib/math/strided/special/acoth-by]: https://github.com/stdlib-js/math-strided-special-acoth-by/tree/deno

[@stdlib/math/strided/special/acovercos-by]: https://github.com/stdlib-js/math-strided-special-acovercos-by/tree/deno

[@stdlib/math/strided/special/acoversin-by]: https://github.com/stdlib-js/math-strided-special-acoversin-by/tree/deno

[@stdlib/math/strided/special/ahavercos-by]: https://github.com/stdlib-js/math-strided-special-ahavercos-by/tree/deno

[@stdlib/math/strided/special/ahaversin-by]: https://github.com/stdlib-js/math-strided-special-ahaversin-by/tree/deno

[@stdlib/math/strided/special/asin-by]: https://github.com/stdlib-js/math-strided-special-asin-by/tree/deno

[@stdlib/math/strided/special/asinh-by]: https://github.com/stdlib-js/math-strided-special-asinh-by/tree/deno

[@stdlib/math/strided/special/atan-by]: https://github.com/stdlib-js/math-strided-special-atan-by/tree/deno

[@stdlib/math/strided/special/atanh-by]: https://github.com/stdlib-js/math-strided-special-atanh-by/tree/deno

[@stdlib/math/strided/special/avercos-by]: https://github.com/stdlib-js/math-strided-special-avercos-by/tree/deno

[@stdlib/math/strided/special/aversin-by]: https://github.com/stdlib-js/math-strided-special-aversin-by/tree/deno

[@stdlib/math/strided/special/besselj0-by]: https://github.com/stdlib-js/math-strided-special-besselj0-by/tree/deno

[@stdlib/math/strided/special/besselj1-by]: https://github.com/stdlib-js/math-strided-special-besselj1-by/tree/deno

[@stdlib/math/strided/special/bessely0-by]: https://github.com/stdlib-js/math-strided-special-bessely0-by/tree/deno

[@stdlib/math/strided/special/bessely1-by]: https://github.com/stdlib-js/math-strided-special-bessely1-by/tree/deno

[@stdlib/math/strided/special/binet-by]: https://github.com/stdlib-js/math-strided-special-binet-by/tree/deno

[@stdlib/math/strided/special/cbrt-by]: https://github.com/stdlib-js/math-strided-special-cbrt-by/tree/deno

[@stdlib/math/strided/special/cbrt]: https://github.com/stdlib-js/math-strided-special-cbrt/tree/deno

[@stdlib/math/strided/special/ceil]: https://github.com/stdlib-js/math-strided-special-ceil/tree/deno

[@stdlib/math/strided/special/cos-by]: https://github.com/stdlib-js/math-strided-special-cos-by/tree/deno

[@stdlib/math/strided/special/dabs]: https://github.com/stdlib-js/math-strided-special-dabs/tree/deno

[@stdlib/math/strided/special/dabs2]: https://github.com/stdlib-js/math-strided-special-dabs2/tree/deno

[@stdlib/math/strided/special/dcbrt-by]: https://github.com/stdlib-js/math-strided-special-dcbrt-by/tree/deno

[@stdlib/math/strided/special/dcbrt]: https://github.com/stdlib-js/math-strided-special-dcbrt/tree/deno

[@stdlib/math/strided/special/dceil]: https://github.com/stdlib-js/math-strided-special-dceil/tree/deno

[@stdlib/math/strided/special/ddeg2rad]: https://github.com/stdlib-js/math-strided-special-ddeg2rad/tree/deno

[@stdlib/math/strided/special/deg2rad]: https://github.com/stdlib-js/math-strided-special-deg2rad/tree/deno

[@stdlib/math/strided/special/dfloor]: https://github.com/stdlib-js/math-strided-special-dfloor/tree/deno

[@stdlib/math/strided/special/dinv]: https://github.com/stdlib-js/math-strided-special-dinv/tree/deno

[@stdlib/math/strided/special/dmskabs]: https://github.com/stdlib-js/math-strided-special-dmskabs/tree/deno

[@stdlib/math/strided/special/dmskabs2]: https://github.com/stdlib-js/math-strided-special-dmskabs2/tree/deno

[@stdlib/math/strided/special/dmskcbrt]: https://github.com/stdlib-js/math-strided-special-dmskcbrt/tree/deno

[@stdlib/math/strided/special/dmskceil]: https://github.com/stdlib-js/math-strided-special-dmskceil/tree/deno

[@stdlib/math/strided/special/dmskdeg2rad]: https://github.com/stdlib-js/math-strided-special-dmskdeg2rad/tree/deno

[@stdlib/math/strided/special/dmskfloor]: https://github.com/stdlib-js/math-strided-special-dmskfloor/tree/deno

[@stdlib/math/strided/special/dmskinv]: https://github.com/stdlib-js/math-strided-special-dmskinv/tree/deno

[@stdlib/math/strided/special/dmskramp]: https://github.com/stdlib-js/math-strided-special-dmskramp/tree/deno

[@stdlib/math/strided/special/dmskrsqrt]: https://github.com/stdlib-js/math-strided-special-dmskrsqrt/tree/deno

[@stdlib/math/strided/special/dmsksqrt]: https://github.com/stdlib-js/math-strided-special-dmsksqrt/tree/deno

[@stdlib/math/strided/special/dmsktrunc]: https://github.com/stdlib-js/math-strided-special-dmsktrunc/tree/deno

[@stdlib/math/strided/special/dramp]: https://github.com/stdlib-js/math-strided-special-dramp/tree/deno

[@stdlib/math/strided/special/drsqrt]: https://github.com/stdlib-js/math-strided-special-drsqrt/tree/deno

[@stdlib/math/strided/special/dsqrt]: https://github.com/stdlib-js/math-strided-special-dsqrt/tree/deno

[@stdlib/math/strided/special/dtrunc]: https://github.com/stdlib-js/math-strided-special-dtrunc/tree/deno

[@stdlib/math/strided/special/floor]: https://github.com/stdlib-js/math-strided-special-floor/tree/deno

[@stdlib/math/strided/special/inv]: https://github.com/stdlib-js/math-strided-special-inv/tree/deno

[@stdlib/math/strided/special/ramp]: https://github.com/stdlib-js/math-strided-special-ramp/tree/deno

[@stdlib/math/strided/special/rsqrt]: https://github.com/stdlib-js/math-strided-special-rsqrt/tree/deno

[@stdlib/math/strided/special/sabs]: https://github.com/stdlib-js/math-strided-special-sabs/tree/deno

[@stdlib/math/strided/special/sabs2]: https://github.com/stdlib-js/math-strided-special-sabs2/tree/deno

[@stdlib/math/strided/special/scbrt]: https://github.com/stdlib-js/math-strided-special-scbrt/tree/deno

[@stdlib/math/strided/special/sceil]: https://github.com/stdlib-js/math-strided-special-sceil/tree/deno

[@stdlib/math/strided/special/sdeg2rad]: https://github.com/stdlib-js/math-strided-special-sdeg2rad/tree/deno

[@stdlib/math/strided/special/sfloor]: https://github.com/stdlib-js/math-strided-special-sfloor/tree/deno

[@stdlib/math/strided/special/sin-by]: https://github.com/stdlib-js/math-strided-special-sin-by/tree/deno

[@stdlib/math/strided/special/sinv]: https://github.com/stdlib-js/math-strided-special-sinv/tree/deno

[@stdlib/math/strided/special/smskabs]: https://github.com/stdlib-js/math-strided-special-smskabs/tree/deno

[@stdlib/math/strided/special/smskabs2]: https://github.com/stdlib-js/math-strided-special-smskabs2/tree/deno

[@stdlib/math/strided/special/smskcbrt]: https://github.com/stdlib-js/math-strided-special-smskcbrt/tree/deno

[@stdlib/math/strided/special/smskceil]: https://github.com/stdlib-js/math-strided-special-smskceil/tree/deno

[@stdlib/math/strided/special/smskdeg2rad]: https://github.com/stdlib-js/math-strided-special-smskdeg2rad/tree/deno

[@stdlib/math/strided/special/smskfloor]: https://github.com/stdlib-js/math-strided-special-smskfloor/tree/deno

[@stdlib/math/strided/special/smskinv]: https://github.com/stdlib-js/math-strided-special-smskinv/tree/deno

[@stdlib/math/strided/special/smskramp]: https://github.com/stdlib-js/math-strided-special-smskramp/tree/deno

[@stdlib/math/strided/special/smskrsqrt]: https://github.com/stdlib-js/math-strided-special-smskrsqrt/tree/deno

[@stdlib/math/strided/special/smsksqrt]: https://github.com/stdlib-js/math-strided-special-smsksqrt/tree/deno

[@stdlib/math/strided/special/smsktrunc]: https://github.com/stdlib-js/math-strided-special-smsktrunc/tree/deno

[@stdlib/math/strided/special/sqrt-by]: https://github.com/stdlib-js/math-strided-special-sqrt-by/tree/deno

[@stdlib/math/strided/special/sqrt]: https://github.com/stdlib-js/math-strided-special-sqrt/tree/deno

[@stdlib/math/strided/special/sramp]: https://github.com/stdlib-js/math-strided-special-sramp/tree/deno

[@stdlib/math/strided/special/srsqrt]: https://github.com/stdlib-js/math-strided-special-srsqrt/tree/deno

[@stdlib/math/strided/special/ssqrt]: https://github.com/stdlib-js/math-strided-special-ssqrt/tree/deno

[@stdlib/math/strided/special/strunc]: https://github.com/stdlib-js/math-strided-special-strunc/tree/deno

[@stdlib/math/strided/special/trunc]: https://github.com/stdlib-js/math-strided-special-trunc/tree/deno

<!-- </toc-links> -->

</section>

<!-- /.links -->
