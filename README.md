# api documentation for  [tween.js (v16.6.0)](https://github.com/tweenjs/tween.js)  [![npm package](https://img.shields.io/npm/v/npmdoc-tween.js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-tween.js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-tween.js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-tween.js)
#### Super simple, fast and easy to use tweening engine which incorporates optimised Robert Penner's equations.

[![NPM](https://nodei.co/npm/tween.js.png?downloads=true)](https://www.npmjs.com/package/tween.js)

[![apidoc](https://npmdoc.github.io/node-npmdoc-tween.js/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-tween.js%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-tween.js/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-tween.js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-tween.js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "tween.js contributors",
        "url": "https://github.com/tweenjs/tween.js/graphs/contributors"
    },
    "bugs": {
        "url": "https://github.com/tweenjs/tween.js/issues"
    },
    "dependencies": {},
    "description": "Super simple, fast and easy to use tweening engine which incorporates optimised Robert Penner's equations.",
    "devDependencies": {
        "jscs": "^2.2.0",
        "jshint": "^2.8.0",
        "nodeunit": "^0.9.1",
        "semantic-release": "^6.3.2"
    },
    "directories": {},
    "dist": {
        "shasum": "739104c9336cc4f11ee53f9ce7cede51e6723624",
        "tarball": "https://registry.npmjs.org/tween.js/-/tween.js-16.6.0.tgz"
    },
    "gitHead": "ae085330fbc0c4e7911c69e786bd3f697f95943f",
    "homepage": "https://github.com/tweenjs/tween.js",
    "keywords": [
        "tween",
        "interpolation"
    ],
    "license": "MIT",
    "main": "src/Tween.js",
    "maintainers": [
        {
            "name": "sole",
            "email": "listas@soledadpenades.com"
        }
    ],
    "name": "tween.js",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/tweenjs/tween.js.git"
    },
    "scripts": {
        "semantic-release": "semantic-release pre && npm publish && semantic-release post",
        "test": "npm run test-unit && npm run test-correctness && npm run test-style",
        "test-correctness": "jshint --config test/jshintrc src/Tween.js",
        "test-style": "jscs --config test/jscs.json src/Tween.js",
        "test-unit": "nodeunit test/unit/nodeunitheadless.js"
    },
    "version": "16.6.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module tween.js](#apidoc.module.tween.js)
1.  [function <span class="apidocSignatureSpan">tween.js.</span>Tween (object)](#apidoc.element.tween.js.Tween)
1.  [function <span class="apidocSignatureSpan">tween.js.</span>add (tween)](#apidoc.element.tween.js.add)
1.  [function <span class="apidocSignatureSpan">tween.js.</span>getAll ()](#apidoc.element.tween.js.getAll)
1.  [function <span class="apidocSignatureSpan">tween.js.</span>now ()](#apidoc.element.tween.js.now)
1.  [function <span class="apidocSignatureSpan">tween.js.</span>remove (tween)](#apidoc.element.tween.js.remove)
1.  [function <span class="apidocSignatureSpan">tween.js.</span>removeAll ()](#apidoc.element.tween.js.removeAll)
1.  [function <span class="apidocSignatureSpan">tween.js.</span>update (time, preserve)](#apidoc.element.tween.js.update)
1.  object <span class="apidocSignatureSpan">tween.js.</span>Easing
1.  object <span class="apidocSignatureSpan">tween.js.</span>Interpolation
1.  object <span class="apidocSignatureSpan">tween.js.</span>js.Interpolation
1.  object <span class="apidocSignatureSpan">tween.js.</span>js.Interpolation.Utils

#### [module tween.js.Interpolation](#apidoc.module.tween.js.Interpolation)
1.  [function <span class="apidocSignatureSpan">tween.js.Interpolation.</span>Bezier (v, k)](#apidoc.element.tween.js.Interpolation.Bezier)
1.  [function <span class="apidocSignatureSpan">tween.js.Interpolation.</span>CatmullRom (v, k)](#apidoc.element.tween.js.Interpolation.CatmullRom)
1.  [function <span class="apidocSignatureSpan">tween.js.Interpolation.</span>Linear (v, k)](#apidoc.element.tween.js.Interpolation.Linear)
1.  object <span class="apidocSignatureSpan">tween.js.Interpolation.</span>Utils

#### [module tween.js.Interpolation.Utils](#apidoc.module.tween.js.Interpolation.Utils)
1.  [function <span class="apidocSignatureSpan">tween.js.Interpolation.Utils.</span>Bernstein (n, i)](#apidoc.element.tween.js.Interpolation.Utils.Bernstein)
1.  [function <span class="apidocSignatureSpan">tween.js.Interpolation.Utils.</span>CatmullRom (p0, p1, p2, p3, t)](#apidoc.element.tween.js.Interpolation.Utils.CatmullRom)
1.  [function <span class="apidocSignatureSpan">tween.js.Interpolation.Utils.</span>Factorial (n)](#apidoc.element.tween.js.Interpolation.Utils.Factorial)
1.  [function <span class="apidocSignatureSpan">tween.js.Interpolation.Utils.</span>Linear (p0, p1, t)](#apidoc.element.tween.js.Interpolation.Utils.Linear)



# <a name="apidoc.module.tween.js"></a>[module tween.js](#apidoc.module.tween.js)

#### <a name="apidoc.element.tween.js.Tween"></a>[function <span class="apidocSignatureSpan">tween.js.</span>Tween (object)](#apidoc.element.tween.js.Tween)
- description and source-code
```javascript
Tween = function (object) {

	var _object = object;
	var _valuesStart = {};
	var _valuesEnd = {};
	var _valuesStartRepeat = {};
	var _duration = 1000;
	var _repeat = 0;
	var _repeatDelayTime;
	var _yoyo = false;
	var _isPlaying = false;
	var _reversed = false;
	var _delayTime = 0;
	var _startTime = null;
	var _easingFunction = TWEEN.Easing.Linear.None;
	var _interpolationFunction = TWEEN.Interpolation.Linear;
	var _chainedTweens = [];
	var _onStartCallback = null;
	var _onStartCallbackFired = false;
	var _onUpdateCallback = null;
	var _onCompleteCallback = null;
	var _onStopCallback = null;

	this.to = function (properties, duration) {

		_valuesEnd = properties;

		if (duration !== undefined) {
			_duration = duration;
		}

		return this;

	};

	this.start = function (time) {

		TWEEN.add(this);

		_isPlaying = true;

		_onStartCallbackFired = false;

		_startTime = time !== undefined ? time : TWEEN.now();
		_startTime += _delayTime;

		for (var property in _valuesEnd) {

			// Check if an Array was provided as property value
			if (_valuesEnd[property] instanceof Array) {

				if (_valuesEnd[property].length === 0) {
					continue;
				}

				// Create a local copy of the Array with the start value at the front
				_valuesEnd[property] = [_object[property]].concat(_valuesEnd[property]);

			}

			// If 'to()' specifies a property that doesn't exist in the source object,
			// we should not set that property in the object
			if (_object[property] === undefined) {
				continue;
			}

			// Save the starting value.
			_valuesStart[property] = _object[property];

			if ((_valuesStart[property] instanceof Array) === false) {
				_valuesStart[property] *= 1.0; // Ensures we're using numbers, not strings
			}

			_valuesStartRepeat[property] = _valuesStart[property] || 0;

		}

		return this;

	};

	this.stop = function () {

		if (!_isPlaying) {
			return this;
		}

		TWEEN.remove(this);
		_isPlaying = false;

		if (_onStopCallback !== null) {
			_onStopCallback.call(_object, _object);
		}

		this.stopChainedTweens();
		return this;

	};

	this.end = function () {

		this.update(_startTime + _duration);
		return this;

	};

	this.stopChainedTweens = function () {

		for (var i = 0, numChainedTweens = _chainedTweens.length; i < numChainedTweens; i++) {
			_chainedTweens[i].stop();
		}

	};

	this.delay = function (amount) {

		_delayTime = amount;
		return this;

	};

	this.repeat = function (times) {

		_repeat = times;
		return this;

	};

	this.repeatDelay = function (amount) {

		_repeatDelayTime = amount;
		return this;

	};

	this.yoyo = function (yoyo) {

		_yoyo = yoyo;
		return this;

	};


	this.easing = function (easing) {

		_easingFunction = easing;
		return this;

	};

	this.interpolation = function (interpolation) {

		_interpolationFunction = interpolation;
		return this;

	};

	this.chain = function () {

		_chainedTweens = arguments;
		return this;

	};

	this.onStart = function (callback) {

		_onStartCallback = callback;
		return this;

	};

	this.onUpdate = function (callback) {

		_onUpdateCallback = callback;
		return this;

	};

	this.onComplete = function (callback) {

		_onCompleteCallback = callback;
		return this;

	};

	this.onStop = function (callback) {

		_onStopCallback = callback;
		return this;

	};

	this.update = function (time) {

		var property;
		var elapsed;
		var value;

		if (time < _startTime) {
			return true;
		}

		if (_onStartCallbackFired === false) {

			if (_onStartCallback !== null) {
				_onStartCallback.call(_object, _object);
			}

			_onStartCallbackFired = true;
		}

		elapsed = (time - _startTime) / _duration;
		elapsed = elapsed > 1 ? 1 : elapsed;

		value = _easingFunction(elapsed);

		for (property in _valuesEnd) {

			// Don't update properties that do not exist in the source object
			if (_valuesStart[property] === undefined) {
				continue;
			}

			var start = _valuesStart[property] || 0;
			var end = _valuesEnd[property];

			if (end instanceof Array) {

				_object[property] = _interpolationFunction(end, value);

			} else {

				// Parses relative end values with sta ...
```
- example usage
```shell
...
[![NPM Downloads][downloads-image]][downloads-url]
[![Travis tests][travis-image]][travis-url]
[![Flattr this][flattr-image]][flattr-url]
[![CDNJS][cdnjs-image]][cdnjs-url]

'''javascript
var coords = { x: 0, y: 0 };
var tween = new TWEEN.Tween(coords)
	.to({ x: 100, y: 100 }, 1000)
	.onUpdate(function() {
		console.log(this.x, this.y);
	})
	.start();

requestAnimationFrame(animate);
...
```

#### <a name="apidoc.element.tween.js.add"></a>[function <span class="apidocSignatureSpan">tween.js.</span>add (tween)](#apidoc.element.tween.js.add)
- description and source-code
```javascript
add = function (tween) {

			_tweens.push(tween);

		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tween.js.getAll"></a>[function <span class="apidocSignatureSpan">tween.js.</span>getAll ()](#apidoc.element.tween.js.getAll)
- description and source-code
```javascript
getAll = function () {

			return _tweens;

		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tween.js.now"></a>[function <span class="apidocSignatureSpan">tween.js.</span>now ()](#apidoc.element.tween.js.now)
- description and source-code
```javascript
now = function () {
		var time = process.hrtime();

		// Convert [seconds, nanoseconds] to milliseconds.
		return time[0] * 1000 + time[1] / 1000000;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tween.js.remove"></a>[function <span class="apidocSignatureSpan">tween.js.</span>remove (tween)](#apidoc.element.tween.js.remove)
- description and source-code
```javascript
remove = function (tween) {

			var i = _tweens.indexOf(tween);

			if (i !== -1) {
				_tweens.splice(i, 1);
			}

		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tween.js.removeAll"></a>[function <span class="apidocSignatureSpan">tween.js.</span>removeAll ()](#apidoc.element.tween.js.removeAll)
- description and source-code
```javascript
removeAll = function () {

			_tweens = [];

		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tween.js.update"></a>[function <span class="apidocSignatureSpan">tween.js.</span>update (time, preserve)](#apidoc.element.tween.js.update)
- description and source-code
```javascript
update = function (time, preserve) {

			if (_tweens.length === 0) {
				return false;
			}

			var i = 0;

			time = time !== undefined ? time : TWEEN.now();

			while (i < _tweens.length) {

				if (_tweens[i].update(time) || preserve) {
					i++;
				} else {
					_tweens.splice(i, 1);
				}

			}

			return true;

		}
```
- example usage
```shell
...
	})
	.start();

requestAnimationFrame(animate);

function animate(time) {
	requestAnimationFrame(animate);
	TWEEN.update(time);
}
'''

## Installation

Download the [library](https://raw.githubusercontent.com/tweenjs/tween.js/master/src/Tween.js) and include it in your code:
...
```



# <a name="apidoc.module.tween.js.Interpolation"></a>[module tween.js.Interpolation](#apidoc.module.tween.js.Interpolation)

#### <a name="apidoc.element.tween.js.Interpolation.Bezier"></a>[function <span class="apidocSignatureSpan">tween.js.Interpolation.</span>Bezier (v, k)](#apidoc.element.tween.js.Interpolation.Bezier)
- description and source-code
```javascript
Bezier = function (v, k) {

		var b = 0;
		var n = v.length - 1;
		var pw = Math.pow;
		var bn = TWEEN.Interpolation.Utils.Bernstein;

		for (var i = 0; i <= n; i++) {
			b += pw(1 - k, n - i) * pw(k, i) * v[i] * bn(n, i);
		}

		return b;

	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tween.js.Interpolation.CatmullRom"></a>[function <span class="apidocSignatureSpan">tween.js.Interpolation.</span>CatmullRom (v, k)](#apidoc.element.tween.js.Interpolation.CatmullRom)
- description and source-code
```javascript
CatmullRom = function (v, k) {

		var m = v.length - 1;
		var f = m * k;
		var i = Math.floor(f);
		var fn = TWEEN.Interpolation.Utils.CatmullRom;

		if (v[0] === v[m]) {

			if (k < 0) {
				i = Math.floor(f = m * (1 + k));
			}

			return fn(v[(i - 1 + m) % m], v[i], v[(i + 1) % m], v[(i + 2) % m], f - i);

		} else {

			if (k < 0) {
				return v[0] - (fn(v[0], v[0], v[1], v[1], -f) - v[0]);
			}

			if (k > 1) {
				return v[m] - (fn(v[m], v[m], v[m - 1], v[m - 1], f - m) - v[m]);
			}

			return fn(v[i ? i - 1 : 0], v[i], v[m < i + 1 ? m : i + 1], v[m < i + 2 ? m : i + 2], f - i);

		}

	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tween.js.Interpolation.Linear"></a>[function <span class="apidocSignatureSpan">tween.js.Interpolation.</span>Linear (v, k)](#apidoc.element.tween.js.Interpolation.Linear)
- description and source-code
```javascript
Linear = function (v, k) {

		var m = v.length - 1;
		var f = m * k;
		var i = Math.floor(f);
		var fn = TWEEN.Interpolation.Utils.Linear;

		if (k < 0) {
			return fn(v[0], v[1], f);
		}

		if (k > 1) {
			return fn(v[m], v[m - 1], m - f);
		}

		return fn(v[i], v[i + 1 > m ? m : i + 1], f - i);

	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tween.js.Interpolation.Utils"></a>[module tween.js.Interpolation.Utils](#apidoc.module.tween.js.Interpolation.Utils)

#### <a name="apidoc.element.tween.js.Interpolation.Utils.Bernstein"></a>[function <span class="apidocSignatureSpan">tween.js.Interpolation.Utils.</span>Bernstein (n, i)](#apidoc.element.tween.js.Interpolation.Utils.Bernstein)
- description and source-code
```javascript
Bernstein = function (n, i) {

			var fc = TWEEN.Interpolation.Utils.Factorial;

			return fc(n) / fc(i) / fc(n - i);

		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tween.js.Interpolation.Utils.CatmullRom"></a>[function <span class="apidocSignatureSpan">tween.js.Interpolation.Utils.</span>CatmullRom (p0, p1, p2, p3, t)](#apidoc.element.tween.js.Interpolation.Utils.CatmullRom)
- description and source-code
```javascript
CatmullRom = function (p0, p1, p2, p3, t) {

			var v0 = (p2 - p0) * 0.5;
			var v1 = (p3 - p1) * 0.5;
			var t2 = t * t;
			var t3 = t * t2;

			return (2 * p1 - 2 * p2 + v0 + v1) * t3 + (- 3 * p1 + 3 * p2 - 2 * v0 - v1) * t2 + v0 * t + p1;

		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tween.js.Interpolation.Utils.Factorial"></a>[function <span class="apidocSignatureSpan">tween.js.Interpolation.Utils.</span>Factorial (n)](#apidoc.element.tween.js.Interpolation.Utils.Factorial)
- description and source-code
```javascript
Factorial = function (n) {

				var s = 1;

				if (a[n]) {
					return a[n];
				}

				for (var i = n; i > 1; i--) {
					s *= i;
				}

				a[n] = s;
				return s;

			}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tween.js.Interpolation.Utils.Linear"></a>[function <span class="apidocSignatureSpan">tween.js.Interpolation.Utils.</span>Linear (p0, p1, t)](#apidoc.element.tween.js.Interpolation.Utils.Linear)
- description and source-code
```javascript
Linear = function (p0, p1, t) {

			return (p1 - p0) * t + p0;

		}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
