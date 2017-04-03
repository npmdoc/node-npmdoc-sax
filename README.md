# api documentation for  [sax (v1.2.2)](https://github.com/isaacs/sax-js#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-sax.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-sax) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-sax.svg)](https://travis-ci.org/npmdoc/node-npmdoc-sax)
#### An evented streaming XML parser in JavaScript

[![NPM](https://nodei.co/npm/sax.png?downloads=true)](https://www.npmjs.com/package/sax)

[![apidoc](https://npmdoc.github.io/node-npmdoc-sax/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-sax_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-sax/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-sax/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-sax/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Isaac Z. Schlueter",
        "email": "i@izs.me",
        "url": "http://blog.izs.me/"
    },
    "bugs": {
        "url": "https://github.com/isaacs/sax-js/issues"
    },
    "contributors": [
        {
            "name": "Isaac Z. Schlueter",
            "email": "i@izs.me"
        },
        {
            "name": "Stein Martin Hustad",
            "email": "stein@hustad.com"
        },
        {
            "name": "Mikeal Rogers",
            "email": "mikeal.rogers@gmail.com"
        },
        {
            "name": "Laurie Harper",
            "email": "laurie@holoweb.net"
        },
        {
            "name": "Jann Horn",
            "email": "jann@Jann-PC.fritz.box"
        },
        {
            "name": "Elijah Insua",
            "email": "tmpvar@gmail.com"
        },
        {
            "name": "Henry Rawas",
            "email": "henryr@schakra.com"
        },
        {
            "name": "Justin Makeig",
            "email": "jmpublic@makeig.com"
        },
        {
            "name": "Mike Schilling",
            "email": "mike@emotive.com"
        }
    ],
    "dependencies": {},
    "description": "An evented streaming XML parser in JavaScript",
    "devDependencies": {
        "standard": "^8.6.0",
        "tap": "^10.0.2"
    },
    "directories": {},
    "dist": {
        "shasum": "fd8631a23bc7826bef5d871bdb87378c95647828",
        "tarball": "https://registry.npmjs.org/sax/-/sax-1.2.2.tgz"
    },
    "files": [
        "lib/sax.js",
        "LICENSE",
        "README.md"
    ],
    "gitHead": "27a70c4af4980323d8af47483a126289ea32e567",
    "homepage": "https://github.com/isaacs/sax-js#readme",
    "license": "ISC",
    "main": "lib/sax.js",
    "maintainers": [
        {
            "name": "isaacs",
            "email": "i@izs.me"
        }
    ],
    "name": "sax",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/isaacs/sax-js.git"
    },
    "scripts": {
        "posttest": "standard -F test/*.js lib/*.js",
        "test": "tap test/*.js --cov -j4"
    },
    "version": "1.2.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module sax](#apidoc.module.sax)
1.  [function <span class="apidocSignatureSpan">sax.</span>SAXParser (strict, opt)](#apidoc.element.sax.SAXParser)
1.  [function <span class="apidocSignatureSpan">sax.</span>SAXStream (strict, opt)](#apidoc.element.sax.SAXStream)
1.  [function <span class="apidocSignatureSpan">sax.</span>createStream (strict, opt)](#apidoc.element.sax.createStream)
1.  [function <span class="apidocSignatureSpan">sax.</span>parser (strict, opt)](#apidoc.element.sax.parser)
1.  number <span class="apidocSignatureSpan">sax.</span>MAX_BUFFER_LENGTH
1.  object <span class="apidocSignatureSpan">sax.</span>ENTITIES
1.  object <span class="apidocSignatureSpan">sax.</span>EVENTS
1.  object <span class="apidocSignatureSpan">sax.</span>SAXParser.prototype
1.  object <span class="apidocSignatureSpan">sax.</span>SAXStream.prototype
1.  object <span class="apidocSignatureSpan">sax.</span>STATE
1.  object <span class="apidocSignatureSpan">sax.</span>XML_ENTITIES

#### [module sax.SAXParser](#apidoc.module.sax.SAXParser)
1.  [function <span class="apidocSignatureSpan">sax.</span>SAXParser (strict, opt)](#apidoc.element.sax.SAXParser.SAXParser)

#### [module sax.SAXParser.prototype](#apidoc.module.sax.SAXParser.prototype)
1.  [function <span class="apidocSignatureSpan">sax.SAXParser.prototype.</span>close ()](#apidoc.element.sax.SAXParser.prototype.close)
1.  [function <span class="apidocSignatureSpan">sax.SAXParser.prototype.</span>end ()](#apidoc.element.sax.SAXParser.prototype.end)
1.  [function <span class="apidocSignatureSpan">sax.SAXParser.prototype.</span>flush ()](#apidoc.element.sax.SAXParser.prototype.flush)
1.  [function <span class="apidocSignatureSpan">sax.SAXParser.prototype.</span>resume ()](#apidoc.element.sax.SAXParser.prototype.resume)
1.  [function <span class="apidocSignatureSpan">sax.SAXParser.prototype.</span>write (chunk)](#apidoc.element.sax.SAXParser.prototype.write)

#### [module sax.SAXStream](#apidoc.module.sax.SAXStream)
1.  [function <span class="apidocSignatureSpan">sax.</span>SAXStream (strict, opt)](#apidoc.element.sax.SAXStream.SAXStream)

#### [module sax.SAXStream.prototype](#apidoc.module.sax.SAXStream.prototype)
1.  [function <span class="apidocSignatureSpan">sax.SAXStream.prototype.</span>end (chunk)](#apidoc.element.sax.SAXStream.prototype.end)
1.  [function <span class="apidocSignatureSpan">sax.SAXStream.prototype.</span>on (ev, handler)](#apidoc.element.sax.SAXStream.prototype.on)
1.  [function <span class="apidocSignatureSpan">sax.SAXStream.prototype.</span>write (data)](#apidoc.element.sax.SAXStream.prototype.write)



# <a name="apidoc.module.sax"></a>[module sax](#apidoc.module.sax)

#### <a name="apidoc.element.sax.SAXParser"></a>[function <span class="apidocSignatureSpan">sax.</span>SAXParser (strict, opt)](#apidoc.element.sax.SAXParser)
- description and source-code
```javascript
function SAXParser(strict, opt) {
  if (!(this instanceof SAXParser)) {
    return new SAXParser(strict, opt)
  }

  var parser = this
  clearBuffers(parser)
  parser.q = parser.c = ''
  parser.bufferCheckPosition = sax.MAX_BUFFER_LENGTH
  parser.opt = opt || {}
  parser.opt.lowercase = parser.opt.lowercase || parser.opt.lowercasetags
  parser.looseCase = parser.opt.lowercase ? 'toLowerCase' : 'toUpperCase'
  parser.tags = []
  parser.closed = parser.closedRoot = parser.sawRoot = false
  parser.tag = parser.error = null
  parser.strict = !!strict
  parser.noscript = !!(strict || parser.opt.noscript)
  parser.state = S.BEGIN
  parser.strictEntities = parser.opt.strictEntities
  parser.ENTITIES = parser.strictEntities ? Object.create(sax.XML_ENTITIES) : Object.create(sax.ENTITIES)
  parser.attribList = []

  // namespaces form a prototype chain.
  // it always points at the current tag,
  // which protos to its parent tag.
  if (parser.opt.xmlns) {
    parser.ns = Object.create(rootNS)
  }

  // mostly just for error reporting
  parser.trackPosition = parser.opt.position !== false
  if (parser.trackPosition) {
    parser.position = parser.line = parser.column = 0
  }
  emit(parser, 'onready')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sax.SAXStream"></a>[function <span class="apidocSignatureSpan">sax.</span>SAXStream (strict, opt)](#apidoc.element.sax.SAXStream)
- description and source-code
```javascript
function SAXStream(strict, opt) {
  if (!(this instanceof SAXStream)) {
    return new SAXStream(strict, opt)
  }

  Stream.apply(this)

  this._parser = new SAXParser(strict, opt)
  this.writable = true
  this.readable = true

  var me = this

  this._parser.onend = function () {
    me.emit('end')
  }

  this._parser.onerror = function (er) {
    me.emit('error', er)

    // if didn't throw, then means error was handled.
    // go ahead and clear error, so we can write again.
    me._parser.error = null
  }

  this._decoder = null

  streamWraps.forEach(function (ev) {
    Object.defineProperty(me, 'on' + ev, {
      get: function () {
        return me._parser['on' + ev]
      },
      set: function (h) {
        if (!h) {
          me.removeAllListeners(ev)
          me._parser['on' + ev] = h
          return h
        }
        me.on(ev, h)
      },
      enumerable: true,
      configurable: false
    })
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sax.createStream"></a>[function <span class="apidocSignatureSpan">sax.</span>createStream (strict, opt)](#apidoc.element.sax.createStream)
- description and source-code
```javascript
function createStream(strict, opt) {
  return new SAXStream(strict, opt)
}
```
- example usage
```shell
...
// parser stream is done, and ready to have more stuff written to it.
};

parser.write('<xml>Hello, <who name="world">world</who>!</xml>').close();

// stream usage
// takes the same options as the parser
var saxStream = require("sax").createStream(strict, options)
saxStream.on("error", function (e) {
// unhandled errors will throw, since this is a proper node
// event emitter.
console.error("error!", e)
// clear the error
this._parser.error = null
this._parser.resume()
...
```

#### <a name="apidoc.element.sax.parser"></a>[function <span class="apidocSignatureSpan">sax.</span>parser (strict, opt)](#apidoc.element.sax.parser)
- description and source-code
```javascript
parser = function (strict, opt) { return new SAXParser(strict, opt) }
```
- example usage
```shell
...
through unmolested.

## Usage

'''javascript
var sax = require("./lib/sax"),
  strict = true, // set to false for html-mode
  parser = sax.parser(strict);

parser.onerror = function (e) {
  // an error happened.
};
parser.ontext = function (t) {
  // got some text.  t is the string of text.
};
...
```



# <a name="apidoc.module.sax.SAXParser"></a>[module sax.SAXParser](#apidoc.module.sax.SAXParser)

#### <a name="apidoc.element.sax.SAXParser.SAXParser"></a>[function <span class="apidocSignatureSpan">sax.</span>SAXParser (strict, opt)](#apidoc.element.sax.SAXParser.SAXParser)
- description and source-code
```javascript
function SAXParser(strict, opt) {
  if (!(this instanceof SAXParser)) {
    return new SAXParser(strict, opt)
  }

  var parser = this
  clearBuffers(parser)
  parser.q = parser.c = ''
  parser.bufferCheckPosition = sax.MAX_BUFFER_LENGTH
  parser.opt = opt || {}
  parser.opt.lowercase = parser.opt.lowercase || parser.opt.lowercasetags
  parser.looseCase = parser.opt.lowercase ? 'toLowerCase' : 'toUpperCase'
  parser.tags = []
  parser.closed = parser.closedRoot = parser.sawRoot = false
  parser.tag = parser.error = null
  parser.strict = !!strict
  parser.noscript = !!(strict || parser.opt.noscript)
  parser.state = S.BEGIN
  parser.strictEntities = parser.opt.strictEntities
  parser.ENTITIES = parser.strictEntities ? Object.create(sax.XML_ENTITIES) : Object.create(sax.ENTITIES)
  parser.attribList = []

  // namespaces form a prototype chain.
  // it always points at the current tag,
  // which protos to its parent tag.
  if (parser.opt.xmlns) {
    parser.ns = Object.create(rootNS)
  }

  // mostly just for error reporting
  parser.trackPosition = parser.opt.position !== false
  if (parser.trackPosition) {
    parser.position = parser.line = parser.column = 0
  }
  emit(parser, 'onready')
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.sax.SAXParser.prototype"></a>[module sax.SAXParser.prototype](#apidoc.module.sax.SAXParser.prototype)

#### <a name="apidoc.element.sax.SAXParser.prototype.close"></a>[function <span class="apidocSignatureSpan">sax.SAXParser.prototype.</span>close ()](#apidoc.element.sax.SAXParser.prototype.close)
- description and source-code
```javascript
close = function () { return this.write(null) }
```
- example usage
```shell
...
parser.onattribute = function (attr) {
// an attribute.  attr has "name" and "value"
};
parser.onend = function () {
// parser stream is done, and ready to have more stuff written to it.
};

parser.write('<xml>Hello, <who name="world">world</who>!</xml>').close();

// stream usage
// takes the same options as the parser
var saxStream = require("sax").createStream(strict, options)
saxStream.on("error", function (e) {
// unhandled errors will throw, since this is a proper node
// event emitter.
...
```

#### <a name="apidoc.element.sax.SAXParser.prototype.end"></a>[function <span class="apidocSignatureSpan">sax.SAXParser.prototype.</span>end ()](#apidoc.element.sax.SAXParser.prototype.end)
- description and source-code
```javascript
end = function () { end(this) }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sax.SAXParser.prototype.flush"></a>[function <span class="apidocSignatureSpan">sax.SAXParser.prototype.</span>flush ()](#apidoc.element.sax.SAXParser.prototype.flush)
- description and source-code
```javascript
flush = function () { flushBuffers(this) }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sax.SAXParser.prototype.resume"></a>[function <span class="apidocSignatureSpan">sax.SAXParser.prototype.</span>resume ()](#apidoc.element.sax.SAXParser.prototype.resume)
- description and source-code
```javascript
resume = function () { this.error = null; return this }
```
- example usage
```shell
...
var saxStream = require("sax").createStream(strict, options)
saxStream.on("error", function (e) {
  // unhandled errors will throw, since this is a proper node
  // event emitter.
  console.error("error!", e)
  // clear the error
  this._parser.error = null
  this._parser.resume()
})
saxStream.on("opentag", function (node) {
  // same object as above
})
// pipe is supported, and it's readable/writable
// same chunks coming in also go out.
fs.createReadStream("file.xml")
...
```

#### <a name="apidoc.element.sax.SAXParser.prototype.write"></a>[function <span class="apidocSignatureSpan">sax.SAXParser.prototype.</span>write (chunk)](#apidoc.element.sax.SAXParser.prototype.write)
- description and source-code
```javascript
function write(chunk) {
  var parser = this
  if (this.error) {
    throw this.error
  }
  if (parser.closed) {
    return error(parser,
      'Cannot write after close. Assign an onready handler.')
  }
  if (chunk === null) {
    return end(parser)
  }
  if (typeof chunk === 'object') {
    chunk = chunk.toString()
  }
  var i = 0
  var c = ''
  while (true) {
    c = charAt(chunk, i++)
    parser.c = c

    if (!c) {
      break
    }

    if (parser.trackPosition) {
      parser.position++
      if (c === '\n') {
        parser.line++
        parser.column = 0
      } else {
        parser.column++
      }
    }

    switch (parser.state) {
      case S.BEGIN:
        parser.state = S.BEGIN_WHITESPACE
        if (c === '\uFEFF') {
          continue
        }
        beginWhiteSpace(parser, c)
        continue

      case S.BEGIN_WHITESPACE:
        beginWhiteSpace(parser, c)
        continue

      case S.TEXT:
        if (parser.sawRoot && !parser.closedRoot) {
          var starti = i - 1
          while (c && c !== '<' && c !== '&') {
            c = charAt(chunk, i++)
            if (c && parser.trackPosition) {
              parser.position++
              if (c === '\n') {
                parser.line++
                parser.column = 0
              } else {
                parser.column++
              }
            }
          }
          parser.textNode += chunk.substring(starti, i - 1)
        }
        if (c === '<' && !(parser.sawRoot && parser.closedRoot && !parser.strict)) {
          parser.state = S.OPEN_WAKA
          parser.startTagPosition = parser.position
        } else {
          if (not(whitespace, c) && (!parser.sawRoot || parser.closedRoot)) {
            strictFail(parser, 'Text data outside of root node.')
          }
          if (c === '&') {
            parser.state = S.TEXT_ENTITY
          } else {
            parser.textNode += c
          }
        }
        continue

      case S.SCRIPT:
        // only non-strict
        if (c === '<') {
          parser.state = S.SCRIPT_ENDING
        } else {
          parser.script += c
        }
        continue

      case S.SCRIPT_ENDING:
        if (c === '/') {
          parser.state = S.CLOSE_TAG
        } else {
          parser.script += '<' + c
          parser.state = S.SCRIPT
        }
        continue

      case S.OPEN_WAKA:
        // either a /, ?, !, or text is coming next.
        if (c === '!') {
          parser.state = S.SGML_DECL
          parser.sgmlDecl = ''
        } else if (is(whitespace, c)) {
          // wait for it...
        } else if (isMatch(nameStart, c)) {
          parser.state = S.OPEN_TAG
          parser.tagName = c
        } else if (c === '/') {
          parser.state = S.CLOSE_TAG
          parser.tagName = ''
        } else if (c === '?') {
          parser.state = S.PROC_INST
          parser.procInstName = parser.procInstBody = ''
        } else {
          strictFail(parser, 'Unencoded <')
          // if there was some whitespace, then add that in.
          if (parser.startTagPosition + 1 < parser.position) {
            var pad = parser.position - parser.startTagPosition
            c = new Array(pad).join(' ') + c
          }
          parser.textNode += '<' + c
          parser.state = S.TEXT
        }
        continue

      case S.SGML_DECL:
        if ((parser.sgmlDecl + c).toUpperCase() === CDATA) {
          emitNode(parser, 'onopencdata')
          parser.state = S.CDATA
          parser.sgmlDecl = ''
          parser.cdata = ''
        } else if (parser.sgmlDecl + c === '--') {
          parser.state = S.COMMENT
          parser.comment = ''
          parser.sgmlDecl = ''
        } else if ((parser.sgmlDecl + c).toUpperCase() === DOCTYPE) {
          parser.state = S.DOCTYPE
          if (parser.doctype || parser.sawRoot) {
            strictFail(parser,
              'Inappropriately located doctype declaration')
          }
          parser.doctype = ''
          parser.sgmlDecl = ''
        } else if (c === '>') {
          emitNode(parser, 'onsgmldeclaration', parser.sgmlDecl) ...
```
- example usage
```shell
...
parser.onattribute = function (attr) {
// an attribute.  attr has "name" and "value"
};
parser.onend = function () {
// parser stream is done, and ready to have more stuff written to it.
};

parser.write('<xml>Hello, <who name="world">world</who>!</xml>').close();

// stream usage
// takes the same options as the parser
var saxStream = require("sax").createStream(strict, options)
saxStream.on("error", function (e) {
// unhandled errors will throw, since this is a proper node
// event emitter.
...
```



# <a name="apidoc.module.sax.SAXStream"></a>[module sax.SAXStream](#apidoc.module.sax.SAXStream)

#### <a name="apidoc.element.sax.SAXStream.SAXStream"></a>[function <span class="apidocSignatureSpan">sax.</span>SAXStream (strict, opt)](#apidoc.element.sax.SAXStream.SAXStream)
- description and source-code
```javascript
function SAXStream(strict, opt) {
  if (!(this instanceof SAXStream)) {
    return new SAXStream(strict, opt)
  }

  Stream.apply(this)

  this._parser = new SAXParser(strict, opt)
  this.writable = true
  this.readable = true

  var me = this

  this._parser.onend = function () {
    me.emit('end')
  }

  this._parser.onerror = function (er) {
    me.emit('error', er)

    // if didn't throw, then means error was handled.
    // go ahead and clear error, so we can write again.
    me._parser.error = null
  }

  this._decoder = null

  streamWraps.forEach(function (ev) {
    Object.defineProperty(me, 'on' + ev, {
      get: function () {
        return me._parser['on' + ev]
      },
      set: function (h) {
        if (!h) {
          me.removeAllListeners(ev)
          me._parser['on' + ev] = h
          return h
        }
        me.on(ev, h)
      },
      enumerable: true,
      configurable: false
    })
  })
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.sax.SAXStream.prototype"></a>[module sax.SAXStream.prototype](#apidoc.module.sax.SAXStream.prototype)

#### <a name="apidoc.element.sax.SAXStream.prototype.end"></a>[function <span class="apidocSignatureSpan">sax.SAXStream.prototype.</span>end (chunk)](#apidoc.element.sax.SAXStream.prototype.end)
- description and source-code
```javascript
end = function (chunk) {
  if (chunk && chunk.length) {
    this.write(chunk)
  }
  this._parser.end()
  return true
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sax.SAXStream.prototype.on"></a>[function <span class="apidocSignatureSpan">sax.SAXStream.prototype.</span>on (ev, handler)](#apidoc.element.sax.SAXStream.prototype.on)
- description and source-code
```javascript
on = function (ev, handler) {
  var me = this
  if (!me._parser['on' + ev] && streamWraps.indexOf(ev) !== -1) {
    me._parser['on' + ev] = function () {
      var args = arguments.length === 1 ? [arguments[0]] : Array.apply(null, arguments)
      args.splice(0, 0, ev)
      me.emit.apply(me, args)
    }
  }

  return Stream.prototype.on.call(me, ev, handler)
}
```
- example usage
```shell
...
};

parser.write('<xml>Hello, <who name="world">world</who>!</xml>').close();

// stream usage
// takes the same options as the parser
var saxStream = require("sax").createStream(strict, options)
saxStream.on("error", function (e) {
  // unhandled errors will throw, since this is a proper node
  // event emitter.
  console.error("error!", e)
  // clear the error
  this._parser.error = null
  this._parser.resume()
})
...
```

#### <a name="apidoc.element.sax.SAXStream.prototype.write"></a>[function <span class="apidocSignatureSpan">sax.SAXStream.prototype.</span>write (data)](#apidoc.element.sax.SAXStream.prototype.write)
- description and source-code
```javascript
write = function (data) {
  if (typeof Buffer === 'function' &&
    typeof Buffer.isBuffer === 'function' &&
    Buffer.isBuffer(data)) {
    if (!this._decoder) {
      var SD = require('string_decoder').StringDecoder
      this._decoder = new SD('utf8')
    }
    data = this._decoder.write(data)
  }

  this._parser.write(data.toString())
  this.emit('data', data)
  return true
}
```
- example usage
```shell
...
parser.onattribute = function (attr) {
// an attribute.  attr has "name" and "value"
};
parser.onend = function () {
// parser stream is done, and ready to have more stuff written to it.
};

parser.write('<xml>Hello, <who name="world">world</who>!</xml>').close();

// stream usage
// takes the same options as the parser
var saxStream = require("sax").createStream(strict, options)
saxStream.on("error", function (e) {
// unhandled errors will throw, since this is a proper node
// event emitter.
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
