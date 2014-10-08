# ng-key-esc

ng-key-esc allow us to pass a function in on an esc key to do what we want for AngularJS

## Why this?

AngularJS doesn’t have an easily alternative.

## Usage

Include `ng-key-esc.js` in your HTML document somewhere after you have set
up AngularJS.

```html
<script src="ng-key-esc.js">
```

Make sure that `ng-key-esc` is a dependency in your AngularJS app.

```js
angular.module("myApp", ["ngKeyEsc"]);
```

### Directive

Use easily this way. The directive accepts a function.

```html
<input type="text" ng-model="your.model" ng-key-esc="hello()" />
```
```js
$scope.hello() = function() {
	alert('Hello World');
};
```

## License

Copyright © 2014 Stewan Pacheco <talk@stpa.co>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the “Software”), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.