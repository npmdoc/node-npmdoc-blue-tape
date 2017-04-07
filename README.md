# api documentation for  [blue-tape (v1.0.0)](https://github.com/spion/blue-tape#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-blue-tape.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-blue-tape) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-blue-tape.svg)](https://travis-ci.org/npmdoc/node-npmdoc-blue-tape)
#### Tape test runner with promise support

[![NPM](https://nodei.co/npm/blue-tape.png?downloads=true)](https://www.npmjs.com/package/blue-tape)

[![apidoc](https://npmdoc.github.io/node-npmdoc-blue-tape/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-blue-tape%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-blue-tape/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-blue-tape/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-blue-tape/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "spion"
    },
    "bin": {
        "blue-tape": "./bin/blue-tape.js"
    },
    "bugs": {
        "url": "https://github.com/spion/blue-tape/issues"
    },
    "dependencies": {
        "tape": ">=2.0.0 <5.0.0"
    },
    "description": "Tape test runner with promise support",
    "devDependencies": {
        "bl": "^1.0.0",
        "bluebird": "^2.1.2",
        "standard": "*"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "7581d04c07395c95c426b2ed6d1edb454a76b92b",
        "tarball": "https://registry.npmjs.org/blue-tape/-/blue-tape-1.0.0.tgz"
    },
    "gitHead": "b375ea85ff97480891e36588313e9787eaeaaffc",
    "homepage": "https://github.com/spion/blue-tape#readme",
    "keywords": [
        "tape",
        "bluebird",
        "promises"
    ],
    "license": "MIT",
    "main": "blue-tape.js",
    "maintainers": [
        {
            "name": "spion",
            "email": "gorgi.kosev@gmail.com"
        }
    ],
    "name": "blue-tape",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/spion/blue-tape.git"
    },
    "scripts": {
        "test": "standard && node test/index.js"
    },
    "version": "1.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module blue-tape](#apidoc.module.blue-tape)
1.  [function <span class="apidocSignatureSpan">blue-tape.</span>Test (name_, opts_, cb_)](#apidoc.element.blue-tape.Test)
1.  [function <span class="apidocSignatureSpan">blue-tape.</span>createHarness (conf_)](#apidoc.element.blue-tape.createHarness)
1.  [function <span class="apidocSignatureSpan">blue-tape.</span>createStream (opts)](#apidoc.element.blue-tape.createStream)
1.  [function <span class="apidocSignatureSpan">blue-tape.</span>getHarness (opts)](#apidoc.element.blue-tape.getHarness)
1.  [function <span class="apidocSignatureSpan">blue-tape.</span>onFinish ()](#apidoc.element.blue-tape.onFinish)
1.  [function <span class="apidocSignatureSpan">blue-tape.</span>only ()](#apidoc.element.blue-tape.only)
1.  [function <span class="apidocSignatureSpan">blue-tape.</span>skip (name_, _opts, _cb)](#apidoc.element.blue-tape.skip)
1.  [function <span class="apidocSignatureSpan">blue-tape.</span>test ()](#apidoc.element.blue-tape.test)
1.  object <span class="apidocSignatureSpan">blue-tape.</span>Test.prototype

#### [module blue-tape.Test](#apidoc.module.blue-tape.Test)
1.  [function <span class="apidocSignatureSpan">blue-tape.</span>Test (name_, opts_, cb_)](#apidoc.element.blue-tape.Test.Test)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.</span>skip (name_, _opts, _cb)](#apidoc.element.blue-tape.Test.skip)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.</span>super_ ()](#apidoc.element.blue-tape.Test.super_)

#### [module blue-tape.Test.prototype](#apidoc.module.blue-tape.Test.prototype)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>_assert (ok, opts)](#apidoc.element.blue-tape.Test.prototype._assert)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>_end (err)](#apidoc.element.blue-tape.Test.prototype._end)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>_exit ()](#apidoc.element.blue-tape.Test.prototype._exit)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>_pendingAsserts ()](#apidoc.element.blue-tape.Test.prototype._pendingAsserts)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>assert (value, msg, extra)](#apidoc.element.blue-tape.Test.prototype.assert)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>comment (msg)](#apidoc.element.blue-tape.Test.prototype.comment)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>deepEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.deepEqual)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>deepEquals (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.deepEquals)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>deepLooseEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.deepLooseEqual)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>doesNotEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.doesNotEqual)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>doesNotThrow (fn, expected, msg, extra)](#apidoc.element.blue-tape.Test.prototype.doesNotThrow)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>end (err)](#apidoc.element.blue-tape.Test.prototype.end)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>equal (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.equal)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>equals (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.equals)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>error (err, msg, extra)](#apidoc.element.blue-tape.Test.prototype.error)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>fail (msg, extra)](#apidoc.element.blue-tape.Test.prototype.fail)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>false (value, msg, extra)](#apidoc.element.blue-tape.Test.prototype.false)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>ifErr (err, msg, extra)](#apidoc.element.blue-tape.Test.prototype.ifErr)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>ifError (err, msg, extra)](#apidoc.element.blue-tape.Test.prototype.ifError)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>iferror (err, msg, extra)](#apidoc.element.blue-tape.Test.prototype.iferror)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>is (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.is)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isEqual)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isEquivalent (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isEquivalent)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isInequal (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isInequal)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isInequivalent (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isInequivalent)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isNot (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isNot)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isNotDeepEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isNotDeepEqual)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isNotDeeply (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isNotDeeply)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isNotEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isNotEqual)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isNotEquivalent (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isNotEquivalent)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>looseEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.looseEqual)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>looseEquals (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.looseEquals)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>not (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.not)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notDeepEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notDeepEqual)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notDeepLooseEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notDeepLooseEqual)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notDeeply (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notDeeply)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notEqual)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notEquals (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notEquals)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notEquivalent (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notEquivalent)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notLooseEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notLooseEqual)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notLooseEquals (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notLooseEquals)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notOk (value, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notOk)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notSame (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notSame)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notStrictEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notStrictEqual)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notStrictEquals (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notStrictEquals)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notok (value, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notok)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>ok (value, msg, extra)](#apidoc.element.blue-tape.Test.prototype.ok)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>pass (msg, extra)](#apidoc.element.blue-tape.Test.prototype.pass)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>plan (n)](#apidoc.element.blue-tape.Test.prototype.plan)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>run ()](#apidoc.element.blue-tape.Test.prototype.run)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>same (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.same)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>shouldFail (promise, expected, message, extra)](#apidoc.element.blue-tape.Test.prototype.shouldFail)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>shouldReject (promise, expected, message, extra)](#apidoc.element.blue-tape.Test.prototype.shouldReject)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>skip (msg, extra)](#apidoc.element.blue-tape.Test.prototype.skip)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>strictEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.strictEqual)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>strictEquals (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.strictEquals)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>test (name, opts, cb)](#apidoc.element.blue-tape.Test.prototype.test)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>throws (fn, expected, msg, extra)](#apidoc.element.blue-tape.Test.prototype.throws)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>timeoutAfter (ms)](#apidoc.element.blue-tape.Test.prototype.timeoutAfter)
1.  [function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>true (value, msg, extra)](#apidoc.element.blue-tape.Test.prototype.true)



# <a name="apidoc.module.blue-tape"></a>[module blue-tape](#apidoc.module.blue-tape)

#### <a name="apidoc.element.blue-tape.Test"></a>[function <span class="apidocSignatureSpan">blue-tape.</span>Test (name_, opts_, cb_)](#apidoc.element.blue-tape.Test)
- description and source-code
```javascript
function Test(name_, opts_, cb_) {
    if (! (this instanceof Test)) {
        return new Test(name_, opts_, cb_);
    }

    var args = getTestArgs(name_, opts_, cb_);

    this.readable = true;
    this.name = args.name || '(anonymous)';
    this.assertCount = 0;
    this.pendingCount = 0;
    this._skip = args.opts.skip || false;
    this._timeout = args.opts.timeout;
    this._objectPrintDepth = args.opts.objectPrintDepth || 5;
    this._plan = undefined;
    this._cb = args.cb;
    this._progeny = [];
    this._ok = true;

    for (var prop in this) {
        this[prop] = (function bind(self, val) {
            if (typeof val === 'function') {
                return function bound() {
                    return val.apply(self, arguments);
                };
            }
            else return val;
        })(this, this[prop]);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.createHarness"></a>[function <span class="apidocSignatureSpan">blue-tape.</span>createHarness (conf_)](#apidoc.element.blue-tape.createHarness)
- description and source-code
```javascript
function createHarness(conf_) {
    if (!conf_) conf_ = {};
    var results = createResult();
    if (conf_.autoclose !== false) {
        results.once('done', function () { results.close() });
    }

    var test = function (name, conf, cb) {
        var t = new Test(name, conf, cb);
        test._tests.push(t);

        (function inspectCode (st) {
            st.on('test', function sub (st_) {
                inspectCode(st_);
            });
            st.on('result', function (r) {
                if (!r.ok && typeof r !== 'string') test._exitCode = 1
            });
        })(t);

        results.push(t);
        return t;
    };
    test._results = results;

    test._tests = [];

    test.createStream = function (opts) {
        return results.createStream(opts);
    };

    test.onFinish = function (cb) {
        results.on('done', cb);
    };

    var only = false;
    test.only = function () {
        if (only) throw new Error('there can only be one only test');
        only = true;
        var t = test.apply(null, arguments);
        results.only(t);
        return t;
    };
    test._exitCode = 0;

    test.close = function () { results.close() };

    return test;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.createStream"></a>[function <span class="apidocSignatureSpan">blue-tape.</span>createStream (opts)](#apidoc.element.blue-tape.createStream)
- description and source-code
```javascript
createStream = function (opts) {
    if (!opts) opts = {};
    if (!harness) {
        var output = through();
        getHarness({ stream: output, objectMode: opts.objectMode });
        return output;
    }
    return harness.createStream(opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.getHarness"></a>[function <span class="apidocSignatureSpan">blue-tape.</span>getHarness (opts)](#apidoc.element.blue-tape.getHarness)
- description and source-code
```javascript
function getHarness(opts) {
    if (!opts) opts = {};
    opts.autoclose = !canEmitExit;
    if (!harness) harness = createExitHarness(opts);
    return harness;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.onFinish"></a>[function <span class="apidocSignatureSpan">blue-tape.</span>onFinish ()](#apidoc.element.blue-tape.onFinish)
- description and source-code
```javascript
onFinish = function () {
    return getHarness().onFinish.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.only"></a>[function <span class="apidocSignatureSpan">blue-tape.</span>only ()](#apidoc.element.blue-tape.only)
- description and source-code
```javascript
only = function () {
    return getHarness().only.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.skip"></a>[function <span class="apidocSignatureSpan">blue-tape.</span>skip (name_, _opts, _cb)](#apidoc.element.blue-tape.skip)
- description and source-code
```javascript
skip = function (name_, _opts, _cb) {
    var args = getTestArgs.apply(null, arguments);
    args.opts.skip = true;
    return Test(args.name, args.opts, args.cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.test"></a>[function <span class="apidocSignatureSpan">blue-tape.</span>test ()](#apidoc.element.blue-tape.test)
- description and source-code
```javascript
test = function () {
    return getHarness().apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blue-tape.Test"></a>[module blue-tape.Test](#apidoc.module.blue-tape.Test)

#### <a name="apidoc.element.blue-tape.Test.Test"></a>[function <span class="apidocSignatureSpan">blue-tape.</span>Test (name_, opts_, cb_)](#apidoc.element.blue-tape.Test.Test)
- description and source-code
```javascript
function Test(name_, opts_, cb_) {
    if (! (this instanceof Test)) {
        return new Test(name_, opts_, cb_);
    }

    var args = getTestArgs(name_, opts_, cb_);

    this.readable = true;
    this.name = args.name || '(anonymous)';
    this.assertCount = 0;
    this.pendingCount = 0;
    this._skip = args.opts.skip || false;
    this._timeout = args.opts.timeout;
    this._objectPrintDepth = args.opts.objectPrintDepth || 5;
    this._plan = undefined;
    this._cb = args.cb;
    this._progeny = [];
    this._ok = true;

    for (var prop in this) {
        this[prop] = (function bind(self, val) {
            if (typeof val === 'function') {
                return function bound() {
                    return val.apply(self, arguments);
                };
            }
            else return val;
        })(this, this[prop]);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.skip"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.</span>skip (name_, _opts, _cb)](#apidoc.element.blue-tape.Test.skip)
- description and source-code
```javascript
skip = function (name_, _opts, _cb) {
    var args = getTestArgs.apply(null, arguments);
    args.opts.skip = true;
    return Test(args.name, args.opts, args.cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.super_"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.</span>super_ ()](#apidoc.element.blue-tape.Test.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.blue-tape.Test.prototype"></a>[module blue-tape.Test.prototype](#apidoc.module.blue-tape.Test.prototype)

#### <a name="apidoc.element.blue-tape.Test.prototype._assert"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>_assert (ok, opts)](#apidoc.element.blue-tape.Test.prototype._assert)
- description and source-code
```javascript
function assert(ok, opts) {
    var self = this;
    var extra = opts.extra || {};

    var res = {
        id : self.assertCount ++,
        ok : Boolean(ok),
        skip : defined(extra.skip, opts.skip),
        name : defined(extra.message, opts.message, '(unnamed assert)'),
        operator : defined(extra.operator, opts.operator),
        objectPrintDepth : self._objectPrintDepth
    };
    if (has(opts, 'actual') || has(extra, 'actual')) {
        res.actual = defined(extra.actual, opts.actual);
    }
    if (has(opts, 'expected') || has(extra, 'expected')) {
        res.expected = defined(extra.expected, opts.expected);
    }
    this._ok = Boolean(this._ok && ok);

    if (!ok) {
        res.error = defined(extra.error, opts.error, new Error(res.name));
    }

    if (!ok) {
        var e = new Error('exception');
        var err = (e.stack || '').split('\n');
        var dir = path.dirname(__dirname) + path.sep;

        for (var i = 0; i < err.length; i++) {
            var m = /^[^\s]*\s*\bat\s+(.+)/.exec(err[i]);
            if (!m) {
                continue;
            }

            var s = m[1].split(/\s+/);
            var filem = /((?:\/|[A-Z]:\\)[^:\s]+:(\d+)(?::(\d+))?)/.exec(s[1]);
            if (!filem) {
                filem = /((?:\/|[A-Z]:\\)[^:\s]+:(\d+)(?::(\d+))?)/.exec(s[2]);

                if (!filem) {
                    filem = /((?:\/|[A-Z]:\\)[^:\s]+:(\d+)(?::(\d+))?)/.exec(s[3]);

                    if (!filem) {
                        continue;
                    }
                }
            }

            if (filem[1].slice(0, dir.length) === dir) {
                continue;
            }

            res.functionName = s[0];
            res.file = filem[1];
            res.line = Number(filem[2]);
            if (filem[3]) res.column = filem[3];

            res.at = m[1];
            break;
        }
    }

    self.emit('result', res);

    var pendingAsserts = self._pendingAsserts();
    if (!pendingAsserts) {
        if (extra.exiting) {
            self._end();
        } else {
            nextTick(function () {
                self._end();
            });
        }
    }

    if (!self._planError && pendingAsserts < 0) {
        self._planError = true;
        self.fail('plan != count', {
            expected : self._plan,
            actual : self._plan - pendingAsserts
        });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype._end"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>_end (err)](#apidoc.element.blue-tape.Test.prototype._end)
- description and source-code
```javascript
_end = function (err) {
    var self = this;
    if (this._progeny.length) {
        var t = this._progeny.shift();
        t.on('end', function () { self._end() });
        t.run();
        return;
    }

    if (!this.ended) this.emit('end');
    var pendingAsserts = this._pendingAsserts();
    if (!this._planError && this._plan !== undefined && pendingAsserts) {
        this._planError = true;
        this.fail('plan != count', {
            expected : this._plan,
            actual : this.assertCount
        });
    }
    this.ended = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype._exit"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>_exit ()](#apidoc.element.blue-tape.Test.prototype._exit)
- description and source-code
```javascript
_exit = function () {
    if (this._plan !== undefined &&
        !this._planError && this.assertCount !== this._plan) {
        this._planError = true;
        this.fail('plan != count', {
            expected : this._plan,
            actual : this.assertCount,
            exiting : true
        });
    }
    else if (!this.ended) {
        this.fail('test exited without ending', {
            exiting: true
        });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype._pendingAsserts"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>_pendingAsserts ()](#apidoc.element.blue-tape.Test.prototype._pendingAsserts)
- description and source-code
```javascript
_pendingAsserts = function () {
    if (this._plan === undefined) {
        return 1;
    }
    else {
        return this._plan - (this._progeny.length + this.assertCount);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.assert"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>assert (value, msg, extra)](#apidoc.element.blue-tape.Test.prototype.assert)
- description and source-code
```javascript
assert = function (value, msg, extra) {
    this._assert(value, {
        message : defined(msg, 'should be truthy'),
        operator : 'ok',
        expected : true,
        actual : value,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.comment"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>comment (msg)](#apidoc.element.blue-tape.Test.prototype.comment)
- description and source-code
```javascript
comment = function (msg) {
    var that = this;
    forEach(trim(msg).split('\n'), function (aMsg) {
        that.emit('result', trim(aMsg).replace(/^#\s*/, ''));
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.deepEqual"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>deepEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.deepEqual)
- description and source-code
```javascript
deepEqual = function (a, b, msg, extra) {
    this._assert(deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should be equivalent'),
        operator : 'deepEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.deepEquals"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>deepEquals (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.deepEquals)
- description and source-code
```javascript
deepEquals = function (a, b, msg, extra) {
    this._assert(deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should be equivalent'),
        operator : 'deepEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.deepLooseEqual"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>deepLooseEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.deepLooseEqual)
- description and source-code
```javascript
deepLooseEqual = function (a, b, msg, extra) {
    this._assert(deepEqual(a, b), {
        message : defined(msg, 'should be equivalent'),
        operator : 'deepLooseEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.doesNotEqual"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>doesNotEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.doesNotEqual)
- description and source-code
```javascript
doesNotEqual = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.doesNotThrow"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>doesNotThrow (fn, expected, msg, extra)](#apidoc.element.blue-tape.Test.prototype.doesNotThrow)
- description and source-code
```javascript
doesNotThrow = function (fn, expected, msg, extra) {
    if (typeof expected === 'string') {
        msg = expected;
        expected = undefined;
    }
    var caught = undefined;
    try {
        fn();
    }
    catch (err) {
        caught = { error : err };
    }
    this._assert(!caught, {
        message : defined(msg, 'should not throw'),
        operator : 'throws',
        actual : caught && caught.error,
        expected : expected,
        error : caught && caught.error,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.end"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>end (err)](#apidoc.element.blue-tape.Test.prototype.end)
- description and source-code
```javascript
end = function (err) {
    var self = this;
    if (arguments.length >= 1 && !!err) {
        this.ifError(err);
    }

    if (this.calledEnd) {
        this.fail('.end() called twice');
    }
    this.calledEnd = true;
    this._end();
}
```
- example usage
```shell
...

Tape with promise support.

### Usage

Same as [tape](https://github.com/substack/tape), except if you return a promise from a test,
it will be checked for errors. If there are no errors, the test will end. Otherwise the test
will fail. This means there is no need to use 't.plan()' or 't.end()'.

Also provides 't.shouldFail(promise P, optional class|regex expected, optional message)' (as
well as the alias 'shouldReject') which returns a new promise that resolves successfully if 'P'
rejects. If you provide the optional class, or regex then it additionally ensures that 'err' is
an instance of that class or that the message matches the regular expression. The behaviour is
identical to tape's 'throws' assertion.
...
```

#### <a name="apidoc.element.blue-tape.Test.prototype.equal"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>equal (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.equal)
- description and source-code
```javascript
equal = function (a, b, msg, extra) {
    this._assert(a === b, {
        message : defined(msg, 'should be equal'),
        operator : 'equal',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.equals"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>equals (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.equals)
- description and source-code
```javascript
equals = function (a, b, msg, extra) {
    this._assert(a === b, {
        message : defined(msg, 'should be equal'),
        operator : 'equal',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.error"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>error (err, msg, extra)](#apidoc.element.blue-tape.Test.prototype.error)
- description and source-code
```javascript
error = function (err, msg, extra) {
    this._assert(!err, {
        message : defined(msg, String(err)),
        operator : 'error',
        actual : err,
        extra : extra
    });
}
```
- example usage
```shell
...
  var p = this._cb && this._cb(this)
  var isPromise = checkPromise(p)
  var self = this
  if (isPromise) {
    p.then(function () {
      self.end()
    }, function (err) {
      err ? self.error(err) : self.fail(err)
      self.end()
    })
  }
} catch (err) {
  if (err) {
    this.error(err)
  } else {
...
```

#### <a name="apidoc.element.blue-tape.Test.prototype.fail"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>fail (msg, extra)](#apidoc.element.blue-tape.Test.prototype.fail)
- description and source-code
```javascript
fail = function (msg, extra) {
    this._assert(false, {
        message : msg,
        operator : 'fail',
        extra : extra
    });
}
```
- example usage
```shell
...
  var p = this._cb && this._cb(this)
  var isPromise = checkPromise(p)
  var self = this
  if (isPromise) {
    p.then(function () {
      self.end()
    }, function (err) {
      err ? self.error(err) : self.fail(err)
      self.end()
    })
  }
} catch (err) {
  if (err) {
    this.error(err)
  } else {
...
```

#### <a name="apidoc.element.blue-tape.Test.prototype.false"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>false (value, msg, extra)](#apidoc.element.blue-tape.Test.prototype.false)
- description and source-code
```javascript
false = function (value, msg, extra) {
    this._assert(!value, {
        message : defined(msg, 'should be falsy'),
        operator : 'notOk',
        expected : false,
        actual : value,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.ifErr"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>ifErr (err, msg, extra)](#apidoc.element.blue-tape.Test.prototype.ifErr)
- description and source-code
```javascript
ifErr = function (err, msg, extra) {
    this._assert(!err, {
        message : defined(msg, String(err)),
        operator : 'error',
        actual : err,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.ifError"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>ifError (err, msg, extra)](#apidoc.element.blue-tape.Test.prototype.ifError)
- description and source-code
```javascript
ifError = function (err, msg, extra) {
    this._assert(!err, {
        message : defined(msg, String(err)),
        operator : 'error',
        actual : err,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.iferror"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>iferror (err, msg, extra)](#apidoc.element.blue-tape.Test.prototype.iferror)
- description and source-code
```javascript
iferror = function (err, msg, extra) {
    this._assert(!err, {
        message : defined(msg, String(err)),
        operator : 'error',
        actual : err,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.is"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>is (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.is)
- description and source-code
```javascript
is = function (a, b, msg, extra) {
    this._assert(a === b, {
        message : defined(msg, 'should be equal'),
        operator : 'equal',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.isEqual"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isEqual)
- description and source-code
```javascript
isEqual = function (a, b, msg, extra) {
    this._assert(a === b, {
        message : defined(msg, 'should be equal'),
        operator : 'equal',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.isEquivalent"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isEquivalent (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isEquivalent)
- description and source-code
```javascript
isEquivalent = function (a, b, msg, extra) {
    this._assert(deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should be equivalent'),
        operator : 'deepEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.isInequal"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isInequal (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isInequal)
- description and source-code
```javascript
isInequal = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.isInequivalent"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isInequivalent (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isInequivalent)
- description and source-code
```javascript
isInequivalent = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should not be equivalent'),
        operator : 'notDeepEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.isNot"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isNot (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isNot)
- description and source-code
```javascript
isNot = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.isNotDeepEqual"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isNotDeepEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isNotDeepEqual)
- description and source-code
```javascript
isNotDeepEqual = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should not be equivalent'),
        operator : 'notDeepEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.isNotDeeply"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isNotDeeply (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isNotDeeply)
- description and source-code
```javascript
isNotDeeply = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should not be equivalent'),
        operator : 'notDeepEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.isNotEqual"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isNotEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isNotEqual)
- description and source-code
```javascript
isNotEqual = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.isNotEquivalent"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>isNotEquivalent (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.isNotEquivalent)
- description and source-code
```javascript
isNotEquivalent = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should not be equivalent'),
        operator : 'notDeepEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.looseEqual"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>looseEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.looseEqual)
- description and source-code
```javascript
looseEqual = function (a, b, msg, extra) {
    this._assert(deepEqual(a, b), {
        message : defined(msg, 'should be equivalent'),
        operator : 'deepLooseEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.looseEquals"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>looseEquals (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.looseEquals)
- description and source-code
```javascript
looseEquals = function (a, b, msg, extra) {
    this._assert(deepEqual(a, b), {
        message : defined(msg, 'should be equivalent'),
        operator : 'deepLooseEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.not"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>not (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.not)
- description and source-code
```javascript
not = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.notDeepEqual"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notDeepEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notDeepEqual)
- description and source-code
```javascript
notDeepEqual = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should not be equivalent'),
        operator : 'notDeepEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.notDeepLooseEqual"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notDeepLooseEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notDeepLooseEqual)
- description and source-code
```javascript
notDeepLooseEqual = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b), {
        message : defined(msg, 'should be equivalent'),
        operator : 'notDeepLooseEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.notDeeply"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notDeeply (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notDeeply)
- description and source-code
```javascript
notDeeply = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should not be equivalent'),
        operator : 'notDeepEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.notEqual"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notEqual)
- description and source-code
```javascript
notEqual = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.notEquals"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notEquals (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notEquals)
- description and source-code
```javascript
notEquals = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.notEquivalent"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notEquivalent (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notEquivalent)
- description and source-code
```javascript
notEquivalent = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should not be equivalent'),
        operator : 'notDeepEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.notLooseEqual"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notLooseEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notLooseEqual)
- description and source-code
```javascript
notLooseEqual = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b), {
        message : defined(msg, 'should be equivalent'),
        operator : 'notDeepLooseEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.notLooseEquals"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notLooseEquals (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notLooseEquals)
- description and source-code
```javascript
notLooseEquals = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b), {
        message : defined(msg, 'should be equivalent'),
        operator : 'notDeepLooseEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.notOk"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notOk (value, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notOk)
- description and source-code
```javascript
notOk = function (value, msg, extra) {
    this._assert(!value, {
        message : defined(msg, 'should be falsy'),
        operator : 'notOk',
        expected : false,
        actual : value,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.notSame"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notSame (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notSame)
- description and source-code
```javascript
notSame = function (a, b, msg, extra) {
    this._assert(!deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should not be equivalent'),
        operator : 'notDeepEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.notStrictEqual"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notStrictEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notStrictEqual)
- description and source-code
```javascript
notStrictEqual = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.notStrictEquals"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notStrictEquals (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notStrictEquals)
- description and source-code
```javascript
notStrictEquals = function (a, b, msg, extra) {
    this._assert(a !== b, {
        message : defined(msg, 'should not be equal'),
        operator : 'notEqual',
        actual : a,
        notExpected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.notok"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>notok (value, msg, extra)](#apidoc.element.blue-tape.Test.prototype.notok)
- description and source-code
```javascript
notok = function (value, msg, extra) {
    this._assert(!value, {
        message : defined(msg, 'should be falsy'),
        operator : 'notOk',
        expected : false,
        actual : value,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.ok"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>ok (value, msg, extra)](#apidoc.element.blue-tape.Test.prototype.ok)
- description and source-code
```javascript
ok = function (value, msg, extra) {
    this._assert(value, {
        message : defined(msg, 'should be truthy'),
        operator : 'ok',
        expected : true,
        actual : value,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.pass"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>pass (msg, extra)](#apidoc.element.blue-tape.Test.prototype.pass)
- description and source-code
```javascript
pass = function (msg, extra) {
    this._assert(true, {
        message : msg,
        operator : 'pass',
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.plan"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>plan (n)](#apidoc.element.blue-tape.Test.prototype.plan)
- description and source-code
```javascript
plan = function (n) {
    this._plan = n;
    this.emit('plan', n);
}
```
- example usage
```shell
...

Tape with promise support.

### Usage

Same as [tape](https://github.com/substack/tape), except if you return a promise from a test,
it will be checked for errors. If there are no errors, the test will end. Otherwise the test
will fail. This means there is no need to use 't.plan()' or 't.end()'.

Also provides 't.shouldFail(promise P, optional class|regex expected, optional message)' (as
well as the alias 'shouldReject') which returns a new promise that resolves successfully if 'P'
rejects. If you provide the optional class, or regex then it additionally ensures that 'err' is
an instance of that class or that the message matches the regular expression. The behaviour is
identical to tape's 'throws' assertion.
...
```

#### <a name="apidoc.element.blue-tape.Test.prototype.run"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>run ()](#apidoc.element.blue-tape.Test.prototype.run)
- description and source-code
```javascript
run = function () {
  if (this._skip) {
    return this.end()
  }
  this.emit('prerun')
  try {
    var p = this._cb && this._cb(this)
    var isPromise = checkPromise(p)
    var self = this
    if (isPromise) {
      p.then(function () {
        self.end()
      }, function (err) {
        err ? self.error(err) : self.fail(err)
        self.end()
      })
    }
  } catch (err) {
    if (err) {
      this.error(err)
    } else {
      this.fail(err)
    }
    this.end()
    return
  }
  this.emit('run')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.same"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>same (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.same)
- description and source-code
```javascript
same = function (a, b, msg, extra) {
    this._assert(deepEqual(a, b, { strict: true }), {
        message : defined(msg, 'should be equivalent'),
        operator : 'deepEqual',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.shouldFail"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>shouldFail (promise, expected, message, extra)](#apidoc.element.blue-tape.Test.prototype.shouldFail)
- description and source-code
```javascript
shouldFail = function (promise, expected, message, extra) {
  var self = this
  return promise.then(function () {
    self.throws(noop, expected, message, extra)
  }, function (err) {
    function f() {throw err}
    self.throws(f, expected, message, extra)
  })
}
```
- example usage
```shell
...

### Usage

Same as [tape](https://github.com/substack/tape), except if you return a promise from a test,
it will be checked for errors. If there are no errors, the test will end. Otherwise the test
will fail. This means there is no need to use 't.plan()' or 't.end()'.

Also provides 't.shouldFail(promise P, optional class|regex expected, optional message)' (as
well as the alias 'shouldReject') which returns a new promise that resolves successfully if 'P'
rejects. If you provide the optional class, or regex then it additionally ensures that 'err' is
an instance of that class or that the message matches the regular expression. The behaviour is
identical to tape's 'throws' assertion.

### Examples
...
```

#### <a name="apidoc.element.blue-tape.Test.prototype.shouldReject"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>shouldReject (promise, expected, message, extra)](#apidoc.element.blue-tape.Test.prototype.shouldReject)
- description and source-code
```javascript
shouldReject = function (promise, expected, message, extra) {
  var self = this
  return promise.then(function () {
    self.throws(noop, expected, message, extra)
  }, function (err) {
    function f() {throw err}
    self.throws(f, expected, message, extra)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.skip"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>skip (msg, extra)](#apidoc.element.blue-tape.Test.prototype.skip)
- description and source-code
```javascript
skip = function (msg, extra) {
    this._assert(true, {
        message : msg,
        operator : 'skip',
        skip : true,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.strictEqual"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>strictEqual (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.strictEqual)
- description and source-code
```javascript
strictEqual = function (a, b, msg, extra) {
    this._assert(a === b, {
        message : defined(msg, 'should be equal'),
        operator : 'equal',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.strictEquals"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>strictEquals (a, b, msg, extra)](#apidoc.element.blue-tape.Test.prototype.strictEquals)
- description and source-code
```javascript
strictEquals = function (a, b, msg, extra) {
    this._assert(a === b, {
        message : defined(msg, 'should be equal'),
        operator : 'equal',
        actual : a,
        expected : b,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.test"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>test (name, opts, cb)](#apidoc.element.blue-tape.Test.prototype.test)
- description and source-code
```javascript
test = function (name, opts, cb) {
    var self = this;
    var t = new Test(name, opts, cb);
    this._progeny.push(t);
    this.pendingCount++;
    this.emit('test', t);
    t.on('prerun', function () {
        self.assertCount++;
    })

    if (!self._pendingAsserts()) {
        nextTick(function () {
            self._end();
        });
    }

    nextTick(function() {
        if (!self._plan && self.pendingCount == self._progeny.length) {
            self._end();
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.throws"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>throws (fn, expected, msg, extra)](#apidoc.element.blue-tape.Test.prototype.throws)
- description and source-code
```javascript
throws = function (fn, expected, msg, extra) {
    if (typeof expected === 'string') {
        msg = expected;
        expected = undefined;
    }

    var caught = undefined;

    try {
        fn();
    } catch (err) {
        caught = { error : err };
        if ((err != null) && (!isEnumerable(err, 'message') || !has(err, 'message'))) {
            var message = err.message;
            delete err.message;
            err.message = message;
        }
    }

    var passed = caught;

    if (expected instanceof RegExp) {
        passed = expected.test(caught && caught.error);
        expected = String(expected);
    }

    if (typeof expected === 'function' && caught) {
        passed = caught.error instanceof expected;
        caught.error = caught.error.constructor;
    }

    this._assert(typeof fn === 'function' && passed, {
        message : defined(msg, 'should throw'),
        operator : 'throws',
        actual : caught && caught.error,
        expected : expected,
        error: !passed && caught && caught.error,
        extra : extra
    });
}
```
- example usage
```shell
...
function noop() {}

Test.prototype.shouldFail =
Test.prototype.shouldReject =
function (promise, expected, message, extra) {
  var self = this
  return promise.then(function () {
    self.throws(noop, expected, message, extra)
  }, function (err) {
    function f() {throw err}
    self.throws(f, expected, message, extra)
  })
}
...
```

#### <a name="apidoc.element.blue-tape.Test.prototype.timeoutAfter"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>timeoutAfter (ms)](#apidoc.element.blue-tape.Test.prototype.timeoutAfter)
- description and source-code
```javascript
timeoutAfter = function (ms) {
    if (!ms) throw new Error('timeoutAfter requires a timespan');
    var self = this;
    var timeout = safeSetTimeout(function() {
        self.fail('test timed out after ' + ms + 'ms');
        self.end();
    }, ms);
    this.once('end', function() {
        clearTimeout(timeout);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.blue-tape.Test.prototype.true"></a>[function <span class="apidocSignatureSpan">blue-tape.Test.prototype.</span>true (value, msg, extra)](#apidoc.element.blue-tape.Test.prototype.true)
- description and source-code
```javascript
true = function (value, msg, extra) {
    this._assert(value, {
        message : defined(msg, 'should be truthy'),
        operator : 'ok',
        expected : true,
        actual : value,
        extra : extra
    });
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
