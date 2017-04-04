# api documentation for  [director (v1.2.8)](https://github.com/flatiron/director)  [![npm package](https://img.shields.io/npm/v/npmdoc-director.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-director) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-director.svg)](https://travis-ci.org/npmdoc/node-npmdoc-director)
#### A client Side/Server Side Router

[![NPM](https://nodei.co/npm/director.png?downloads=true)](https://www.npmjs.com/package/director)

[![apidoc](https://npmdoc.github.io/node-npmdoc-director/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-director_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-director/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-director/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-director/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Charlie Robbins",
        "email": "charlie.robbins@gmail.com"
    },
    "browserify": "./build/director",
    "bugs": {
        "url": "https://github.com/flatiron/director/issues"
    },
    "dependencies": {},
    "description": "A client Side/Server Side Router",
    "devDependencies": {
        "api-easy": "0.4.x",
        "codesurgeon": "https://github.com/hij1nx/codesurgeon/tarball/master",
        "colors": "1.0.x",
        "qunitjs": "1.9.x",
        "request": "2.49.x",
        "uglify-js": "2.4.x",
        "vows": "0.8.0"
    },
    "directories": {},
    "dist": {
        "shasum": "c6d9b4dd890e9aff5365183fe9cc8e73994cf2d5",
        "tarball": "https://registry.npmjs.org/director/-/director-1.2.8.tgz"
    },
    "ender": "./build/ender.js",
    "engines": {
        "node": ">= 0.8.0"
    },
    "gitHead": "b507baed25cfd38307808ea41a0d6305ee6e1ebf",
    "homepage": "https://github.com/flatiron/director",
    "keywords": [
        "URL",
        "router",
        "http",
        "cli",
        "flatiron",
        "client side",
        "ender"
    ],
    "main": "./lib/director",
    "maintainers": [
        {
            "name": "indexzero",
            "email": "charlie.robbins@gmail.com"
        },
        {
            "name": "jcrugzz",
            "email": "jcrugzz@gmail.com"
        },
        {
            "name": "swaagie",
            "email": "info@martijnswaagman.nl"
        }
    ],
    "name": "director",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/flatiron/director.git"
    },
    "scripts": {
        "test": "vows test/server/*/*-test.js --spec"
    },
    "version": "1.2.8"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module director](#apidoc.module.director)
1.  [function <span class="apidocSignatureSpan">director.</span>Router (routes)](#apidoc.element.director.Router)
1.  [function <span class="apidocSignatureSpan">director.</span>cli.Router (routes)](#apidoc.element.director.cli.Router)
1.  [function <span class="apidocSignatureSpan">director.</span>http.BadRequest (msg)](#apidoc.element.director.http.BadRequest)
1.  [function <span class="apidocSignatureSpan">director.</span>http.Forbidden (msg)](#apidoc.element.director.http.Forbidden)
1.  [function <span class="apidocSignatureSpan">director.</span>http.MethodNotAllowed (allowed)](#apidoc.element.director.http.MethodNotAllowed)
1.  [function <span class="apidocSignatureSpan">director.</span>http.NotAcceptable (accept)](#apidoc.element.director.http.NotAcceptable)
1.  [function <span class="apidocSignatureSpan">director.</span>http.NotAuthorized (msg)](#apidoc.element.director.http.NotAuthorized)
1.  [function <span class="apidocSignatureSpan">director.</span>http.NotFound (msg)](#apidoc.element.director.http.NotFound)
1.  [function <span class="apidocSignatureSpan">director.</span>http.NotImplemented (msg)](#apidoc.element.director.http.NotImplemented)
1.  [function <span class="apidocSignatureSpan">director.</span>http.NotModified ()](#apidoc.element.director.http.NotModified)
1.  [function <span class="apidocSignatureSpan">director.</span>http.Router (routes)](#apidoc.element.director.http.Router)
1.  object <span class="apidocSignatureSpan">director.</span>Router.prototype
1.  object <span class="apidocSignatureSpan">director.</span>cli
1.  object <span class="apidocSignatureSpan">director.</span>cli.Router.prototype
1.  object <span class="apidocSignatureSpan">director.</span>http
1.  object <span class="apidocSignatureSpan">director.</span>http.Router.prototype
1.  object <span class="apidocSignatureSpan">director.</span>http.Router.prototype.parsers

#### [module director.Router](#apidoc.module.director.Router)
1.  [function <span class="apidocSignatureSpan">director.</span>Router (routes)](#apidoc.element.director.Router.Router)

#### [module director.Router.prototype](#apidoc.module.director.Router.prototype)
1.  [function <span class="apidocSignatureSpan">director.Router.prototype.</span>configure (options)](#apidoc.element.director.Router.prototype.configure)
1.  [function <span class="apidocSignatureSpan">director.Router.prototype.</span>dispatch (method, path, callback)](#apidoc.element.director.Router.prototype.dispatch)
1.  [function <span class="apidocSignatureSpan">director.Router.prototype.</span>extend (methods)](#apidoc.element.director.Router.prototype.extend)
1.  [function <span class="apidocSignatureSpan">director.Router.prototype.</span>insert (method, path, route, parent)](#apidoc.element.director.Router.prototype.insert)
1.  [function <span class="apidocSignatureSpan">director.Router.prototype.</span>invoke (fns, thisArg, callback)](#apidoc.element.director.Router.prototype.invoke)
1.  [function <span class="apidocSignatureSpan">director.Router.prototype.</span>mount (routes, path)](#apidoc.element.director.Router.prototype.mount)
1.  [function <span class="apidocSignatureSpan">director.Router.prototype.</span>on (method, path, route)](#apidoc.element.director.Router.prototype.on)
1.  [function <span class="apidocSignatureSpan">director.Router.prototype.</span>param (token, matcher)](#apidoc.element.director.Router.prototype.param)
1.  [function <span class="apidocSignatureSpan">director.Router.prototype.</span>path (path, routesFn)](#apidoc.element.director.Router.prototype.path)
1.  [function <span class="apidocSignatureSpan">director.Router.prototype.</span>route (method, path, route)](#apidoc.element.director.Router.prototype.route)
1.  [function <span class="apidocSignatureSpan">director.Router.prototype.</span>runlist (fns)](#apidoc.element.director.Router.prototype.runlist)
1.  [function <span class="apidocSignatureSpan">director.Router.prototype.</span>traverse (method, path, routes, regexp, filter)](#apidoc.element.director.Router.prototype.traverse)

#### [module director.cli](#apidoc.module.director.cli)
1.  [function <span class="apidocSignatureSpan">director.cli.</span>Router (routes)](#apidoc.element.director.cli.Router)

#### [module director.cli.Router](#apidoc.module.director.cli.Router)
1.  [function <span class="apidocSignatureSpan">director.cli.</span>Router (routes)](#apidoc.element.director.cli.Router.Router)
1.  [function <span class="apidocSignatureSpan">director.cli.Router.</span>super_ (routes)](#apidoc.element.director.cli.Router.super_)

#### [module director.cli.Router.prototype](#apidoc.module.director.cli.Router.prototype)
1.  [function <span class="apidocSignatureSpan">director.cli.Router.prototype.</span>configure (options)](#apidoc.element.director.cli.Router.prototype.configure)
1.  [function <span class="apidocSignatureSpan">director.cli.Router.prototype.</span>dispatch (method, path, tty, callback)](#apidoc.element.director.cli.Router.prototype.dispatch)

#### [module director.http](#apidoc.module.director.http)
1.  [function <span class="apidocSignatureSpan">director.http.</span>BadRequest (msg)](#apidoc.element.director.http.BadRequest)
1.  [function <span class="apidocSignatureSpan">director.http.</span>Forbidden (msg)](#apidoc.element.director.http.Forbidden)
1.  [function <span class="apidocSignatureSpan">director.http.</span>MethodNotAllowed (allowed)](#apidoc.element.director.http.MethodNotAllowed)
1.  [function <span class="apidocSignatureSpan">director.http.</span>NotAcceptable (accept)](#apidoc.element.director.http.NotAcceptable)
1.  [function <span class="apidocSignatureSpan">director.http.</span>NotAuthorized (msg)](#apidoc.element.director.http.NotAuthorized)
1.  [function <span class="apidocSignatureSpan">director.http.</span>NotFound (msg)](#apidoc.element.director.http.NotFound)
1.  [function <span class="apidocSignatureSpan">director.http.</span>NotImplemented (msg)](#apidoc.element.director.http.NotImplemented)
1.  [function <span class="apidocSignatureSpan">director.http.</span>NotModified ()](#apidoc.element.director.http.NotModified)
1.  [function <span class="apidocSignatureSpan">director.http.</span>Router (routes)](#apidoc.element.director.http.Router)
1.  object <span class="apidocSignatureSpan">director.http.</span>methods

#### [module director.http.BadRequest](#apidoc.module.director.http.BadRequest)
1.  [function <span class="apidocSignatureSpan">director.http.</span>BadRequest (msg)](#apidoc.element.director.http.BadRequest.BadRequest)
1.  [function <span class="apidocSignatureSpan">director.http.BadRequest.</span>super_ ()](#apidoc.element.director.http.BadRequest.super_)

#### [module director.http.Forbidden](#apidoc.module.director.http.Forbidden)
1.  [function <span class="apidocSignatureSpan">director.http.</span>Forbidden (msg)](#apidoc.element.director.http.Forbidden.Forbidden)
1.  [function <span class="apidocSignatureSpan">director.http.Forbidden.</span>super_ ()](#apidoc.element.director.http.Forbidden.super_)

#### [module director.http.MethodNotAllowed](#apidoc.module.director.http.MethodNotAllowed)
1.  [function <span class="apidocSignatureSpan">director.http.</span>MethodNotAllowed (allowed)](#apidoc.element.director.http.MethodNotAllowed.MethodNotAllowed)
1.  [function <span class="apidocSignatureSpan">director.http.MethodNotAllowed.</span>super_ ()](#apidoc.element.director.http.MethodNotAllowed.super_)

#### [module director.http.NotAcceptable](#apidoc.module.director.http.NotAcceptable)
1.  [function <span class="apidocSignatureSpan">director.http.</span>NotAcceptable (accept)](#apidoc.element.director.http.NotAcceptable.NotAcceptable)
1.  [function <span class="apidocSignatureSpan">director.http.NotAcceptable.</span>super_ ()](#apidoc.element.director.http.NotAcceptable.super_)

#### [module director.http.NotAuthorized](#apidoc.module.director.http.NotAuthorized)
1.  [function <span class="apidocSignatureSpan">director.http.</span>NotAuthorized (msg)](#apidoc.element.director.http.NotAuthorized.NotAuthorized)
1.  [function <span class="apidocSignatureSpan">director.http.NotAuthorized.</span>super_ ()](#apidoc.element.director.http.NotAuthorized.super_)

#### [module director.http.NotFound](#apidoc.module.director.http.NotFound)
1.  [function <span class="apidocSignatureSpan">director.http.</span>NotFound (msg)](#apidoc.element.director.http.NotFound.NotFound)
1.  [function <span class="apidocSignatureSpan">director.http.NotFound.</span>super_ ()](#apidoc.element.director.http.NotFound.super_)

#### [module director.http.NotImplemented](#apidoc.module.director.http.NotImplemented)
1.  [function <span class="apidocSignatureSpan">director.http.</span>NotImplemented (msg)](#apidoc.element.director.http.NotImplemented.NotImplemented)
1.  [function <span class="apidocSignatureSpan">director.http.NotImplemented.</span>super_ ()](#apidoc.element.director.http.NotImplemented.super_)

#### [module director.http.NotModified](#apidoc.module.director.http.NotModified)
1.  [function <span class="apidocSignatureSpan">director.http.</span>NotModified ()](#apidoc.element.director.http.NotModified.NotModified)
1.  [function <span class="apidocSignatureSpan">director.http.NotModified.</span>super_ ()](#apidoc.element.director.http.NotModified.super_)

#### [module director.http.Router](#apidoc.module.director.http.Router)
1.  [function <span class="apidocSignatureSpan">director.http.</span>Router (routes)](#apidoc.element.director.http.Router.Router)
1.  [function <span class="apidocSignatureSpan">director.http.Router.</span>super_ (routes)](#apidoc.element.director.http.Router.super_)

#### [module director.http.Router.prototype](#apidoc.module.director.http.Router.prototype)
1.  [function <span class="apidocSignatureSpan">director.http.Router.prototype.</span>attach (func)](#apidoc.element.director.http.Router.prototype.attach)
1.  [function <span class="apidocSignatureSpan">director.http.Router.prototype.</span>configure (options)](#apidoc.element.director.http.Router.prototype.configure)
1.  [function <span class="apidocSignatureSpan">director.http.Router.prototype.</span>dispatch (req, res, callback)](#apidoc.element.director.http.Router.prototype.dispatch)
1.  [function <span class="apidocSignatureSpan">director.http.Router.prototype.</span>on (method, path)](#apidoc.element.director.http.Router.prototype.on)
1.  [function <span class="apidocSignatureSpan">director.http.Router.prototype.</span>parse (req)](#apidoc.element.director.http.Router.prototype.parse)
1.  object <span class="apidocSignatureSpan">director.http.Router.prototype.</span>parsers

#### [module director.http.Router.prototype.parsers](#apidoc.module.director.http.Router.prototype.parsers)



# <a name="apidoc.module.director"></a>[module director](#apidoc.module.director)

#### <a name="apidoc.element.director.Router"></a>[function <span class="apidocSignatureSpan">director.</span>Router (routes)](#apidoc.element.director.Router)
- description and source-code
```javascript
Router = function (routes) {
  this.params   = {};
  this.routes   = {};
  this.methods  = ['on', 'after', 'before'];
  this.scope    = [];
  this._methods = {};

  this.configure();
  this.mount(routes || {});
}
```
- example usage
```shell
...
  this.res.writeHead(200, { 'Content-Type': 'text/plain' })
  this.res.end('hello world');
}

//
// define a routing table.
//
var router = new director.http.Router({
  '/hello': {
    get: helloWorld
  }
});

//
// setup a server and when there is a request, dispatch the
...
```

#### <a name="apidoc.element.director.cli.Router"></a>[function <span class="apidocSignatureSpan">director.</span>cli.Router (routes)](#apidoc.element.director.cli.Router)
- description and source-code
```javascript
cli.Router = function (routes) {
  BaseRouter.call(this, routes);
  this.recurse = false;
}
```
- example usage
```shell
...

Director supports Command Line Interface routing. Routes for cli options are
based on command line input (i.e. 'process.argv') instead of a URL.

''' js
var director = require('director');

var router = new director.cli.Router();

router.on('create', function () {
  console.log('create something');
});

router.on(/destroy/, function () {
  console.log('destroy something');
...
```

#### <a name="apidoc.element.director.http.BadRequest"></a>[function <span class="apidocSignatureSpan">director.</span>http.BadRequest (msg)](#apidoc.element.director.http.BadRequest)
- description and source-code
```javascript
http.BadRequest = function (msg) {
  msg = msg || 'Bad request';

  this.status = 400;
  this.headers = {};
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.Forbidden"></a>[function <span class="apidocSignatureSpan">director.</span>http.Forbidden (msg)](#apidoc.element.director.http.Forbidden)
- description and source-code
```javascript
http.Forbidden = function (msg) {
  msg = msg || 'Not Authorized';

  this.status = 403;
  this.headers = {};
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.MethodNotAllowed"></a>[function <span class="apidocSignatureSpan">director.</span>http.MethodNotAllowed (allowed)](#apidoc.element.director.http.MethodNotAllowed)
- description and source-code
```javascript
http.MethodNotAllowed = function (allowed) {
  var msg = 'method not allowed.';

  this.status = 405;
  this.headers = { allow: allowed };
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.NotAcceptable"></a>[function <span class="apidocSignatureSpan">director.</span>http.NotAcceptable (accept)](#apidoc.element.director.http.NotAcceptable)
- description and source-code
```javascript
http.NotAcceptable = function (accept) {
  var msg = 'cannot generate "' + accept + '" response';

  this.status = 406;
  this.headers = {};
  this.message = msg;
  this.body = {
    error: msg,
    only: 'application/json'
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.NotAuthorized"></a>[function <span class="apidocSignatureSpan">director.</span>http.NotAuthorized (msg)](#apidoc.element.director.http.NotAuthorized)
- description and source-code
```javascript
http.NotAuthorized = function (msg) {
  msg = msg || 'Not Authorized';

  this.status = 401;
  this.headers = {};
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.NotFound"></a>[function <span class="apidocSignatureSpan">director.</span>http.NotFound (msg)](#apidoc.element.director.http.NotFound)
- description and source-code
```javascript
http.NotFound = function (msg) {
  msg = msg || 'Not Found';

  this.status = 404;
  this.headers = {};
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.NotImplemented"></a>[function <span class="apidocSignatureSpan">director.</span>http.NotImplemented (msg)](#apidoc.element.director.http.NotImplemented)
- description and source-code
```javascript
http.NotImplemented = function (msg) {
  msg = msg || 'Not Implemented';

  this.status = 501;
  this.headers = {};
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.NotModified"></a>[function <span class="apidocSignatureSpan">director.</span>http.NotModified ()](#apidoc.element.director.http.NotModified)
- description and source-code
```javascript
http.NotModified = function () {
  this.status = 304;
  this.options = {
    removeContentHeaders: true
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.Router"></a>[function <span class="apidocSignatureSpan">director.</span>http.Router (routes)](#apidoc.element.director.http.Router)
- description and source-code
```javascript
http.Router = function (routes) {
  //
  // ### Extend the 'Router' prototype with all of the RFC methods.
  //
  this.params   = {};
  this.routes   = {};
  this.methods  = ['on', 'after', 'before'];
  this.scope    = [];
  this._methods = {};
  this.recurse = 'forward';
  this._attach = [];

  this.extend(exports.methods.concat(['before', 'after']));
  this.configure();
  this.mount(routes || {});
}
```
- example usage
```shell
...
  this.res.writeHead(200, { 'Content-Type': 'text/plain' })
  this.res.end('hello world');
}

//
// define a routing table.
//
var router = new director.http.Router({
  '/hello': {
    get: helloWorld
  }
});

//
// setup a server and when there is a request, dispatch the
...
```



# <a name="apidoc.module.director.Router"></a>[module director.Router](#apidoc.module.director.Router)

#### <a name="apidoc.element.director.Router.Router"></a>[function <span class="apidocSignatureSpan">director.</span>Router (routes)](#apidoc.element.director.Router.Router)
- description and source-code
```javascript
Router = function (routes) {
  this.params   = {};
  this.routes   = {};
  this.methods  = ['on', 'after', 'before'];
  this.scope    = [];
  this._methods = {};

  this.configure();
  this.mount(routes || {});
}
```
- example usage
```shell
...
  this.res.writeHead(200, { 'Content-Type': 'text/plain' })
  this.res.end('hello world');
}

//
// define a routing table.
//
var router = new director.http.Router({
  '/hello': {
    get: helloWorld
  }
});

//
// setup a server and when there is a request, dispatch the
...
```



# <a name="apidoc.module.director.Router.prototype"></a>[module director.Router.prototype](#apidoc.module.director.Router.prototype)

#### <a name="apidoc.element.director.Router.prototype.configure"></a>[function <span class="apidocSignatureSpan">director.Router.prototype.</span>configure (options)](#apidoc.element.director.Router.prototype.configure)
- description and source-code
```javascript
configure = function (options) {
  options = options || {};

  for (var i = 0; i < this.methods.length; i++) {
    this._methods[this.methods[i]] = true;
  }

  this.recurse   = typeof options.recurse === 'undefined' ? this.recurse || false : options.recurse;
  this.async     = options.async     || false;
  this.delimiter = options.delimiter || '\/';
  this.strict    = typeof options.strict === 'undefined' ? true : options.strict;
  this.notfound  = options.notfound;
  this.resource  = options.resource;

  // Client only, but browser.js does not include a super implementation
  this.history     = (options.html5history && this.historySupport) || false;
  this.run_in_init = (this.history === true && options.run_handler_in_init !== false);
  this.convert_hash_in_init = (this.history === true && options.convert_hash_in_init !== false);

  //
  // TODO: Global once
  //
  this.every = {
    after: options.after || null,
    before: options.before || null,
    on: options.on || null
  };

  return this;
}
```
- example usage
```shell
...
    // instantiate the router.
    //
    var router = Router(routes);

    //
    // a global configuration setting.
    //
    router.configure({
      on: allroutes
    });

    router.init();
  });
  </script>
</head>
...
```

#### <a name="apidoc.element.director.Router.prototype.dispatch"></a>[function <span class="apidocSignatureSpan">director.Router.prototype.</span>dispatch (method, path, callback)](#apidoc.element.director.Router.prototype.dispatch)
- description and source-code
```javascript
dispatch = function (method, path, callback) {
  var self = this,
      fns = this.traverse(method, path.replace(QUERY_SEPARATOR, ''), this.routes, ''),
      invoked = this._invoked,
      after;

  this._invoked = true;
  if (!fns || fns.length === 0) {
    this.last = [];
    if (typeof this.notfound === 'function') {
      this.invoke([this.notfound], { method: method, path: path }, callback);
    }

    return false;
  }

  if (this.recurse === 'forward') {
    fns = fns.reverse();
  }

  function updateAndInvoke() {
    self.last = fns.after;
    self.invoke(self.runlist(fns), self, callback);
  }

  //
  // Builds the list of functions to invoke from this call
  // to dispatch conforming to the following order:
  //
  // 1. Global after (if any)
  // 2. After functions from the last call to dispatch
  // 3. Global before (if any)
  // 4. Global on (if any)
  // 5. Matched functions from routing table ('['before', 'on'], ['before', 'on'], ...]')
  //
  after = this.every && this.every.after
    ? [this.every.after].concat(this.last)
    : [this.last];

  if (after && after.length > 0 && invoked) {
    if (this.async) {
      this.invoke(after, this, updateAndInvoke);
    }
    else {
      this.invoke(after, this);
      updateAndInvoke();
    }

    return true;
  }

  updateAndInvoke();
  return true;
}
```
- example usage
```shell
...
});

//
// setup a server and when there is a request, dispatch the
// route that was requested in the request object.
//
var server = http.createServer(function (req, res) {
  router.dispatch(req, res, function (err) {
    if (err) {
      res.writeHead(404);
      res.end();
    }
  });
});
...
```

#### <a name="apidoc.element.director.Router.prototype.extend"></a>[function <span class="apidocSignatureSpan">director.Router.prototype.</span>extend (methods)](#apidoc.element.director.Router.prototype.extend)
- description and source-code
```javascript
extend = function (methods) {
  var self = this,
      len = methods.length,
      i;

  function extend(method) {
    self._methods[method] = true;
    self[method] = function () {
      var extra = arguments.length === 1
        ? [method, '']
        : [method];

      self.on.apply(self, extra.concat(Array.prototype.slice.call(arguments)));
    };
  }

  for (i = 0; i < len; i++) {
    extend(methods[i]);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.Router.prototype.insert"></a>[function <span class="apidocSignatureSpan">director.Router.prototype.</span>insert (method, path, route, parent)](#apidoc.element.director.Router.prototype.insert)
- description and source-code
```javascript
insert = function (method, path, route, parent) {
  var methodType,
      parentType,
      isArray,
      nested,
      part;

  path = path.filter(function (p) {
    return p && p.length > 0;
  });

  parent = parent || this.routes;
  part = path.shift();
  if (/\:|\*/.test(part) && !/\\d|\\w/.test(part)) {
    part = regifyString(part, this.params);
  }

  if (path.length > 0) {
    //
    // If this is not the last part left in the 'path'
    // (e.g. '['cities', 'new-york']') then recurse into that
    // child
    //
    parent[part] = parent[part] || {};
    return this.insert(method, path, route, parent[part]);
  }

  //
  // If there is no part and the path has been exhausted
  // and the parent is the root of the routing table,
  // then we are inserting into the root and should
  // only dive one level deep in the Routing Table.
  //
  if (!part && !path.length && parent === this.routes) {
    methodType = typeof parent[method];

    switch (methodType) {
      case 'function':
        parent[method] = [parent[method], route];
        return;
      case 'object':
        parent[method].push(route);
        return;
      case 'undefined':
        parent[method] = route;
        return;
    }

    return;
  }

  //
  // Otherwise, we are at the end of our insertion so we should
  // insert the 'route' based on the 'method' after getting the
  // 'parent' of the last 'part'.
  //
  parentType = typeof parent[part];
  isArray = Array.isArray(parent[part]);

  if (parent[part] && !isArray && parentType == 'object') {
    methodType = typeof parent[part][method];

    switch (methodType) {
      case 'function':
        parent[part][method] = [parent[part][method], route];
        return;
      case 'object':
        parent[part][method].push(route);
        return;
      case 'undefined':
        parent[part][method] = route;
        return;
    }
  }
  else if (parentType == 'undefined') {
    nested = {};
    nested[method] = route;
    parent[part] = nested;
    return;
  }

  throw new Error('Invalid route context: ' + parentType);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.Router.prototype.invoke"></a>[function <span class="apidocSignatureSpan">director.Router.prototype.</span>invoke (fns, thisArg, callback)](#apidoc.element.director.Router.prototype.invoke)
- description and source-code
```javascript
invoke = function (fns, thisArg, callback) {
  var self = this;

  var apply;
  if (this.async) {
    apply = function(fn, next){
      if (Array.isArray(fn)) {
        return _asyncEverySeries(fn, apply, next);
      }
      else if (typeof fn == 'function') {
        fn.apply(thisArg, (fns.captures || []).concat(next));
      }
    };
    _asyncEverySeries(fns, apply, function () {
      //
      // Ignore the response here. Let the routed take care
      // of themselves and eagerly return true.
      //

      if (callback) {
        callback.apply(thisArg, arguments);
      }
    });
  }
  else {
    apply = function(fn){
      if (Array.isArray(fn)) {
        return _every(fn, apply);
      }
      else if (typeof fn === 'function') {
        return fn.apply(thisArg, fns.captures || []);
      }
      else if (typeof fn === 'string' && self.resource) {
        self.resource[fn].apply(thisArg, fns.captures || []);
      }
    }
    _every(fns, apply);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.Router.prototype.mount"></a>[function <span class="apidocSignatureSpan">director.Router.prototype.</span>mount (routes, path)](#apidoc.element.director.Router.prototype.mount)
- description and source-code
```javascript
mount = function (routes, path) {
  if (!routes || typeof routes !== "object" || Array.isArray(routes)) {
    return;
  }

  var self = this;
  path = path || [];
  if (!Array.isArray(path)) {
    path = path.split(self.delimiter);
  }

  function insertOrMount(route, local) {
    var rename = route,
        parts = route.split(self.delimiter),
        routeType = typeof routes[route],
        isRoute = parts[0] === "" || !self._methods[parts[0]],
        event = isRoute ? "on" : rename;

    if (isRoute) {
      rename = rename.slice((rename.match(new RegExp('^' + self.delimiter)) || [''])[0].length);
      parts.shift();
    }

    if (isRoute && routeType === 'object' && !Array.isArray(routes[route])) {
      local = local.concat(parts);
      self.mount(routes[route], local);
      return;
    }

    if (isRoute) {
      local = local.concat(rename.split(self.delimiter));
      local = terminator(local, self.delimiter);
    }

    self.insert(event, local, routes[route]);
  }

  for (var route in routes) {
    if (routes.hasOwnProperty(route)) {
      insertOrMount(route, path.slice(0));
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.Router.prototype.on"></a>[function <span class="apidocSignatureSpan">director.Router.prototype.</span>on (method, path, route)](#apidoc.element.director.Router.prototype.on)
- description and source-code
```javascript
on = function (method, path, route) {
  var self = this;

  if (!route && typeof path == 'function') {
    //
    // If only two arguments are supplied then assume this
    // 'route' was meant to be a generic 'on'.
    //
    route = path;
    path = method;
    method = 'on';
  }

  if (Array.isArray(path)) {
    return path.forEach(function(p) {
      self.on(method, p, route);
    });
  }

  if (path.source) {
    path = path.source.replace(/\\\//ig, '/');
  }

  if (Array.isArray(method)) {
    return method.forEach(function (m) {
      self.on(m.toLowerCase(), path, route);
    });
  }

  //
  // ### Split the route up by the delimiter.
  //
  path = path.split(new RegExp(this.delimiter));

  //
  // ### Fix unterminated groups. Fixes #59
  //
  path = terminator(path, this.delimiter);

  this.insert(method, this.scope.concat(path), route);
}
```
- example usage
```shell
...
based on command line input (i.e. 'process.argv') instead of a URL.

''' js
var director = require('director');

var router = new director.cli.Router();

router.on('create', function () {
  console.log('create something');
});

router.on(/destroy/, function () {
  console.log('destroy something');
});
...
```

#### <a name="apidoc.element.director.Router.prototype.param"></a>[function <span class="apidocSignatureSpan">director.Router.prototype.</span>param (token, matcher)](#apidoc.element.director.Router.prototype.param)
- description and source-code
```javascript
param = function (token, matcher) {
  if (token[0] !== ':') {
    token = ':' + token;
  }

  var compiled = new RegExp(token, 'g');
  this.params[token] = function (str) {
    return str.replace(compiled, matcher.source || matcher);
  };
  return this;
}
```
- example usage
```shell
...
// A route could be defined using the 'userId' explicitly.
//
router.on(/([\w-_]+)/, function (userId) { });

//
// Define a shorthand for this fragment called 'userId'.
//
router.param('userId', /([\\w\\-]+)/);

//
// Now multiple routes can be defined with the same
// regular expression.
//
router.on('/anything/:userId', function (userId) { });
router.on('/something-else/:userId', function (userId) { });
...
```

#### <a name="apidoc.element.director.Router.prototype.path"></a>[function <span class="apidocSignatureSpan">director.Router.prototype.</span>path (path, routesFn)](#apidoc.element.director.Router.prototype.path)
- description and source-code
```javascript
path = function (path, routesFn) {
  var self = this,
      length = this.scope.length;

  if (path.source) {
    path = path.source.replace(/\\\//ig, '/');
  }

  //
  // ### Split the route up by the delimiter.
  //
  path = path.split(new RegExp(this.delimiter));

  //
  // ### Fix unterminated groups.
  //
  path = terminator(path, this.delimiter);
  this.scope = this.scope.concat(path);

  routesFn.call(this, this);
  this.scope.splice(length, path.length);
}
```
- example usage
```shell
...

''' js
  var router = new director.http.Router();

  //
  // Create routes inside the '/users' scope.
  //
  router.path(/\/users\/(\w+)/, function () {
//
// The 'this' context of the function passed to '.path()'
// is the Router itself.
//

this.post(function (id) {
  //
...
```

#### <a name="apidoc.element.director.Router.prototype.route"></a>[function <span class="apidocSignatureSpan">director.Router.prototype.</span>route (method, path, route)](#apidoc.element.director.Router.prototype.route)
- description and source-code
```javascript
route = function (method, path, route) {
  var self = this;

  if (!route && typeof path == 'function') {
    //
    // If only two arguments are supplied then assume this
    // 'route' was meant to be a generic 'on'.
    //
    route = path;
    path = method;
    method = 'on';
  }

  if (Array.isArray(path)) {
    return path.forEach(function(p) {
      self.on(method, p, route);
    });
  }

  if (path.source) {
    path = path.source.replace(/\\\//ig, '/');
  }

  if (Array.isArray(method)) {
    return method.forEach(function (m) {
      self.on(m.toLowerCase(), path, route);
    });
  }

  //
  // ### Split the route up by the delimiter.
  //
  path = path.split(new RegExp(this.delimiter));

  //
  // ### Fix unterminated groups. Fixes #59
  //
  path = terminator(path, this.delimiter);

  this.insert(method, this.scope.concat(path), route);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.Router.prototype.runlist"></a>[function <span class="apidocSignatureSpan">director.Router.prototype.</span>runlist (fns)](#apidoc.element.director.Router.prototype.runlist)
- description and source-code
```javascript
runlist = function (fns) {
  var runlist = this.every && this.every.before
    ? [this.every.before].concat(_flatten(fns))
    : _flatten(fns);

  if (this.every && this.every.on) {
    runlist.push(this.every.on);
  }

  runlist.captures = fns.captures;
  runlist.source = fns.source;
  return runlist;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.Router.prototype.traverse"></a>[function <span class="apidocSignatureSpan">director.Router.prototype.</span>traverse (method, path, routes, regexp, filter)](#apidoc.element.director.Router.prototype.traverse)
- description and source-code
```javascript
traverse = function (method, path, routes, regexp, filter) {
  var fns = [],
      current,
      exact,
      match,
      next,
      that;

  function filterRoutes(routes) {
    if (!filter) {
      return routes;
    }

    function deepCopy(source) {
      var result = [];
      for (var i = 0; i < source.length; i++) {
        result[i] = Array.isArray(source[i]) ? deepCopy(source[i]) : source[i];
      }
      return result;
    }

    function applyFilter(fns) {
      for (var i = fns.length - 1; i >= 0; i--) {
        if (Array.isArray(fns[i])) {
          applyFilter(fns[i]);
          if (fns[i].length === 0) {
            fns.splice(i, 1);
          }
        }
        else {
          if (!filter(fns[i])) {
            fns.splice(i, 1);
          }
        }
      }
    }

    var newRoutes = deepCopy(routes);
    newRoutes.matched = routes.matched;
    newRoutes.captures = routes.captures;
    newRoutes.after = routes.after.filter(filter);

    applyFilter(newRoutes);

    return newRoutes;
  }

  //
  // Base Case #1:
  // If we are dispatching from the root
  // then only check if the method exists.
  //
  if (path === this.delimiter && routes[method]) {
    next = [[routes.before, routes[method]].filter(Boolean)];
    next.after = [routes.after].filter(Boolean);
    next.matched = true;
    next.captures = [];
    return filterRoutes(next);
  }

  for (var r in routes) {
    //
    // We dont have an exact match, lets explore the tree
    // in a depth-first, recursive, in-order manner where
    // order is defined as:
    //
    //    ['before', 'on', '<method>', 'after']
    //
    // Remember to ignore keys (i.e. values of 'r') which
    // are actual methods (e.g. 'on', 'before', etc), but
    // which are not actual nested route (i.e. JSON literals).
    //
    if (routes.hasOwnProperty(r) && (!this._methods[r] ||
      this._methods[r] && typeof routes[r] === 'object' && !Array.isArray(routes[r]))) {
      //
      // Attempt to make an exact match for the current route
      // which is built from the 'regexp' that has been built
      // through recursive iteration.
      //
      current = exact = regexp + this.delimiter + r;

      if (!this.strict) {
        exact += '[' + this.delimiter + ']?';
      }

      match = path.match(new RegExp('^' + exact));

      if (!match) {
        //
        // If there isn't a 'match' then continue. Here, the
        // 'match' is a partial match. e.g.
        //
        //    '/foo/bar/buzz'.match(/^\/foo/)   // ['/foo']
        //    '/no-match/route'.match(/^\/foo/) // null
        //
        continue;
      }

      if (match[0] && match[0] == path && routes[r][method]) {
        //
        // ### Base case 2:
        // If we had a 'match' and the capture is the path itself,
        // then we have completed our recursion.
        //
        next = [[routes[r].before, routes[r][method]].filter(Boolean)];
        next.after = [routes[r].after].filter(Boolean);
        next.matched = true;
        next.captures = match.slice(1);

        if (this.recurse && routes === this.routes) {
          next.push([routes.before, routes.on].filter(Boolean));
          next.after = next.after.concat([routes.after].filter(Boolean));
        }

        return filterRoutes(next);
      }

      //
      // ### Recursive case:
      // If we had a match, but it is not yet an exact match then
      // attempt to continue matching against the next portion of the
      // routing table.
      //
      next = this.traverse(method, path, routes[r], current);

      //
      // 'next.matched' will be true if the depth-first search of the routing
      // table from this position was successful.
      //
      if (next.matched) {
        //
        // Build the in-place tree structure representing the function
        // in the correct order.
        //
        if (next.length > 0) {
          fns = fns.concat(next);
        }

        if (this.recurse) {
          fns.push([routes[r].before, routes[r][method]].filter(Boolean));
          next.after = next.after.concat([routes[r].after].f ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.director.cli"></a>[module director.cli](#apidoc.module.director.cli)

#### <a name="apidoc.element.director.cli.Router"></a>[function <span class="apidocSignatureSpan">director.cli.</span>Router (routes)](#apidoc.element.director.cli.Router)
- description and source-code
```javascript
Router = function (routes) {
  BaseRouter.call(this, routes);
  this.recurse = false;
}
```
- example usage
```shell
...
  this.res.writeHead(200, { 'Content-Type': 'text/plain' })
  this.res.end('hello world');
}

//
// define a routing table.
//
var router = new director.http.Router({
  '/hello': {
    get: helloWorld
  }
});

//
// setup a server and when there is a request, dispatch the
...
```



# <a name="apidoc.module.director.cli.Router"></a>[module director.cli.Router](#apidoc.module.director.cli.Router)

#### <a name="apidoc.element.director.cli.Router.Router"></a>[function <span class="apidocSignatureSpan">director.cli.</span>Router (routes)](#apidoc.element.director.cli.Router.Router)
- description and source-code
```javascript
Router = function (routes) {
  BaseRouter.call(this, routes);
  this.recurse = false;
}
```
- example usage
```shell
...
  this.res.writeHead(200, { 'Content-Type': 'text/plain' })
  this.res.end('hello world');
}

//
// define a routing table.
//
var router = new director.http.Router({
  '/hello': {
    get: helloWorld
  }
});

//
// setup a server and when there is a request, dispatch the
...
```

#### <a name="apidoc.element.director.cli.Router.super_"></a>[function <span class="apidocSignatureSpan">director.cli.Router.</span>super_ (routes)](#apidoc.element.director.cli.Router.super_)
- description and source-code
```javascript
super_ = function (routes) {
  this.params   = {};
  this.routes   = {};
  this.methods  = ['on', 'after', 'before'];
  this.scope    = [];
  this._methods = {};

  this.configure();
  this.mount(routes || {});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.director.cli.Router.prototype"></a>[module director.cli.Router.prototype](#apidoc.module.director.cli.Router.prototype)

#### <a name="apidoc.element.director.cli.Router.prototype.configure"></a>[function <span class="apidocSignatureSpan">director.cli.Router.prototype.</span>configure (options)](#apidoc.element.director.cli.Router.prototype.configure)
- description and source-code
```javascript
configure = function (options) {
  options = options || {};
  BaseRouter.prototype.configure.call(this, options);

  //
  // Delimiter must always be '\s' in CLI routing.
  // e.g. 'jitsu users create'
  //
  this.delimiter = '\\s';
  return this;
}
```
- example usage
```shell
...
    // instantiate the router.
    //
    var router = Router(routes);

    //
    // a global configuration setting.
    //
    router.configure({
      on: allroutes
    });

    router.init();
  });
  </script>
</head>
...
```

#### <a name="apidoc.element.director.cli.Router.prototype.dispatch"></a>[function <span class="apidocSignatureSpan">director.cli.Router.prototype.</span>dispatch (method, path, tty, callback)](#apidoc.element.director.cli.Router.prototype.dispatch)
- description and source-code
```javascript
dispatch = function (method, path, tty, callback) {
  //
  // Prepend a single space onto the path so that the traversal
  // algorithm will recognize it. This is because we always assume
  // that the 'path' begins with 'this.delimiter'.
  //
  path = ' ' + path;
  var fns = this.traverse(method, path, this.routes, '');
  if (!fns || fns.length === 0) {
    if (typeof this.notfound === 'function') {
      this.notfound.call({ tty: tty, cmd: path }, callback);
    }
    else if (callback) {
      callback(new Error('Could not find path: ' + path));
    }

    return false;
  }

  if (this.recurse === 'forward') {
    fns = fns.reverse();
  }

  this.invoke(this.runlist(fns), { tty: tty, cmd: path }, callback);
  return true;
}
```
- example usage
```shell
...
});

//
// setup a server and when there is a request, dispatch the
// route that was requested in the request object.
//
var server = http.createServer(function (req, res) {
  router.dispatch(req, res, function (err) {
    if (err) {
      res.writeHead(404);
      res.end();
    }
  });
});
...
```



# <a name="apidoc.module.director.http"></a>[module director.http](#apidoc.module.director.http)

#### <a name="apidoc.element.director.http.BadRequest"></a>[function <span class="apidocSignatureSpan">director.http.</span>BadRequest (msg)](#apidoc.element.director.http.BadRequest)
- description and source-code
```javascript
BadRequest = function (msg) {
  msg = msg || 'Bad request';

  this.status = 400;
  this.headers = {};
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.Forbidden"></a>[function <span class="apidocSignatureSpan">director.http.</span>Forbidden (msg)](#apidoc.element.director.http.Forbidden)
- description and source-code
```javascript
Forbidden = function (msg) {
  msg = msg || 'Not Authorized';

  this.status = 403;
  this.headers = {};
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.MethodNotAllowed"></a>[function <span class="apidocSignatureSpan">director.http.</span>MethodNotAllowed (allowed)](#apidoc.element.director.http.MethodNotAllowed)
- description and source-code
```javascript
MethodNotAllowed = function (allowed) {
  var msg = 'method not allowed.';

  this.status = 405;
  this.headers = { allow: allowed };
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.NotAcceptable"></a>[function <span class="apidocSignatureSpan">director.http.</span>NotAcceptable (accept)](#apidoc.element.director.http.NotAcceptable)
- description and source-code
```javascript
NotAcceptable = function (accept) {
  var msg = 'cannot generate "' + accept + '" response';

  this.status = 406;
  this.headers = {};
  this.message = msg;
  this.body = {
    error: msg,
    only: 'application/json'
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.NotAuthorized"></a>[function <span class="apidocSignatureSpan">director.http.</span>NotAuthorized (msg)](#apidoc.element.director.http.NotAuthorized)
- description and source-code
```javascript
NotAuthorized = function (msg) {
  msg = msg || 'Not Authorized';

  this.status = 401;
  this.headers = {};
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.NotFound"></a>[function <span class="apidocSignatureSpan">director.http.</span>NotFound (msg)](#apidoc.element.director.http.NotFound)
- description and source-code
```javascript
NotFound = function (msg) {
  msg = msg || 'Not Found';

  this.status = 404;
  this.headers = {};
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.NotImplemented"></a>[function <span class="apidocSignatureSpan">director.http.</span>NotImplemented (msg)](#apidoc.element.director.http.NotImplemented)
- description and source-code
```javascript
NotImplemented = function (msg) {
  msg = msg || 'Not Implemented';

  this.status = 501;
  this.headers = {};
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.NotModified"></a>[function <span class="apidocSignatureSpan">director.http.</span>NotModified ()](#apidoc.element.director.http.NotModified)
- description and source-code
```javascript
NotModified = function () {
  this.status = 304;
  this.options = {
    removeContentHeaders: true
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.Router"></a>[function <span class="apidocSignatureSpan">director.http.</span>Router (routes)](#apidoc.element.director.http.Router)
- description and source-code
```javascript
Router = function (routes) {
  //
  // ### Extend the 'Router' prototype with all of the RFC methods.
  //
  this.params   = {};
  this.routes   = {};
  this.methods  = ['on', 'after', 'before'];
  this.scope    = [];
  this._methods = {};
  this.recurse = 'forward';
  this._attach = [];

  this.extend(exports.methods.concat(['before', 'after']));
  this.configure();
  this.mount(routes || {});
}
```
- example usage
```shell
...
  this.res.writeHead(200, { 'Content-Type': 'text/plain' })
  this.res.end('hello world');
}

//
// define a routing table.
//
var router = new director.http.Router({
  '/hello': {
    get: helloWorld
  }
});

//
// setup a server and when there is a request, dispatch the
...
```



# <a name="apidoc.module.director.http.BadRequest"></a>[module director.http.BadRequest](#apidoc.module.director.http.BadRequest)

#### <a name="apidoc.element.director.http.BadRequest.BadRequest"></a>[function <span class="apidocSignatureSpan">director.http.</span>BadRequest (msg)](#apidoc.element.director.http.BadRequest.BadRequest)
- description and source-code
```javascript
BadRequest = function (msg) {
  msg = msg || 'Bad request';

  this.status = 400;
  this.headers = {};
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.BadRequest.super_"></a>[function <span class="apidocSignatureSpan">director.http.BadRequest.</span>super_ ()](#apidoc.element.director.http.BadRequest.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.director.http.Forbidden"></a>[module director.http.Forbidden](#apidoc.module.director.http.Forbidden)

#### <a name="apidoc.element.director.http.Forbidden.Forbidden"></a>[function <span class="apidocSignatureSpan">director.http.</span>Forbidden (msg)](#apidoc.element.director.http.Forbidden.Forbidden)
- description and source-code
```javascript
Forbidden = function (msg) {
  msg = msg || 'Not Authorized';

  this.status = 403;
  this.headers = {};
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.Forbidden.super_"></a>[function <span class="apidocSignatureSpan">director.http.Forbidden.</span>super_ ()](#apidoc.element.director.http.Forbidden.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.director.http.MethodNotAllowed"></a>[module director.http.MethodNotAllowed](#apidoc.module.director.http.MethodNotAllowed)

#### <a name="apidoc.element.director.http.MethodNotAllowed.MethodNotAllowed"></a>[function <span class="apidocSignatureSpan">director.http.</span>MethodNotAllowed (allowed)](#apidoc.element.director.http.MethodNotAllowed.MethodNotAllowed)
- description and source-code
```javascript
MethodNotAllowed = function (allowed) {
  var msg = 'method not allowed.';

  this.status = 405;
  this.headers = { allow: allowed };
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.MethodNotAllowed.super_"></a>[function <span class="apidocSignatureSpan">director.http.MethodNotAllowed.</span>super_ ()](#apidoc.element.director.http.MethodNotAllowed.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.director.http.NotAcceptable"></a>[module director.http.NotAcceptable](#apidoc.module.director.http.NotAcceptable)

#### <a name="apidoc.element.director.http.NotAcceptable.NotAcceptable"></a>[function <span class="apidocSignatureSpan">director.http.</span>NotAcceptable (accept)](#apidoc.element.director.http.NotAcceptable.NotAcceptable)
- description and source-code
```javascript
NotAcceptable = function (accept) {
  var msg = 'cannot generate "' + accept + '" response';

  this.status = 406;
  this.headers = {};
  this.message = msg;
  this.body = {
    error: msg,
    only: 'application/json'
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.NotAcceptable.super_"></a>[function <span class="apidocSignatureSpan">director.http.NotAcceptable.</span>super_ ()](#apidoc.element.director.http.NotAcceptable.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.director.http.NotAuthorized"></a>[module director.http.NotAuthorized](#apidoc.module.director.http.NotAuthorized)

#### <a name="apidoc.element.director.http.NotAuthorized.NotAuthorized"></a>[function <span class="apidocSignatureSpan">director.http.</span>NotAuthorized (msg)](#apidoc.element.director.http.NotAuthorized.NotAuthorized)
- description and source-code
```javascript
NotAuthorized = function (msg) {
  msg = msg || 'Not Authorized';

  this.status = 401;
  this.headers = {};
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.NotAuthorized.super_"></a>[function <span class="apidocSignatureSpan">director.http.NotAuthorized.</span>super_ ()](#apidoc.element.director.http.NotAuthorized.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.director.http.NotFound"></a>[module director.http.NotFound](#apidoc.module.director.http.NotFound)

#### <a name="apidoc.element.director.http.NotFound.NotFound"></a>[function <span class="apidocSignatureSpan">director.http.</span>NotFound (msg)](#apidoc.element.director.http.NotFound.NotFound)
- description and source-code
```javascript
NotFound = function (msg) {
  msg = msg || 'Not Found';

  this.status = 404;
  this.headers = {};
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.NotFound.super_"></a>[function <span class="apidocSignatureSpan">director.http.NotFound.</span>super_ ()](#apidoc.element.director.http.NotFound.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.director.http.NotImplemented"></a>[module director.http.NotImplemented](#apidoc.module.director.http.NotImplemented)

#### <a name="apidoc.element.director.http.NotImplemented.NotImplemented"></a>[function <span class="apidocSignatureSpan">director.http.</span>NotImplemented (msg)](#apidoc.element.director.http.NotImplemented.NotImplemented)
- description and source-code
```javascript
NotImplemented = function (msg) {
  msg = msg || 'Not Implemented';

  this.status = 501;
  this.headers = {};
  this.message = msg;
  this.body = { error: msg };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.NotImplemented.super_"></a>[function <span class="apidocSignatureSpan">director.http.NotImplemented.</span>super_ ()](#apidoc.element.director.http.NotImplemented.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.director.http.NotModified"></a>[module director.http.NotModified](#apidoc.module.director.http.NotModified)

#### <a name="apidoc.element.director.http.NotModified.NotModified"></a>[function <span class="apidocSignatureSpan">director.http.</span>NotModified ()](#apidoc.element.director.http.NotModified.NotModified)
- description and source-code
```javascript
NotModified = function () {
  this.status = 304;
  this.options = {
    removeContentHeaders: true
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.director.http.NotModified.super_"></a>[function <span class="apidocSignatureSpan">director.http.NotModified.</span>super_ ()](#apidoc.element.director.http.NotModified.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.director.http.Router"></a>[module director.http.Router](#apidoc.module.director.http.Router)

#### <a name="apidoc.element.director.http.Router.Router"></a>[function <span class="apidocSignatureSpan">director.http.</span>Router (routes)](#apidoc.element.director.http.Router.Router)
- description and source-code
```javascript
Router = function (routes) {
  //
  // ### Extend the 'Router' prototype with all of the RFC methods.
  //
  this.params   = {};
  this.routes   = {};
  this.methods  = ['on', 'after', 'before'];
  this.scope    = [];
  this._methods = {};
  this.recurse = 'forward';
  this._attach = [];

  this.extend(exports.methods.concat(['before', 'after']));
  this.configure();
  this.mount(routes || {});
}
```
- example usage
```shell
...
  this.res.writeHead(200, { 'Content-Type': 'text/plain' })
  this.res.end('hello world');
}

//
// define a routing table.
//
var router = new director.http.Router({
  '/hello': {
    get: helloWorld
  }
});

//
// setup a server and when there is a request, dispatch the
...
```

#### <a name="apidoc.element.director.http.Router.super_"></a>[function <span class="apidocSignatureSpan">director.http.Router.</span>super_ (routes)](#apidoc.element.director.http.Router.super_)
- description and source-code
```javascript
super_ = function (routes) {
  this.params   = {};
  this.routes   = {};
  this.methods  = ['on', 'after', 'before'];
  this.scope    = [];
  this._methods = {};

  this.configure();
  this.mount(routes || {});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.director.http.Router.prototype"></a>[module director.http.Router.prototype](#apidoc.module.director.http.Router.prototype)

#### <a name="apidoc.element.director.http.Router.prototype.attach"></a>[function <span class="apidocSignatureSpan">director.http.Router.prototype.</span>attach (func)](#apidoc.element.director.http.Router.prototype.attach)
- description and source-code
```javascript
attach = function (func) {
  this._attach.push(func);
}
```
- example usage
```shell
...
var director = require('director');

var router = new director.http.Router().configure(options);

//
// Attach properties to 'this'
//
router.attach(function () {
  this.data = [1,2,3];
});

//
// Access properties attached to 'this' in your routes!
//
router.get('/hello', function () {
...
```

#### <a name="apidoc.element.director.http.Router.prototype.configure"></a>[function <span class="apidocSignatureSpan">director.http.Router.prototype.</span>configure (options)](#apidoc.element.director.http.Router.prototype.configure)
- description and source-code
```javascript
configure = function (options) {
  options = options || {};

  // useful when using connect's bodyParser
  this.stream = options.stream || false;

  return BaseRouter.prototype.configure.call(this, options);
}
```
- example usage
```shell
...
    // instantiate the router.
    //
    var router = Router(routes);

    //
    // a global configuration setting.
    //
    router.configure({
      on: allroutes
    });

    router.init();
  });
  </script>
</head>
...
```

#### <a name="apidoc.element.director.http.Router.prototype.dispatch"></a>[function <span class="apidocSignatureSpan">director.http.Router.prototype.</span>dispatch (req, res, callback)](#apidoc.element.director.http.Router.prototype.dispatch)
- description and source-code
```javascript
dispatch = function (req, res, callback) {
  //
  // Dispatch 'HEAD' requests to 'GET'
  //
  var method = req.method === 'HEAD' ? 'get' : req.method.toLowerCase(),
      thisArg = { req: req, res: res },
      self = this,
      contentType,
      runlist,
      stream,
      error,
      fns,
      url;

  //
  // Trap bad URLs from 'decodeUri'
  //
  try { url = decodeURI(req.url.split('?', 1)[0]); }
  catch (ex) { url = null }

  if (url && this._hasAccepts) {
    contentType = req.headers['content-type'];
    fns = this.traverse(method, url, this.routes, '', function (route) {
      return !route.accept || route.accept.some(function (a) {
        return a.test(contentType);
      });
    });
  }
  else if (url) {
    fns = this.traverse(method, url, this.routes, '');
  }

  if (this._attach) {
    for (var i = 0; i < this._attach.length; i++) {
      this._attach[i].call(thisArg);
    }
  }

  if (!fns || fns.length === 0) {
    error = new exports.NotFound('Could not find path: ' + req.url);
    if (typeof this.notfound === 'function') {
      this.notfound.call(thisArg, callback);
    }
    else if (callback) {
      callback.call(thisArg, error, req, res);
    }
    return false;
  }

  if (this.recurse === 'forward') {
    fns = fns.reverse();
  }

  runlist = this.runlist(fns);
  stream  = this.stream || runlist.some(function (fn) { return fn.stream === true; });

  function parseAndInvoke() {
    error = self.parse(req);
    if (error) {
      if (callback) {
        callback.call(thisArg, error, req, res);
      }
      return false;
    }

    self.invoke(runlist, thisArg, callback);
  }

  if (!stream) {
    //
    // If there is no streaming required on any of the functions on the
    // way to 'path', then attempt to parse the fully buffered request stream
    // once it has emitted the 'end' event.
    //
    if (req.readable) {
      //
      // If the 'http.ServerRequest' is still readable, then await
      // the end event and then continue
      //
      req.once('end', parseAndInvoke);
      // Streams2 requires us to start the stream if we're not explicitly
      // reading from it.
      req.resume();
    }
    else {
      //
      // Otherwise, just parse the body now.
      //
      parseAndInvoke();
    }
  }
  else {
    this.invoke(runlist, thisArg, callback);
  }

  return true;
}
```
- example usage
```shell
...
});

//
// setup a server and when there is a request, dispatch the
// route that was requested in the request object.
//
var server = http.createServer(function (req, res) {
  router.dispatch(req, res, function (err) {
    if (err) {
      res.writeHead(404);
      res.end();
    }
  });
});
...
```

#### <a name="apidoc.element.director.http.Router.prototype.on"></a>[function <span class="apidocSignatureSpan">director.http.Router.prototype.</span>on (method, path)](#apidoc.element.director.http.Router.prototype.on)
- description and source-code
```javascript
on = function (method, path) {
  var args = Array.prototype.slice.call(arguments, 2),
      route = args.pop(),
      options = args.pop(),
      accept;

  if (options) {
    if (options.stream) {
      route.stream = true;
    }

    if (options.accept) {
      this._hasAccepts = true;
      accept = options.accept;
      route.accept = (Array.isArray(accept) ? accept : [accept]).map(function (a) {
        return typeof a === 'string' ? RegExp(a) : a;
      });
    }
  }

  if (typeof path !== 'string' && !path.source) {
    path = '';
  }

  BaseRouter.prototype.on.call(this, method, path, route);
}
```
- example usage
```shell
...
based on command line input (i.e. 'process.argv') instead of a URL.

''' js
var director = require('director');

var router = new director.cli.Router();

router.on('create', function () {
  console.log('create something');
});

router.on(/destroy/, function () {
  console.log('destroy something');
});
...
```

#### <a name="apidoc.element.director.http.Router.prototype.parse"></a>[function <span class="apidocSignatureSpan">director.http.Router.prototype.</span>parse (req)](#apidoc.element.director.http.Router.prototype.parse)
- description and source-code
```javascript
parse = function (req) {
  function mime(req) {
    var str = req.headers['content-type'] || '';
    return str.split(';')[0];
  }

  var parser = this.parsers[mime(req)],
      body;

  if (parser) {
    req.body = req.body || '';

    if (req.chunks) {
      req.chunks.forEach(function (chunk) {
        req.body += chunk;
      });
    }

    if ('string' === typeof req.body) {
      try {
        req.body = req.body && req.body.length
          ? parser(req.body)
          : {};
      }
      catch (err) {
        return new exports.BadRequest('Malformed data');
      }
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.director.http.Router.prototype.parsers"></a>[module director.http.Router.prototype.parsers](#apidoc.module.director.http.Router.prototype.parsers)



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
