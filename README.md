# api documentation for  [urijs (v1.18.10)](http://medialize.github.io/URI.js/)  [![npm package](https://img.shields.io/npm/v/npmdoc-urijs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-urijs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-urijs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-urijs)
#### URI.js is a Javascript library for working with URLs.

[![NPM](https://nodei.co/npm/urijs.png?downloads=true)](https://www.npmjs.com/package/urijs)

[![apidoc](https://npmdoc.github.io/node-npmdoc-urijs/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-urijs%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-urijs/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-urijs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-urijs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Rodney Rehm",
        "url": "http://rodneyrehm.de"
    },
    "bugs": {
        "url": "https://github.com/medialize/URI.js/issues"
    },
    "categories": [
        "Parsers & Compilers",
        "Utilities"
    ],
    "contributors": [
        {
            "name": "Francois-Guillaume Ribreau",
            "email": "npm@fgribreau.com",
            "url": "http://fgribreau.com"
        },
        {
            "name": "Justin Chase",
            "email": "justin.m.chase@gmail.com",
            "url": "http://justinmchase.com"
        }
    ],
    "dependencies": {},
    "description": "URI.js is a Javascript library for working with URLs.",
    "devDependencies": {
        "grunt": "~0.4.2",
        "grunt-contrib-jshint": "~0.8.0",
        "jshint-stylish": "~0.1.5"
    },
    "directories": {},
    "dist": {
        "shasum": "b94463eaba59a1a796036a467bb633c667f221ab",
        "tarball": "https://registry.npmjs.org/urijs/-/urijs-1.18.10.tgz"
    },
    "files": [
        "src/URI.js",
        "src/IPv6.js",
        "src/SecondLevelDomains.js",
        "src/punycode.js",
        "src/URITemplate.js",
        "src/jquery.URI.js",
        "src/URI.min.js",
        "src/jquery.URI.min.js",
        "src/URI.fragmentQuery.js",
        "src/URI.fragmentURI.js",
        "LICENSE.txt"
    ],
    "gitHead": "d6f596ce5dd463289ddd0ecf994503461b5f1894",
    "homepage": "http://medialize.github.io/URI.js/",
    "keywords": [
        "uri",
        "url",
        "urn",
        "uri mutation",
        "url mutation",
        "uri manipulation",
        "url manipulation",
        "uri template",
        "url template",
        "unified resource locator",
        "unified resource identifier",
        "query string",
        "RFC 3986",
        "RFC3986",
        "RFC 6570",
        "RFC6570",
        "jquery-plugin",
        "ecosystem:jquery"
    ],
    "license": "MIT",
    "main": "./src/URI",
    "maintainers": [
        {
            "name": "rodneyrehm",
            "email": "rodney.rehm@medialize.de"
        }
    ],
    "name": "urijs",
    "npmFileMap": [
        {
            "basePath": "/src/",
            "files": [
                "*.js"
            ]
        },
        {
            "basePath": "/",
            "files": [
                "LICENSE.txt"
            ]
        }
    ],
    "npmName": "urijs",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/medialize/URI.js.git"
    },
    "scripts": {},
    "title": "URI.js - Mutating URLs",
    "version": "1.18.10"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module urijs](#apidoc.module.urijs)
1.  boolean <span class="apidocSignatureSpan">urijs.</span>duplicateQueryParameters
1.  boolean <span class="apidocSignatureSpan">urijs.</span>escapeQuerySpace
1.  [function <span class="apidocSignatureSpan">urijs.</span>URITemplate (expression)](#apidoc.element.urijs.URITemplate)
1.  [function <span class="apidocSignatureSpan">urijs.</span>_parts ()](#apidoc.element.urijs._parts)
1.  [function <span class="apidocSignatureSpan">urijs.</span>addQuery (data, name, value)](#apidoc.element.urijs.addQuery)
1.  [function <span class="apidocSignatureSpan">urijs.</span>build (parts)](#apidoc.element.urijs.build)
1.  [function <span class="apidocSignatureSpan">urijs.</span>buildAuthority (parts)](#apidoc.element.urijs.buildAuthority)
1.  [function <span class="apidocSignatureSpan">urijs.</span>buildHost (parts)](#apidoc.element.urijs.buildHost)
1.  [function <span class="apidocSignatureSpan">urijs.</span>buildQuery (data, duplicateQueryParameters, escapeQuerySpace)](#apidoc.element.urijs.buildQuery)
1.  [function <span class="apidocSignatureSpan">urijs.</span>buildQueryParameter (name, value, escapeQuerySpace)](#apidoc.element.urijs.buildQueryParameter)
1.  [function <span class="apidocSignatureSpan">urijs.</span>buildUserinfo (parts)](#apidoc.element.urijs.buildUserinfo)
1.  [function <span class="apidocSignatureSpan">urijs.</span>commonPath (one, two)](#apidoc.element.urijs.commonPath)
1.  [function <span class="apidocSignatureSpan">urijs.</span>decode ()](#apidoc.element.urijs.decode)
1.  [function <span class="apidocSignatureSpan">urijs.</span>decodePath (string)](#apidoc.element.urijs.decodePath)
1.  [function <span class="apidocSignatureSpan">urijs.</span>decodePathSegment (string)](#apidoc.element.urijs.decodePathSegment)
1.  [function <span class="apidocSignatureSpan">urijs.</span>decodeQuery (string, escapeQuerySpace)](#apidoc.element.urijs.decodeQuery)
1.  [function <span class="apidocSignatureSpan">urijs.</span>decodeUrnPath (string)](#apidoc.element.urijs.decodeUrnPath)
1.  [function <span class="apidocSignatureSpan">urijs.</span>decodeUrnPathSegment (string)](#apidoc.element.urijs.decodeUrnPathSegment)
1.  [function <span class="apidocSignatureSpan">urijs.</span>encode (string)](#apidoc.element.urijs.encode)
1.  [function <span class="apidocSignatureSpan">urijs.</span>encodePathSegment (string)](#apidoc.element.urijs.encodePathSegment)
1.  [function <span class="apidocSignatureSpan">urijs.</span>encodeQuery (string, escapeQuerySpace)](#apidoc.element.urijs.encodeQuery)
1.  [function <span class="apidocSignatureSpan">urijs.</span>encodeReserved (string)](#apidoc.element.urijs.encodeReserved)
1.  [function <span class="apidocSignatureSpan">urijs.</span>encodeUrnPathSegment (string)](#apidoc.element.urijs.encodeUrnPathSegment)
1.  [function <span class="apidocSignatureSpan">urijs.</span>ensureValidHostname (v)](#apidoc.element.urijs.ensureValidHostname)
1.  [function <span class="apidocSignatureSpan">urijs.</span>expand (expression, data)](#apidoc.element.urijs.expand)
1.  [function <span class="apidocSignatureSpan">urijs.</span>getDomAttribute (node)](#apidoc.element.urijs.getDomAttribute)
1.  [function <span class="apidocSignatureSpan">urijs.</span>hasQuery (data, name, value, withinArray)](#apidoc.element.urijs.hasQuery)
1.  [function <span class="apidocSignatureSpan">urijs.</span>iso8859 ()](#apidoc.element.urijs.iso8859)
1.  [function <span class="apidocSignatureSpan">urijs.</span>joinPaths ()](#apidoc.element.urijs.joinPaths)
1.  [function <span class="apidocSignatureSpan">urijs.</span>noConflict (removeAll)](#apidoc.element.urijs.noConflict)
1.  [function <span class="apidocSignatureSpan">urijs.</span>parse (string, parts)](#apidoc.element.urijs.parse)
1.  [function <span class="apidocSignatureSpan">urijs.</span>parseAuthority (string, parts)](#apidoc.element.urijs.parseAuthority)
1.  [function <span class="apidocSignatureSpan">urijs.</span>parseHost (string, parts)](#apidoc.element.urijs.parseHost)
1.  [function <span class="apidocSignatureSpan">urijs.</span>parseQuery (string, escapeQuerySpace)](#apidoc.element.urijs.parseQuery)
1.  [function <span class="apidocSignatureSpan">urijs.</span>parseUserinfo (string, parts)](#apidoc.element.urijs.parseUserinfo)
1.  [function <span class="apidocSignatureSpan">urijs.</span>recodePath (string)](#apidoc.element.urijs.recodePath)
1.  [function <span class="apidocSignatureSpan">urijs.</span>recodeUrnPath (string)](#apidoc.element.urijs.recodeUrnPath)
1.  [function <span class="apidocSignatureSpan">urijs.</span>removeQuery (data, name, value)](#apidoc.element.urijs.removeQuery)
1.  [function <span class="apidocSignatureSpan">urijs.</span>unicode ()](#apidoc.element.urijs.unicode)
1.  [function <span class="apidocSignatureSpan">urijs.</span>withinString (string, callback, options)](#apidoc.element.urijs.withinString)
1.  object <span class="apidocSignatureSpan">urijs.</span>IPv6
1.  object <span class="apidocSignatureSpan">urijs.</span>SecondLevelDomains
1.  object <span class="apidocSignatureSpan">urijs.</span>URITemplate.prototype
1.  object <span class="apidocSignatureSpan">urijs.</span>characters
1.  object <span class="apidocSignatureSpan">urijs.</span>defaultPorts
1.  object <span class="apidocSignatureSpan">urijs.</span>domAttributes
1.  object <span class="apidocSignatureSpan">urijs.</span>findUri
1.  object <span class="apidocSignatureSpan">urijs.</span>find_uri_expression
1.  object <span class="apidocSignatureSpan">urijs.</span>idn_expression
1.  object <span class="apidocSignatureSpan">urijs.</span>invalid_hostname_characters
1.  object <span class="apidocSignatureSpan">urijs.</span>ip4_expression
1.  object <span class="apidocSignatureSpan">urijs.</span>ip6_expression
1.  object <span class="apidocSignatureSpan">urijs.</span>protocol_expression
1.  object <span class="apidocSignatureSpan">urijs.</span>punycode
1.  object <span class="apidocSignatureSpan">urijs.</span>punycode_expression
1.  string <span class="apidocSignatureSpan">urijs.</span>fragmentPrefix
1.  string <span class="apidocSignatureSpan">urijs.</span>version

#### [module urijs.IPv6](#apidoc.module.urijs.IPv6)
1.  [function <span class="apidocSignatureSpan">urijs.IPv6.</span>best (address)](#apidoc.element.urijs.IPv6.best)
1.  [function <span class="apidocSignatureSpan">urijs.IPv6.</span>noConflict ()](#apidoc.element.urijs.IPv6.noConflict)

#### [module urijs.SecondLevelDomains](#apidoc.module.urijs.SecondLevelDomains)
1.  [function <span class="apidocSignatureSpan">urijs.SecondLevelDomains.</span>get (domain)](#apidoc.element.urijs.SecondLevelDomains.get)
1.  [function <span class="apidocSignatureSpan">urijs.SecondLevelDomains.</span>has (domain)](#apidoc.element.urijs.SecondLevelDomains.has)
1.  [function <span class="apidocSignatureSpan">urijs.SecondLevelDomains.</span>is (domain)](#apidoc.element.urijs.SecondLevelDomains.is)
1.  [function <span class="apidocSignatureSpan">urijs.SecondLevelDomains.</span>noConflict ()](#apidoc.element.urijs.SecondLevelDomains.noConflict)
1.  object <span class="apidocSignatureSpan">urijs.SecondLevelDomains.</span>list

#### [module urijs.URITemplate](#apidoc.module.urijs.URITemplate)
1.  [function <span class="apidocSignatureSpan">urijs.</span>URITemplate (expression)](#apidoc.element.urijs.URITemplate.URITemplate)
1.  [function <span class="apidocSignatureSpan">urijs.URITemplate.</span>expand (expression, data, opts)](#apidoc.element.urijs.URITemplate.expand)
1.  [function <span class="apidocSignatureSpan">urijs.URITemplate.</span>expandNamed (d, options, explode, separator, length, name)](#apidoc.element.urijs.URITemplate.expandNamed)
1.  [function <span class="apidocSignatureSpan">urijs.URITemplate.</span>expandUnnamed (d, options, explode, separator, length)](#apidoc.element.urijs.URITemplate.expandUnnamed)
1.  [function <span class="apidocSignatureSpan">urijs.URITemplate.</span>noConflict ()](#apidoc.element.urijs.URITemplate.noConflict)
1.  object <span class="apidocSignatureSpan">urijs.URITemplate.</span>EXPRESSION_PATTERN
1.  object <span class="apidocSignatureSpan">urijs.URITemplate.</span>LITERAL_PATTERN
1.  object <span class="apidocSignatureSpan">urijs.URITemplate.</span>VARIABLE_NAME_PATTERN
1.  object <span class="apidocSignatureSpan">urijs.URITemplate.</span>VARIABLE_PATTERN
1.  object <span class="apidocSignatureSpan">urijs.URITemplate.</span>_cache

#### [module urijs.URITemplate.prototype](#apidoc.module.urijs.URITemplate.prototype)
1.  [function <span class="apidocSignatureSpan">urijs.URITemplate.prototype.</span>expand (data, opts)](#apidoc.element.urijs.URITemplate.prototype.expand)
1.  [function <span class="apidocSignatureSpan">urijs.URITemplate.prototype.</span>parse ()](#apidoc.element.urijs.URITemplate.prototype.parse)

#### [module urijs.punycode](#apidoc.module.urijs.punycode)
1.  [function <span class="apidocSignatureSpan">urijs.punycode.</span>decode (input)](#apidoc.element.urijs.punycode.decode)
1.  [function <span class="apidocSignatureSpan">urijs.punycode.</span>encode (input)](#apidoc.element.urijs.punycode.encode)
1.  [function <span class="apidocSignatureSpan">urijs.punycode.</span>toASCII (input)](#apidoc.element.urijs.punycode.toASCII)
1.  [function <span class="apidocSignatureSpan">urijs.punycode.</span>toUnicode (input)](#apidoc.element.urijs.punycode.toUnicode)
1.  object <span class="apidocSignatureSpan">urijs.punycode.</span>ucs2
1.  string <span class="apidocSignatureSpan">urijs.punycode.</span>version



# <a name="apidoc.module.urijs"></a>[module urijs](#apidoc.module.urijs)

#### <a name="apidoc.element.urijs.URITemplate"></a>[function <span class="apidocSignatureSpan">urijs.</span>URITemplate (expression)](#apidoc.element.urijs.URITemplate)
- description and source-code
```javascript
function URITemplate(expression) {
  // serve from cache where possible
  if (URITemplate._cache[expression]) {
    return URITemplate._cache[expression];
  }

  // Allow instantiation without the 'new' keyword
  if (!(this instanceof URITemplate)) {
    return new URITemplate(expression);
  }

  this.expression = expression;
  URITemplate._cache[expression] = this;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs._parts"></a>[function <span class="apidocSignatureSpan">urijs.</span>_parts ()](#apidoc.element.urijs._parts)
- description and source-code
```javascript
_parts = function () {
  var parts = _parts();
  parts.fragmentPrefix = URI.fragmentPrefix;
  return parts;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.addQuery"></a>[function <span class="apidocSignatureSpan">urijs.</span>addQuery (data, name, value)](#apidoc.element.urijs.addQuery)
- description and source-code
```javascript
addQuery = function (data, name, value) {
  if (typeof name === 'object') {
    for (var key in name) {
      if (hasOwn.call(name, key)) {
        URI.addQuery(data, key, name[key]);
      }
    }
  } else if (typeof name === 'string') {
    if (data[name] === undefined) {
      data[name] = value;
      return;
    } else if (typeof data[name] === 'string') {
      data[name] = [data[name]];
    }

    if (!isArray(value)) {
      value = [value];
    }

    data[name] = (data[name] || []).concat(value);
  } else {
    throw new TypeError('URI.addQuery() accepts an object, string as the name parameter');
  }
}
```
- example usage
```shell
...
url += separator + encodeURIComponent("foo") + "=" + encodeURIComponent("bar");
'''

Things are looking up with [URL](https://developer.mozilla.org/en/docs/Web/API/URL) and the [URL spec](http://url.spec.whatwg.org
/) but until we can safely rely on that API, have a look at URI.js for a clean and simple API for mutating URIs:

'''javascript
var url = new URI("http://example.org/foo?bar=baz");
url.addQuery("foo", "bar");
'''

URI.js is here to help with that.


## API Example ##
...
```

#### <a name="apidoc.element.urijs.build"></a>[function <span class="apidocSignatureSpan">urijs.</span>build (parts)](#apidoc.element.urijs.build)
- description and source-code
```javascript
build = function (parts) {
  var t = '';

  if (parts.protocol) {
    t += parts.protocol + ':';
  }

  if (!parts.urn && (t || parts.hostname)) {
    t += '//';
  }

  t += (URI.buildAuthority(parts) || '');

  if (typeof parts.path === 'string') {
    if (parts.path.charAt(0) !== '/' && typeof parts.hostname === 'string') {
      t += '/';
    }

    t += parts.path;
  }

  if (typeof parts.query === 'string' && parts.query) {
    t += '?' + parts.query;
  }

  if (typeof parts.fragment === 'string' && parts.fragment) {
    t += '#' + parts.fragment;
  }
  return t;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.buildAuthority"></a>[function <span class="apidocSignatureSpan">urijs.</span>buildAuthority (parts)](#apidoc.element.urijs.buildAuthority)
- description and source-code
```javascript
buildAuthority = function (parts) {
  return URI.buildUserinfo(parts) + URI.buildHost(parts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.buildHost"></a>[function <span class="apidocSignatureSpan">urijs.</span>buildHost (parts)](#apidoc.element.urijs.buildHost)
- description and source-code
```javascript
buildHost = function (parts) {
  var t = '';

  if (!parts.hostname) {
    return '';
  } else if (URI.ip6_expression.test(parts.hostname)) {
    t += '[' + parts.hostname + ']';
  } else {
    t += parts.hostname;
  }

  if (parts.port) {
    t += ':' + parts.port;
  }

  return t;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.buildQuery"></a>[function <span class="apidocSignatureSpan">urijs.</span>buildQuery (data, duplicateQueryParameters, escapeQuerySpace)](#apidoc.element.urijs.buildQuery)
- description and source-code
```javascript
buildQuery = function (data, duplicateQueryParameters, escapeQuerySpace) {
  // according to http://tools.ietf.org/html/rfc3986 or http://labs.apache.org/webarch/uri/rfc/rfc3986.html
  // being »-._~!$&'()*+,;=:@/?« %HEX and alnum are allowed
  // the RFC explicitly states ?/foo being a valid use case, no mention of parameter syntax!
  // URI.js treats the query string as being application/x-www-form-urlencoded
  // see http://www.w3.org/TR/REC-html40/interact/forms.html#form-content-type

  var t = '';
  var unique, key, i, length;
  for (key in data) {
    if (hasOwn.call(data, key) && key) {
      if (isArray(data[key])) {
        unique = {};
        for (i = 0, length = data[key].length; i < length; i++) {
          if (data[key][i] !== undefined && unique[data[key][i] + ''] === undefined) {
            t += '&' + URI.buildQueryParameter(key, data[key][i], escapeQuerySpace);
            if (duplicateQueryParameters !== true) {
              unique[data[key][i] + ''] = true;
            }
          }
        }
      } else if (data[key] !== undefined) {
        t += '&' + URI.buildQueryParameter(key, data[key], escapeQuerySpace);
      }
    }
  }

  return t.substring(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.buildQueryParameter"></a>[function <span class="apidocSignatureSpan">urijs.</span>buildQueryParameter (name, value, escapeQuerySpace)](#apidoc.element.urijs.buildQueryParameter)
- description and source-code
```javascript
buildQueryParameter = function (name, value, escapeQuerySpace) {
  // http://www.w3.org/TR/REC-html40/interact/forms.html#form-content-type -- application/x-www-form-urlencoded
  // don't append "=" for null values, according to http://dvcs.w3.org/hg/url/raw-file/tip/Overview.html#url-parameter-serialization
  return URI.encodeQuery(name, escapeQuerySpace) + (value !== null ? '=' + URI.encodeQuery(value, escapeQuerySpace) : '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.buildUserinfo"></a>[function <span class="apidocSignatureSpan">urijs.</span>buildUserinfo (parts)](#apidoc.element.urijs.buildUserinfo)
- description and source-code
```javascript
buildUserinfo = function (parts) {
  var t = '';

  if (parts.username) {
    t += URI.encode(parts.username);
  }

  if (parts.password) {
    t += ':' + URI.encode(parts.password);
  }

  if (t) {
    t += '@';
  }

  return t;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.commonPath"></a>[function <span class="apidocSignatureSpan">urijs.</span>commonPath (one, two)](#apidoc.element.urijs.commonPath)
- description and source-code
```javascript
commonPath = function (one, two) {
  var length = Math.min(one.length, two.length);
  var pos;

  // find first non-matching character
  for (pos = 0; pos < length; pos++) {
    if (one.charAt(pos) !== two.charAt(pos)) {
      pos--;
      break;
    }
  }

  if (pos < 1) {
    return one.charAt(0) === two.charAt(0) && one.charAt(0) === '/' ? '/' : '';
  }

  // revert to last /
  if (one.charAt(pos) !== '/' || two.charAt(pos) !== '/') {
    pos = one.substring(0, pos).lastIndexOf('/');
  }

  return one.substring(0, pos + 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.decode"></a>[function <span class="apidocSignatureSpan">urijs.</span>decode ()](#apidoc.element.urijs.decode)
- description and source-code
```javascript
function decodeURIComponent() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.decodePath"></a>[function <span class="apidocSignatureSpan">urijs.</span>decodePath (string)](#apidoc.element.urijs.decodePath)
- description and source-code
```javascript
decodePath = function (string) {
  // Why pass in names of functions, rather than the function objects themselves? The
  // definitions of some functions (but in particular, URI.decode) will occasionally change due
  // to URI.js having ISO8859 and Unicode modes. Passing in the name and getting it will ensure
  // that the functions we use here are "fresh".
  var actualCodingFunc;
  if (!_innerCodingFuncName) {
    actualCodingFunc = URI[_codingFuncName];
  } else {
    actualCodingFunc = function(string) {
      return URI[_codingFuncName](URI[_innerCodingFuncName](string));
    };
  }

  var segments = (string + '').split(_sep);

  for (var i = 0, length = segments.length; i < length; i++) {
    segments[i] = actualCodingFunc(segments[i]);
  }

  return segments.join(_sep);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.decodePathSegment"></a>[function <span class="apidocSignatureSpan">urijs.</span>decodePathSegment (string)](#apidoc.element.urijs.decodePathSegment)
- description and source-code
```javascript
decodePathSegment = function (string) {
  try {
    return URI[_part](string + '').replace(URI.characters[_group][_part].expression, function(c) {
      return URI.characters[_group][_part].map[c];
    });
  } catch (e) {
    // we're not going to mess with weird encodings,
    // give up and return the undecoded original string
    // see https://github.com/medialize/URI.js/issues/87
    // see https://github.com/medialize/URI.js/issues/92
    return string;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.decodeQuery"></a>[function <span class="apidocSignatureSpan">urijs.</span>decodeQuery (string, escapeQuerySpace)](#apidoc.element.urijs.decodeQuery)
- description and source-code
```javascript
decodeQuery = function (string, escapeQuerySpace) {
  string += '';
  if (escapeQuerySpace === undefined) {
    escapeQuerySpace = URI.escapeQuerySpace;
  }

  try {
    return URI.decode(escapeQuerySpace ? string.replace(/\+/g, '%20') : string);
  } catch(e) {
    // we're not going to mess with weird encodings,
    // give up and return the undecoded original string
    // see https://github.com/medialize/URI.js/issues/87
    // see https://github.com/medialize/URI.js/issues/92
    return string;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.decodeUrnPath"></a>[function <span class="apidocSignatureSpan">urijs.</span>decodeUrnPath (string)](#apidoc.element.urijs.decodeUrnPath)
- description and source-code
```javascript
decodeUrnPath = function (string) {
  // Why pass in names of functions, rather than the function objects themselves? The
  // definitions of some functions (but in particular, URI.decode) will occasionally change due
  // to URI.js having ISO8859 and Unicode modes. Passing in the name and getting it will ensure
  // that the functions we use here are "fresh".
  var actualCodingFunc;
  if (!_innerCodingFuncName) {
    actualCodingFunc = URI[_codingFuncName];
  } else {
    actualCodingFunc = function(string) {
      return URI[_codingFuncName](URI[_innerCodingFuncName](string));
    };
  }

  var segments = (string + '').split(_sep);

  for (var i = 0, length = segments.length; i < length; i++) {
    segments[i] = actualCodingFunc(segments[i]);
  }

  return segments.join(_sep);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.decodeUrnPathSegment"></a>[function <span class="apidocSignatureSpan">urijs.</span>decodeUrnPathSegment (string)](#apidoc.element.urijs.decodeUrnPathSegment)
- description and source-code
```javascript
decodeUrnPathSegment = function (string) {
  try {
    return URI[_part](string + '').replace(URI.characters[_group][_part].expression, function(c) {
      return URI.characters[_group][_part].map[c];
    });
  } catch (e) {
    // we're not going to mess with weird encodings,
    // give up and return the undecoded original string
    // see https://github.com/medialize/URI.js/issues/87
    // see https://github.com/medialize/URI.js/issues/92
    return string;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.encode"></a>[function <span class="apidocSignatureSpan">urijs.</span>encode (string)](#apidoc.element.urijs.encode)
- description and source-code
```javascript
function strictEncodeURIComponent(string) {
  // see https://developer.mozilla.org/en-US/docs/JavaScript/Reference/Global_Objects/encodeURIComponent
  return encodeURIComponent(string)
    .replace(/[!'()*]/g, escapeForDumbFirefox36)
    .replace(/\*/g, '%2A');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.encodePathSegment"></a>[function <span class="apidocSignatureSpan">urijs.</span>encodePathSegment (string)](#apidoc.element.urijs.encodePathSegment)
- description and source-code
```javascript
encodePathSegment = function (string) {
  try {
    return URI[_part](string + '').replace(URI.characters[_group][_part].expression, function(c) {
      return URI.characters[_group][_part].map[c];
    });
  } catch (e) {
    // we're not going to mess with weird encodings,
    // give up and return the undecoded original string
    // see https://github.com/medialize/URI.js/issues/87
    // see https://github.com/medialize/URI.js/issues/92
    return string;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.encodeQuery"></a>[function <span class="apidocSignatureSpan">urijs.</span>encodeQuery (string, escapeQuerySpace)](#apidoc.element.urijs.encodeQuery)
- description and source-code
```javascript
encodeQuery = function (string, escapeQuerySpace) {
  var escaped = URI.encode(string + '');
  if (escapeQuerySpace === undefined) {
    escapeQuerySpace = URI.escapeQuerySpace;
  }

  return escapeQuerySpace ? escaped.replace(/%20/g, '+') : escaped;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.encodeReserved"></a>[function <span class="apidocSignatureSpan">urijs.</span>encodeReserved (string)](#apidoc.element.urijs.encodeReserved)
- description and source-code
```javascript
encodeReserved = function (string) {
  try {
    return URI[_part](string + '').replace(URI.characters[_group][_part].expression, function(c) {
      return URI.characters[_group][_part].map[c];
    });
  } catch (e) {
    // we're not going to mess with weird encodings,
    // give up and return the undecoded original string
    // see https://github.com/medialize/URI.js/issues/87
    // see https://github.com/medialize/URI.js/issues/92
    return string;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.encodeUrnPathSegment"></a>[function <span class="apidocSignatureSpan">urijs.</span>encodeUrnPathSegment (string)](#apidoc.element.urijs.encodeUrnPathSegment)
- description and source-code
```javascript
encodeUrnPathSegment = function (string) {
  try {
    return URI[_part](string + '').replace(URI.characters[_group][_part].expression, function(c) {
      return URI.characters[_group][_part].map[c];
    });
  } catch (e) {
    // we're not going to mess with weird encodings,
    // give up and return the undecoded original string
    // see https://github.com/medialize/URI.js/issues/87
    // see https://github.com/medialize/URI.js/issues/92
    return string;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.ensureValidHostname"></a>[function <span class="apidocSignatureSpan">urijs.</span>ensureValidHostname (v)](#apidoc.element.urijs.ensureValidHostname)
- description and source-code
```javascript
ensureValidHostname = function (v) {
  // Theoretically URIs allow percent-encoding in Hostnames (according to RFC 3986)
  // they are not part of DNS and therefore ignored by URI.js

  if (v.match(URI.invalid_hostname_characters)) {
    // test punycode
    if (!punycode) {
      throw new TypeError('Hostname "' + v + '" contains characters other than [A-Z0-9.-] and Punycode.js is not available');
    }

    if (punycode.toASCII(v).match(URI.invalid_hostname_characters)) {
      throw new TypeError('Hostname "' + v + '" contains characters other than [A-Z0-9.-]');
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.expand"></a>[function <span class="apidocSignatureSpan">urijs.</span>expand (expression, data)](#apidoc.element.urijs.expand)
- description and source-code
```javascript
expand = function (expression, data) {
  var template = new URITemplate(expression);
  var expansion = template.expand(data);

  return new URI(expansion);
}
```
- example usage
```shell
...
URI("/foo/bar/baz.html")
  .relativeTo("/foo/bar/sub/world.html")
    // -> ../baz.html
  .absoluteTo("/foo/bar/sub/world.html");
    // -> /foo/bar/baz.html

// URI Templates
URI.expand("/foo/{dir}/{file}", {
  dir: "bar",
  file: "world.html"
});
// -> /foo/bar/world.html
'''

See the [About Page](http://medialize.github.io/URI.js/) and [API Docs](http://medialize.github.io/URI.js/docs.html) for more stuff
.
...
```

#### <a name="apidoc.element.urijs.getDomAttribute"></a>[function <span class="apidocSignatureSpan">urijs.</span>getDomAttribute (node)](#apidoc.element.urijs.getDomAttribute)
- description and source-code
```javascript
getDomAttribute = function (node) {
  if (!node || !node.nodeName) {
    return undefined;
  }

  var nodeName = node.nodeName.toLowerCase();
  // <input> should only expose src for type="image"
  if (nodeName === 'input' && node.type !== 'image') {
    return undefined;
  }

  return URI.domAttributes[nodeName];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.hasQuery"></a>[function <span class="apidocSignatureSpan">urijs.</span>hasQuery (data, name, value, withinArray)](#apidoc.element.urijs.hasQuery)
- description and source-code
```javascript
hasQuery = function (data, name, value, withinArray) {
  switch (getType(name)) {
    case 'String':
      // Nothing to do here
      break;

    case 'RegExp':
      for (var key in data) {
        if (hasOwn.call(data, key)) {
          if (name.test(key) && (value === undefined || URI.hasQuery(data, key, value))) {
            return true;
          }
        }
      }

      return false;

    case 'Object':
      for (var _key in name) {
        if (hasOwn.call(name, _key)) {
          if (!URI.hasQuery(data, _key, name[_key])) {
            return false;
          }
        }
      }

      return true;

    default:
      throw new TypeError('URI.hasQuery() accepts a string, regular expression or object as the name parameter');
  }

  switch (getType(value)) {
    case 'Undefined':
      // true if exists (but may be empty)
      return name in data; // data[name] !== undefined;

    case 'Boolean':
      // true if exists and non-empty
      var _booly = Boolean(isArray(data[name]) ? data[name].length : data[name]);
      return value === _booly;

    case 'Function':
      // allow complex comparison
      return !!value(data[name], name, data);

    case 'Array':
      if (!isArray(data[name])) {
        return false;
      }

      var op = withinArray ? arrayContains : arraysEqual;
      return op(data[name], value);

    case 'RegExp':
      if (!isArray(data[name])) {
        return Boolean(data[name] && data[name].match(value));
      }

      if (!withinArray) {
        return false;
      }

      return arrayContains(data[name], value);

    case 'Number':
      value = String(value);
<span class="apidocCodeCommentSpan">      /* falls through */
</span>    case 'String':
      if (!isArray(data[name])) {
        return data[name] === value;
      }

      if (!withinArray) {
        return false;
      }

      return arrayContains(data[name], value);

    default:
      throw new TypeError('URI.hasQuery() accepts undefined, boolean, string, number, RegExp, Function as the value parameter');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.iso8859"></a>[function <span class="apidocSignatureSpan">urijs.</span>iso8859 ()](#apidoc.element.urijs.iso8859)
- description and source-code
```javascript
iso8859 = function () {
  URI.encode = escape;
  URI.decode = unescape;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.joinPaths"></a>[function <span class="apidocSignatureSpan">urijs.</span>joinPaths ()](#apidoc.element.urijs.joinPaths)
- description and source-code
```javascript
joinPaths = function () {
  var input = [];
  var segments = [];
  var nonEmptySegments = 0;

  for (var i = 0; i < arguments.length; i++) {
    var url = new URI(arguments[i]);
    input.push(url);
    var _segments = url.segment();
    for (var s = 0; s < _segments.length; s++) {
      if (typeof _segments[s] === 'string') {
        segments.push(_segments[s]);
      }

      if (_segments[s]) {
        nonEmptySegments++;
      }
    }
  }

  if (!segments.length || !nonEmptySegments) {
    return new URI('');
  }

  var uri = new URI('').segment(segments);

  if (input[0].path() === '' || input[0].path().slice(0, 1) === '/') {
    uri.path('/' + uri.path());
  }

  return uri.normalize();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.noConflict"></a>[function <span class="apidocSignatureSpan">urijs.</span>noConflict (removeAll)](#apidoc.element.urijs.noConflict)
- description and source-code
```javascript
noConflict = function (removeAll) {
  if (removeAll) {
    var unconflicted = {
      URI: this.noConflict()
    };

    if (root.URITemplate && typeof root.URITemplate.noConflict === 'function') {
      unconflicted.URITemplate = root.URITemplate.noConflict();
    }

    if (root.IPv6 && typeof root.IPv6.noConflict === 'function') {
      unconflicted.IPv6 = root.IPv6.noConflict();
    }

    if (root.SecondLevelDomains && typeof root.SecondLevelDomains.noConflict === 'function') {
      unconflicted.SecondLevelDomains = root.SecondLevelDomains.noConflict();
    }

    return unconflicted;
  } else if (root.URI === this) {
    root.URI = _URI;
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.parse"></a>[function <span class="apidocSignatureSpan">urijs.</span>parse (string, parts)](#apidoc.element.urijs.parse)
- description and source-code
```javascript
parse = function (string, parts) {
  var pos;
  if (!parts) {
    parts = {};
  }
  // [protocol"://"[username[":"password]"@"]hostname[":"port]"/"?][path]["?"querystring]["#"fragment]

  // extract fragment
  pos = string.indexOf('#');
  if (pos > -1) {
    // escaping?
    parts.fragment = string.substring(pos + 1) || null;
    string = string.substring(0, pos);
  }

  // extract query
  pos = string.indexOf('?');
  if (pos > -1) {
    // escaping?
    parts.query = string.substring(pos + 1) || null;
    string = string.substring(0, pos);
  }

  // extract protocol
  if (string.substring(0, 2) === '//') {
    // relative-scheme
    parts.protocol = null;
    string = string.substring(2);
    // extract "user:pass@host:port"
    string = URI.parseAuthority(string, parts);
  } else {
    pos = string.indexOf(':');
    if (pos > -1) {
      parts.protocol = string.substring(0, pos) || null;
      if (parts.protocol && !parts.protocol.match(URI.protocol_expression)) {
        // : may be within the path
        parts.protocol = undefined;
      } else if (string.substring(pos + 1, pos + 3) === '//') {
        string = string.substring(pos + 3);

        // extract "user:pass@host:port"
        string = URI.parseAuthority(string, parts);
      } else {
        string = string.substring(pos + 1);
        parts.urn = true;
      }
    }
  }

  // what's left must be the path
  parts.path = string;

  // and we're done
  return parts;
}
```
- example usage
```shell
...

  // expand template through given data map
  p.expand = function(data, opts) {
var result = '';

if (!this.parts || !this.parts.length) {
  // lazilyy parse the template
  this.parse();
}

if (!(data instanceof Data)) {
  // make given data available through the
  // optimized data handling thingie
  data = new Data(data);
}
...
```

#### <a name="apidoc.element.urijs.parseAuthority"></a>[function <span class="apidocSignatureSpan">urijs.</span>parseAuthority (string, parts)](#apidoc.element.urijs.parseAuthority)
- description and source-code
```javascript
parseAuthority = function (string, parts) {
  string = URI.parseUserinfo(string, parts);
  return URI.parseHost(string, parts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.parseHost"></a>[function <span class="apidocSignatureSpan">urijs.</span>parseHost (string, parts)](#apidoc.element.urijs.parseHost)
- description and source-code
```javascript
parseHost = function (string, parts) {
  // Copy chrome, IE, opera backslash-handling behavior.
  // Back slashes before the query string get converted to forward slashes
  // See: https://github.com/joyent/node/blob/386fd24f49b0e9d1a8a076592a404168faeecc34/lib/url.js#L115-L124
  // See: https://code.google.com/p/chromium/issues/detail?id=25916
  // https://github.com/medialize/URI.js/pull/233
  string = string.replace(/\\/g, '/');

  // extract host:port
  var pos = string.indexOf('/');
  var bracketPos;
  var t;

  if (pos === -1) {
    pos = string.length;
  }

  if (string.charAt(0) === '[') {
    // IPv6 host - http://tools.ietf.org/html/draft-ietf-6man-text-addr-representation-04#section-6
    // I claim most client software breaks on IPv6 anyways. To simplify things, URI only accepts
    // IPv6+port in the format [2001:db8::1]:80 (for the time being)
    bracketPos = string.indexOf(']');
    parts.hostname = string.substring(1, bracketPos) || null;
    parts.port = string.substring(bracketPos + 2, pos) || null;
    if (parts.port === '/') {
      parts.port = null;
    }
  } else {
    var firstColon = string.indexOf(':');
    var firstSlash = string.indexOf('/');
    var nextColon = string.indexOf(':', firstColon + 1);
    if (nextColon !== -1 && (firstSlash === -1 || nextColon < firstSlash)) {
      // IPv6 host contains multiple colons - but no port
      // this notation is actually not allowed by RFC 3986, but we're a liberal parser
      parts.hostname = string.substring(0, pos) || null;
      parts.port = null;
    } else {
      t = string.substring(0, pos).split(':');
      parts.hostname = t[0] || null;
      parts.port = t[1] || null;
    }
  }

  if (parts.hostname && string.substring(pos).charAt(0) !== '/') {
    pos++;
    string = '/' + string;
  }

  return string.substring(pos) || '/';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.parseQuery"></a>[function <span class="apidocSignatureSpan">urijs.</span>parseQuery (string, escapeQuerySpace)](#apidoc.element.urijs.parseQuery)
- description and source-code
```javascript
parseQuery = function (string, escapeQuerySpace) {
  if (!string) {
    return {};
  }

  // throw out the funky business - "?"[name"="value"&"]+
  string = string.replace(/&+/g, '&').replace(/^\?*&*|&+$/g, '');

  if (!string) {
    return {};
  }

  var items = {};
  var splits = string.split('&');
  var length = splits.length;
  var v, name, value;

  for (var i = 0; i < length; i++) {
    v = splits[i].split('=');
    name = URI.decodeQuery(v.shift(), escapeQuerySpace);
    // no "=" is null according to http://dvcs.w3.org/hg/url/raw-file/tip/Overview.html#collect-url-parameters
    value = v.length ? URI.decodeQuery(v.join('='), escapeQuerySpace) : null;

    if (hasOwn.call(items, name)) {
      if (typeof items[name] === 'string' || items[name] === null) {
        items[name] = [items[name]];
      }

      items[name].push(value);
    } else {
      items[name] = value;
    }
  }

  return items;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.parseUserinfo"></a>[function <span class="apidocSignatureSpan">urijs.</span>parseUserinfo (string, parts)](#apidoc.element.urijs.parseUserinfo)
- description and source-code
```javascript
parseUserinfo = function (string, parts) {
  // extract username:password
  var firstSlash = string.indexOf('/');
  var pos = string.lastIndexOf('@', firstSlash > -1 ? firstSlash : string.length - 1);
  var t;

  // authority@ must come before /path
  if (pos > -1 && (firstSlash === -1 || pos < firstSlash)) {
    t = string.substring(0, pos).split(':');
    parts.username = t[0] ? URI.decode(t[0]) : null;
    t.shift();
    parts.password = t[0] ? URI.decode(t.join(':')) : null;
    string = string.substring(pos + 1);
  } else {
    parts.username = null;
    parts.password = null;
  }

  return string;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.recodePath"></a>[function <span class="apidocSignatureSpan">urijs.</span>recodePath (string)](#apidoc.element.urijs.recodePath)
- description and source-code
```javascript
recodePath = function (string) {
  // Why pass in names of functions, rather than the function objects themselves? The
  // definitions of some functions (but in particular, URI.decode) will occasionally change due
  // to URI.js having ISO8859 and Unicode modes. Passing in the name and getting it will ensure
  // that the functions we use here are "fresh".
  var actualCodingFunc;
  if (!_innerCodingFuncName) {
    actualCodingFunc = URI[_codingFuncName];
  } else {
    actualCodingFunc = function(string) {
      return URI[_codingFuncName](URI[_innerCodingFuncName](string));
    };
  }

  var segments = (string + '').split(_sep);

  for (var i = 0, length = segments.length; i < length; i++) {
    segments[i] = actualCodingFunc(segments[i]);
  }

  return segments.join(_sep);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.recodeUrnPath"></a>[function <span class="apidocSignatureSpan">urijs.</span>recodeUrnPath (string)](#apidoc.element.urijs.recodeUrnPath)
- description and source-code
```javascript
recodeUrnPath = function (string) {
  // Why pass in names of functions, rather than the function objects themselves? The
  // definitions of some functions (but in particular, URI.decode) will occasionally change due
  // to URI.js having ISO8859 and Unicode modes. Passing in the name and getting it will ensure
  // that the functions we use here are "fresh".
  var actualCodingFunc;
  if (!_innerCodingFuncName) {
    actualCodingFunc = URI[_codingFuncName];
  } else {
    actualCodingFunc = function(string) {
      return URI[_codingFuncName](URI[_innerCodingFuncName](string));
    };
  }

  var segments = (string + '').split(_sep);

  for (var i = 0, length = segments.length; i < length; i++) {
    segments[i] = actualCodingFunc(segments[i]);
  }

  return segments.join(_sep);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.removeQuery"></a>[function <span class="apidocSignatureSpan">urijs.</span>removeQuery (data, name, value)](#apidoc.element.urijs.removeQuery)
- description and source-code
```javascript
removeQuery = function (data, name, value) {
  var i, length, key;

  if (isArray(name)) {
    for (i = 0, length = name.length; i < length; i++) {
      data[name[i]] = undefined;
    }
  } else if (getType(name) === 'RegExp') {
    for (key in data) {
      if (name.test(key)) {
        data[key] = undefined;
      }
    }
  } else if (typeof name === 'object') {
    for (key in name) {
      if (hasOwn.call(name, key)) {
        URI.removeQuery(data, key, name[key]);
      }
    }
  } else if (typeof name === 'string') {
    if (value !== undefined) {
      if (getType(value) === 'RegExp') {
        if (!isArray(data[name]) && value.test(data[name])) {
          data[name] = undefined;
        } else {
          data[name] = filterArrayValues(data[name], value);
        }
      } else if (data[name] === String(value) && (!isArray(value) || value.length === 1)) {
        data[name] = undefined;
      } else if (isArray(data[name])) {
        data[name] = filterArrayValues(data[name], value);
      }
    } else {
      data[name] = undefined;
    }
  } else {
    throw new TypeError('URI.removeQuery() accepts an object, string, RegExp as the first parameter');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.unicode"></a>[function <span class="apidocSignatureSpan">urijs.</span>unicode ()](#apidoc.element.urijs.unicode)
- description and source-code
```javascript
unicode = function () {
  URI.encode = strictEncodeURIComponent;
  URI.decode = decodeURIComponent;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.withinString"></a>[function <span class="apidocSignatureSpan">urijs.</span>withinString (string, callback, options)](#apidoc.element.urijs.withinString)
- description and source-code
```javascript
withinString = function (string, callback, options) {
  options || (options = {});
  var _start = options.start || URI.findUri.start;
  var _end = options.end || URI.findUri.end;
  var _trim = options.trim || URI.findUri.trim;
  var _parens = options.parens || URI.findUri.parens;
  var _attributeOpen = /[a-z0-9-]=["']?$/i;

  _start.lastIndex = 0;
  while (true) {
    var match = _start.exec(string);
    if (!match) {
      break;
    }

    var start = match.index;
    if (options.ignoreHtml) {
      // attribut(e=["']?$)
      var attributeOpen = string.slice(Math.max(start - 3, 0), start);
      if (attributeOpen && _attributeOpen.test(attributeOpen)) {
        continue;
      }
    }

    var end = start + string.slice(start).search(_end);
    var slice = string.slice(start, end);
    // make sure we include well balanced parens
    var parensEnd = -1;
    while (true) {
      var parensMatch = _parens.exec(slice);
      if (!parensMatch) {
        break;
      }

      var parensMatchEnd = parensMatch.index + parensMatch[0].length;
      parensEnd = Math.max(parensEnd, parensMatchEnd);
    }

    if (parensEnd > -1) {
      slice = slice.slice(0, parensEnd) + slice.slice(parensEnd).replace(_trim, '');
    } else {
      slice = slice.replace(_trim, '');
    }

    if (slice.length <= match[0].length) {
      // the extract only contains the starting marker of a URI,
      // e.g. "www" or "http://"
      continue;
    }

    if (options.ignore && options.ignore.test(slice)) {
      continue;
    }

    end = start + slice.length;
    var result = callback(slice, start, end, string);
    if (result === undefined) {
      _start.lastIndex = end;
      continue;
    }

    result = String(result);
    string = string.slice(0, start) + result + string.slice(end);
    _start.lastIndex = start + result.length;
  }

  _start.lastIndex = 0;
  return string;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.urijs.IPv6"></a>[module urijs.IPv6](#apidoc.module.urijs.IPv6)

#### <a name="apidoc.element.urijs.IPv6.best"></a>[function <span class="apidocSignatureSpan">urijs.IPv6.</span>best (address)](#apidoc.element.urijs.IPv6.best)
- description and source-code
```javascript
function bestPresentation(address) {
  // based on:
  // Javascript to test an IPv6 address for proper format, and to
  // present the "best text representation" according to IETF Draft RFC at
  // http://tools.ietf.org/html/draft-ietf-6man-text-addr-representation-04
  // 8 Feb 2010 Rich Brown, Dartware, LLC
  // Please feel free to use this code as long as you provide a link to
  // http://www.intermapper.com
  // http://intermapper.com/support/tools/IPV6-Validator.aspx
  // http://download.dartware.com/thirdparty/ipv6validator.js

  var _address = address.toLowerCase();
  var segments = _address.split(':');
  var length = segments.length;
  var total = 8;

  // trim colons (:: or ::a:b:c… or …a:b:c::)
  if (segments[0] === '' && segments[1] === '' && segments[2] === '') {
    // must have been ::
    // remove first two items
    segments.shift();
    segments.shift();
  } else if (segments[0] === '' && segments[1] === '') {
    // must have been ::xxxx
    // remove the first item
    segments.shift();
  } else if (segments[length - 1] === '' && segments[length - 2] === '') {
    // must have been xxxx::
    segments.pop();
  }

  length = segments.length;

  // adjust total segments for IPv4 trailer
  if (segments[length - 1].indexOf('.') !== -1) {
    // found a "." which means IPv4
    total = 7;
  }

  // fill empty segments them with "0000"
  var pos;
  for (pos = 0; pos < length; pos++) {
    if (segments[pos] === '') {
      break;
    }
  }

  if (pos < total) {
    segments.splice(pos, 1, '0000');
    while (segments.length < total) {
      segments.splice(pos, 0, '0000');
    }
  }

  // strip leading zeros
  var _segments;
  for (var i = 0; i < total; i++) {
    _segments = segments[i].split('');
    for (var j = 0; j < 3 ; j++) {
      if (_segments[0] === '0' && _segments.length > 1) {
        _segments.splice(0,1);
      } else {
        break;
      }
    }

    segments[i] = _segments.join('');
  }

  // find longest sequence of zeroes and coalesce them into one segment
  var best = -1;
  var _best = 0;
  var _current = 0;
  var current = -1;
  var inzeroes = false;
  // i; already declared

  for (i = 0; i < total; i++) {
    if (inzeroes) {
      if (segments[i] === '0') {
        _current += 1;
      } else {
        inzeroes = false;
        if (_current > _best) {
          best = current;
          _best = _current;
        }
      }
    } else {
      if (segments[i] === '0') {
        inzeroes = true;
        current = i;
        _current = 1;
      }
    }
  }

  if (_current > _best) {
    best = current;
    _best = _current;
  }

  if (_best > 1) {
    segments.splice(best, _best, '');
  }

  length = segments.length;

  // assemble remaining segments
  var result = '';
  if (segments[0] === '')  {
    result = ':';
  }

  for (i = 0; i < length; i++) {
    result += segments[i];
    if (i === length - 1) {
      break;
    }

    result += ':';
  }

  if (segments[length - 1] === '') {
    result += ':';
  }

  return result;
}
```
- example usage
```shell
...
  root.IPv6 = factory(root);
}
}(this, function (root) {
'use strict';

/*
var _in = "fe80:0000:0000:0000:0204:61ff:fe9d:f156";
var _out = IPv6.best(_in);
var _expected = "fe80::204:61ff:fe9d:f156";

console.log(_in, _out, _expected, _out === _expected);
*/

// save current IPv6 variable, if any
var _IPv6 = root && root.IPv6;
...
```

#### <a name="apidoc.element.urijs.IPv6.noConflict"></a>[function <span class="apidocSignatureSpan">urijs.IPv6.</span>noConflict ()](#apidoc.element.urijs.IPv6.noConflict)
- description and source-code
```javascript
function noConflict() {
<span class="apidocCodeCommentSpan">  /*jshint validthis: true */
</span>  if (root.IPv6 === this) {
    root.IPv6 = _IPv6;
  }

  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.urijs.SecondLevelDomains"></a>[module urijs.SecondLevelDomains](#apidoc.module.urijs.SecondLevelDomains)

#### <a name="apidoc.element.urijs.SecondLevelDomains.get"></a>[function <span class="apidocSignatureSpan">urijs.SecondLevelDomains.</span>get (domain)](#apidoc.element.urijs.SecondLevelDomains.get)
- description and source-code
```javascript
get = function (domain) {
  var tldOffset = domain.lastIndexOf('.');
  if (tldOffset <= 0 || tldOffset >= (domain.length-1)) {
    return null;
  }
  var sldOffset = domain.lastIndexOf('.', tldOffset-1);
  if (sldOffset <= 0 || sldOffset >= (tldOffset-1)) {
    return null;
  }
  var sldList = SLD.list[domain.slice(tldOffset+1)];
  if (!sldList) {
    return null;
  }
  if (sldList.indexOf(' ' + domain.slice(sldOffset+1, tldOffset) + ' ') < 0) {
    return null;
  }
  return domain.slice(sldOffset+1);
}
```
- example usage
```shell
...
var variables = expression.variables;
// result buffer for evaluating the expression
var buffer = [];
var d, variable, i;

for (i = 0; (variable = variables[i]); i++) {
  // fetch simplified data source
  d = data.get(variable.name);
  if (d.type === 0 && opts && opts.strict) {
      throw new Error('Missing expansion value for variable "' + variable.name + '"');
  }
  if (!d.val.length) {
    if (d.type) {
      // empty variables (empty string)
      // still lead to a separator being appended!
...
```

#### <a name="apidoc.element.urijs.SecondLevelDomains.has"></a>[function <span class="apidocSignatureSpan">urijs.SecondLevelDomains.</span>has (domain)](#apidoc.element.urijs.SecondLevelDomains.has)
- description and source-code
```javascript
has = function (domain) {
  var tldOffset = domain.lastIndexOf('.');
  if (tldOffset <= 0 || tldOffset >= (domain.length-1)) {
    return false;
  }
  var sldOffset = domain.lastIndexOf('.', tldOffset-1);
  if (sldOffset <= 0 || sldOffset >= (tldOffset-1)) {
    return false;
  }
  var sldList = SLD.list[domain.slice(tldOffset+1)];
  if (!sldList) {
    return false;
  }
  return sldList.indexOf(' ' + domain.slice(sldOffset+1, tldOffset) + ' ') >= 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.SecondLevelDomains.is"></a>[function <span class="apidocSignatureSpan">urijs.SecondLevelDomains.</span>is (domain)](#apidoc.element.urijs.SecondLevelDomains.is)
- description and source-code
```javascript
is = function (domain) {
  var tldOffset = domain.lastIndexOf('.');
  if (tldOffset <= 0 || tldOffset >= (domain.length-1)) {
    return false;
  }
  var sldOffset = domain.lastIndexOf('.', tldOffset-1);
  if (sldOffset >= 0) {
    return false;
  }
  var sldList = SLD.list[domain.slice(tldOffset+1)];
  if (!sldList) {
    return false;
  }
  return sldList.indexOf(' ' + domain.slice(0, tldOffset) + ' ') >= 0;
}
```
- example usage
```shell
...
require.config({
  paths: {
    urijs: 'where-you-put-uri.js/src'
  }
});

require(['urijs/URI'], function(URI) {
  console.log("URI.js and dependencies: ", URI("//amazon.co.uk").is('sld') ? 'loaded' : 'failed');
});
require(['urijs/URITemplate'], function(URITemplate) {
  console.log("URITemplate.js and dependencies: ", URITemplate._cache ? 'loaded' : 'failed');
});
'''

## Minify ##
...
```

#### <a name="apidoc.element.urijs.SecondLevelDomains.noConflict"></a>[function <span class="apidocSignatureSpan">urijs.SecondLevelDomains.</span>noConflict ()](#apidoc.element.urijs.SecondLevelDomains.noConflict)
- description and source-code
```javascript
noConflict = function (){
  if (root.SecondLevelDomains === this) {
    root.SecondLevelDomains = _SecondLevelDomains;
  }
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.urijs.URITemplate"></a>[module urijs.URITemplate](#apidoc.module.urijs.URITemplate)

#### <a name="apidoc.element.urijs.URITemplate.URITemplate"></a>[function <span class="apidocSignatureSpan">urijs.</span>URITemplate (expression)](#apidoc.element.urijs.URITemplate.URITemplate)
- description and source-code
```javascript
function URITemplate(expression) {
  // serve from cache where possible
  if (URITemplate._cache[expression]) {
    return URITemplate._cache[expression];
  }

  // Allow instantiation without the 'new' keyword
  if (!(this instanceof URITemplate)) {
    return new URITemplate(expression);
  }

  this.expression = expression;
  URITemplate._cache[expression] = this;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.URITemplate.expand"></a>[function <span class="apidocSignatureSpan">urijs.URITemplate.</span>expand (expression, data, opts)](#apidoc.element.urijs.URITemplate.expand)
- description and source-code
```javascript
expand = function (expression, data, opts) {
  // container for defined options for the given operator
  var options = operators[expression.operator];
  // expansion type (include keys or not)
  var type = options.named ? 'Named' : 'Unnamed';
  // list of variables within the expression
  var variables = expression.variables;
  // result buffer for evaluating the expression
  var buffer = [];
  var d, variable, i;

  for (i = 0; (variable = variables[i]); i++) {
    // fetch simplified data source
    d = data.get(variable.name);
    if (d.type === 0 && opts && opts.strict) {
        throw new Error('Missing expansion value for variable "' + variable.name + '"');
    }
    if (!d.val.length) {
      if (d.type) {
        // empty variables (empty string)
        // still lead to a separator being appended!
        buffer.push('');
      }
      // no data, no action
      continue;
    }

    if (d.type > 1 && variable.maxlength) {
      // composite variable cannot specify maxlength
      throw new Error('Invalid expression: Prefix modifier not applicable to variable "' + variable.name + '"');
    }

    // expand the given variable
    buffer.push(URITemplate['expand' + type](
      d,
      options,
      variable.explode,
      variable.explode && options.separator || ',',
      variable.maxlength,
      variable.name
    ));
  }

  if (buffer.length) {
    return options.prefix + buffer.join(options.separator);
  } else {
    // prefix is not prepended for empty expressions
    return '';
  }
}
```
- example usage
```shell
...
URI("/foo/bar/baz.html")
  .relativeTo("/foo/bar/sub/world.html")
    // -> ../baz.html
  .absoluteTo("/foo/bar/sub/world.html");
    // -> /foo/bar/baz.html

// URI Templates
URI.expand("/foo/{dir}/{file}", {
  dir: "bar",
  file: "world.html"
});
// -> /foo/bar/world.html
'''

See the [About Page](http://medialize.github.io/URI.js/) and [API Docs](http://medialize.github.io/URI.js/docs.html) for more stuff
.
...
```

#### <a name="apidoc.element.urijs.URITemplate.expandNamed"></a>[function <span class="apidocSignatureSpan">urijs.URITemplate.</span>expandNamed (d, options, explode, separator, length, name)](#apidoc.element.urijs.URITemplate.expandNamed)
- description and source-code
```javascript
expandNamed = function (d, options, explode, separator, length, name) {
  // variable result buffer
  var result = '';
  // peformance crap
  var encode = options.encode;
  var empty_name_separator = options.empty_name_separator;
  // flag noting if values are already encoded
  var _encode = !d[encode].length;
  // key for named expansion
  var _name = d.type === 2 ? '': URI[encode](name);
  var _value, i, l;

  // for each found value
  for (i = 0, l = d.val.length; i < l; i++) {
    if (length) {
      // maxlength must be determined before encoding can happen
      _value = URI[encode](d.val[i][1].substring(0, length));
      if (d.type === 2) {
        // apply maxlength to keys of objects as well
        _name = URI[encode](d.val[i][0].substring(0, length));
      }
    } else if (_encode) {
      // encode value
      _value = URI[encode](d.val[i][1]);
      if (d.type === 2) {
        // encode name and cache encoded value
        _name = URI[encode](d.val[i][0]);
        d[encode].push([_name, _value]);
      } else {
        // cache encoded value
        d[encode].push([undefined, _value]);
      }
    } else {
      // values are already encoded and can be pulled from cache
      _value = d[encode][i][1];
      if (d.type === 2) {
        _name = d[encode][i][0];
      }
    }

    if (result) {
      // unless we're the first value, prepend the separator
      result += separator;
    }

    if (!explode) {
      if (!i) {
        // first element, so prepend variable name
        result += URI[encode](name) + (empty_name_separator || _value ? '=' : '');
      }

      if (d.type === 2) {
        // without explode-modifier, keys of objects are returned comma-separated
        result += _name + ',';
      }

      result += _value;
    } else {
      // only add the = if it is either default (?&) or there actually is a value (;)
      result += _name + (empty_name_separator || _value ? '=' : '') + _value;
    }
  }

  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.URITemplate.expandUnnamed"></a>[function <span class="apidocSignatureSpan">urijs.URITemplate.</span>expandUnnamed (d, options, explode, separator, length)](#apidoc.element.urijs.URITemplate.expandUnnamed)
- description and source-code
```javascript
expandUnnamed = function (d, options, explode, separator, length) {
  // variable result buffer
  var result = '';
  // performance crap
  var encode = options.encode;
  var empty_name_separator = options.empty_name_separator;
  // flag noting if values are already encoded
  var _encode = !d[encode].length;
  var _name, _value, i, l;

  // for each found value
  for (i = 0, l = d.val.length; i < l; i++) {
    if (length) {
      // maxlength must be determined before encoding can happen
      _value = URI[encode](d.val[i][1].substring(0, length));
    } else if (_encode) {
      // encode and cache value
      _value = URI[encode](d.val[i][1]);
      d[encode].push([
        d.type === 2 ? URI[encode](d.val[i][0]) : undefined,
        _value
      ]);
    } else {
      // value already encoded, pull from cache
      _value = d[encode][i][1];
    }

    if (result) {
      // unless we're the first value, prepend the separator
      result += separator;
    }

    if (d.type === 2) {
      if (length) {
        // maxlength also applies to keys of objects
        _name = URI[encode](d.val[i][0].substring(0, length));
      } else {
        // at this point the name must already be encoded
        _name = d[encode][i][0];
      }

      result += _name;
      if (explode) {
        // explode-modifier separates name and value by "="
        result += (empty_name_separator || _value ? '=' : '');
      } else {
        // no explode-modifier separates name and value by ","
        result += ',';
      }
    }

    result += _value;
  }

  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.URITemplate.noConflict"></a>[function <span class="apidocSignatureSpan">urijs.URITemplate.</span>noConflict ()](#apidoc.element.urijs.URITemplate.noConflict)
- description and source-code
```javascript
noConflict = function () {
  if (root.URITemplate === URITemplate) {
    root.URITemplate = _URITemplate;
  }

  return URITemplate;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.urijs.URITemplate.prototype"></a>[module urijs.URITemplate.prototype](#apidoc.module.urijs.URITemplate.prototype)

#### <a name="apidoc.element.urijs.URITemplate.prototype.expand"></a>[function <span class="apidocSignatureSpan">urijs.URITemplate.prototype.</span>expand (data, opts)](#apidoc.element.urijs.URITemplate.prototype.expand)
- description and source-code
```javascript
expand = function (data, opts) {
  var result = '';

  if (!this.parts || !this.parts.length) {
    // lazilyy parse the template
    this.parse();
  }

  if (!(data instanceof Data)) {
    // make given data available through the
    // optimized data handling thingie
    data = new Data(data);
  }

  for (var i = 0, l = this.parts.length; i < l; i++) {
<span class="apidocCodeCommentSpan">    /*jshint laxbreak: true */
</span>    result += typeof this.parts[i] === 'string'
      // literal string
      ? this.parts[i]
      // expression
      : URITemplate.expand(this.parts[i], data, opts);
    /*jshint laxbreak: false */
  }

  return result;
}
```
- example usage
```shell
...
URI("/foo/bar/baz.html")
  .relativeTo("/foo/bar/sub/world.html")
    // -> ../baz.html
  .absoluteTo("/foo/bar/sub/world.html");
    // -> /foo/bar/baz.html

// URI Templates
URI.expand("/foo/{dir}/{file}", {
  dir: "bar",
  file: "world.html"
});
// -> /foo/bar/world.html
'''

See the [About Page](http://medialize.github.io/URI.js/) and [API Docs](http://medialize.github.io/URI.js/docs.html) for more stuff
.
...
```

#### <a name="apidoc.element.urijs.URITemplate.prototype.parse"></a>[function <span class="apidocSignatureSpan">urijs.URITemplate.prototype.</span>parse ()](#apidoc.element.urijs.URITemplate.prototype.parse)
- description and source-code
```javascript
parse = function () {
  // performance crap
  var expression = this.expression;
  var ePattern = URITemplate.EXPRESSION_PATTERN;
  var vPattern = URITemplate.VARIABLE_PATTERN;
  var nPattern = URITemplate.VARIABLE_NAME_PATTERN;
  var lPattern = URITemplate.LITERAL_PATTERN;
  // token result buffer
  var parts = [];
    // position within source template
  var pos = 0;
  var variables, eMatch, vMatch;

  var checkLiteral = function(literal) {
    if (literal.match(lPattern)) {
      throw new Error('Invalid Literal "' + literal + '"');
    }
    return literal;
  };

  // RegExp is shared accross all templates,
  // which requires a manual reset
  ePattern.lastIndex = 0;
  // I don't like while(foo = bar()) loops,
  // to make things simpler I go while(true) and break when required
  while (true) {
    eMatch = ePattern.exec(expression);
    if (eMatch === null) {
      // push trailing literal
      parts.push(checkLiteral(expression.substring(pos)));
      break;
    } else {
      // push leading literal
      parts.push(checkLiteral(expression.substring(pos, eMatch.index)));
      pos = eMatch.index + eMatch[0].length;
    }

    if (!operators[eMatch[1]]) {
      throw new Error('Unknown Operator "' + eMatch[1]  + '" in "' + eMatch[0] + '"');
    } else if (!eMatch[3]) {
      throw new Error('Unclosed Expression "' + eMatch[0]  + '"');
    }

    // parse variable-list
    variables = eMatch[2].split(',');
    for (var i = 0, l = variables.length; i < l; i++) {
      vMatch = variables[i].match(vPattern);
      if (vMatch === null) {
        throw new Error('Invalid Variable "' + variables[i] + '" in "' + eMatch[0] + '"');
      } else if (vMatch[1].match(nPattern)) {
        throw new Error('Invalid Variable Name "' + vMatch[1] + '" in "' + eMatch[0] + '"');
      }

      variables[i] = {
        name: vMatch[1],
        explode: !!vMatch[3],
        maxlength: vMatch[4] && parseInt(vMatch[4], 10)
      };
    }

    if (!variables.length) {
      throw new Error('Expression Missing Variable(s) "' + eMatch[0] + '"');
    }

    parts.push({
      expression: eMatch[0],
      operator: eMatch[1],
      variables: variables
    });
  }

  if (!parts.length) {
    // template doesn't contain any expressions
    // so it is a simple literal string
    // this probably should fire a warning or something?
    parts.push(checkLiteral(expression));
  }

  this.parts = parts;
  return this;
}
```
- example usage
```shell
...

  // expand template through given data map
  p.expand = function(data, opts) {
var result = '';

if (!this.parts || !this.parts.length) {
  // lazilyy parse the template
  this.parse();
}

if (!(data instanceof Data)) {
  // make given data available through the
  // optimized data handling thingie
  data = new Data(data);
}
...
```



# <a name="apidoc.module.urijs.punycode"></a>[module urijs.punycode](#apidoc.module.urijs.punycode)

#### <a name="apidoc.element.urijs.punycode.decode"></a>[function <span class="apidocSignatureSpan">urijs.punycode.</span>decode (input)](#apidoc.element.urijs.punycode.decode)
- description and source-code
```javascript
function decode(input) {
		// Don't use UCS-2
		var output = [],
		    inputLength = input.length,
		    out,
		    i = 0,
		    n = initialN,
		    bias = initialBias,
		    basic,
		    j,
		    index,
		    oldi,
		    w,
		    k,
		    digit,
		    t,
		<span class="apidocCodeCommentSpan">    /** Cached calculation results */
</span>		    baseMinusT;

		// Handle the basic code points: let 'basic' be the number of input code
		// points before the last delimiter, or '0' if there is none, then copy
		// the first basic code points to the output.

		basic = input.lastIndexOf(delimiter);
		if (basic < 0) {
			basic = 0;
		}

		for (j = 0; j < basic; ++j) {
			// if it's not a basic code point
			if (input.charCodeAt(j) >= 0x80) {
				error('not-basic');
			}
			output.push(input.charCodeAt(j));
		}

		// Main decoding loop: start just after the last delimiter if any basic code
		// points were copied; start at the beginning otherwise.

		for (index = basic > 0 ? basic + 1 : 0; index < inputLength; /* no final expression */) {

			// 'index' is the index of the next character to be consumed.
			// Decode a generalized variable-length integer into 'delta',
			// which gets added to 'i'. The overflow checking is easier
			// if we increase 'i' as we go, then subtract off its starting
			// value at the end to obtain 'delta'.
			for (oldi = i, w = 1, k = base; /* no condition */; k += base) {

				if (index >= inputLength) {
					error('invalid-input');
				}

				digit = basicToDigit(input.charCodeAt(index++));

				if (digit >= base || digit > floor((maxInt - i) / w)) {
					error('overflow');
				}

				i += digit * w;
				t = k <= bias ? tMin : (k >= bias + tMax ? tMax : k - bias);

				if (digit < t) {
					break;
				}

				baseMinusT = base - t;
				if (w > floor(maxInt / baseMinusT)) {
					error('overflow');
				}

				w *= baseMinusT;

			}

			out = output.length + 1;
			bias = adapt(i - oldi, out, oldi == 0);

			// 'i' was supposed to wrap around from 'out' to '0',
			// incrementing 'n' each time, so we'll fix that now:
			if (floor(i / out) > maxInt - n) {
				error('overflow');
			}

			n += floor(i / out);
			i %= out;

			// Insert 'n' at position 'i' of the output
			output.splice(i++, 0, n);

		}

		return ucs2encode(output);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.punycode.encode"></a>[function <span class="apidocSignatureSpan">urijs.punycode.</span>encode (input)](#apidoc.element.urijs.punycode.encode)
- description and source-code
```javascript
function encode(input) {
		var n,
		    delta,
		    handledCPCount,
		    basicLength,
		    bias,
		    j,
		    m,
		    q,
		    k,
		    t,
		    currentValue,
		    output = [],
		<span class="apidocCodeCommentSpan">    /** 'inputLength' will hold the number of code points in 'input'. */
</span>		    inputLength,
		    /** Cached calculation results */
		    handledCPCountPlusOne,
		    baseMinusT,
		    qMinusT;

		// Convert the input in UCS-2 to Unicode
		input = ucs2decode(input);

		// Cache the length
		inputLength = input.length;

		// Initialize the state
		n = initialN;
		delta = 0;
		bias = initialBias;

		// Handle the basic code points
		for (j = 0; j < inputLength; ++j) {
			currentValue = input[j];
			if (currentValue < 0x80) {
				output.push(stringFromCharCode(currentValue));
			}
		}

		handledCPCount = basicLength = output.length;

		// 'handledCPCount' is the number of code points that have been handled;
		// 'basicLength' is the number of basic code points.

		// Finish the basic string - if it is not empty - with a delimiter
		if (basicLength) {
			output.push(delimiter);
		}

		// Main encoding loop:
		while (handledCPCount < inputLength) {

			// All non-basic code points < n have been handled already. Find the next
			// larger one:
			for (m = maxInt, j = 0; j < inputLength; ++j) {
				currentValue = input[j];
				if (currentValue >= n && currentValue < m) {
					m = currentValue;
				}
			}

			// Increase 'delta' enough to advance the decoder's <n,i> state to <m,0>,
			// but guard against overflow
			handledCPCountPlusOne = handledCPCount + 1;
			if (m - n > floor((maxInt - delta) / handledCPCountPlusOne)) {
				error('overflow');
			}

			delta += (m - n) * handledCPCountPlusOne;
			n = m;

			for (j = 0; j < inputLength; ++j) {
				currentValue = input[j];

				if (currentValue < n && ++delta > maxInt) {
					error('overflow');
				}

				if (currentValue == n) {
					// Represent delta as a generalized variable-length integer
					for (q = delta, k = base; /* no condition */; k += base) {
						t = k <= bias ? tMin : (k >= bias + tMax ? tMax : k - bias);
						if (q < t) {
							break;
						}
						qMinusT = q - t;
						baseMinusT = base - t;
						output.push(
							stringFromCharCode(digitToBasic(t + qMinusT % baseMinusT, 0))
						);
						q = floor(qMinusT / baseMinusT);
					}

					output.push(stringFromCharCode(digitToBasic(q, 0)));
					bias = adapt(delta, handledCPCountPlusOne, handledCPCount == basicLength);
					delta = 0;
					++handledCPCount;
				}
			}

			++delta;
			++n;

		}
		return output.join('');
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.punycode.toASCII"></a>[function <span class="apidocSignatureSpan">urijs.punycode.</span>toASCII (input)](#apidoc.element.urijs.punycode.toASCII)
- description and source-code
```javascript
function toASCII(input) {
		return mapDomain(input, function(string) {
			return regexNonASCII.test(string)
				? 'xn--' + encode(string)
				: string;
		});
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.urijs.punycode.toUnicode"></a>[function <span class="apidocSignatureSpan">urijs.punycode.</span>toUnicode (input)](#apidoc.element.urijs.punycode.toUnicode)
- description and source-code
```javascript
function toUnicode(input) {
		return mapDomain(input, function(string) {
			return regexPunycode.test(string)
				? decode(string.slice(4).toLowerCase())
				: string;
		});
	}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
