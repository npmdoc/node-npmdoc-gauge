# api documentation for  [gauge (v2.7.3)](https://github.com/iarna/gauge)  [![npm package](https://img.shields.io/npm/v/npmdoc-gauge.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gauge) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gauge.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gauge)
#### A terminal based horizontal guage

[![NPM](https://nodei.co/npm/gauge.png?downloads=true)](https://www.npmjs.com/package/gauge)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gauge/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-gauge_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gauge/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gauge/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gauge/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Rebecca Turner",
        "email": "me@re-becca.org"
    },
    "bugs": {
        "url": "https://github.com/iarna/gauge/issues"
    },
    "dependencies": {
        "aproba": "^1.0.3",
        "console-control-strings": "^1.0.0",
        "has-unicode": "^2.0.0",
        "object-assign": "^4.1.0",
        "signal-exit": "^3.0.0",
        "string-width": "^1.0.1",
        "strip-ansi": "^3.0.1",
        "wide-align": "^1.1.0"
    },
    "description": "A terminal based horizontal guage",
    "devDependencies": {
        "readable-stream": "^2.0.6",
        "require-inject": "^1.4.0",
        "standard": "^7.1.2",
        "tap": "^5.7.2",
        "through2": "^2.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "1c23855f962f17b3ad3d0dc7443f304542edfe09",
        "tarball": "https://registry.npmjs.org/gauge/-/gauge-2.7.3.tgz"
    },
    "files": [
        "base-theme.js",
        "CHANGELOG.md",
        "error.js",
        "has-color.js",
        "index.js",
        "LICENSE",
        "package.json",
        "plumbing.js",
        "process.js",
        "progress-bar.js",
        "README.md",
        "render-template.js",
        "set-immediate.js",
        "set-interval.js",
        "spin.js",
        "template-item.js",
        "theme-set.js",
        "themes.js",
        "wide-truncate.js"
    ],
    "gitHead": "2defcdb50c243c92d21f0fd39c4b06bd48bcfdf3",
    "homepage": "https://github.com/iarna/gauge",
    "keywords": [
        "progressbar",
        "progress",
        "gauge"
    ],
    "license": "ISC",
    "main": "index.js",
    "maintainers": [
        {
            "name": "iarna",
            "email": "me@re-becca.org"
        }
    ],
    "name": "gauge",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/iarna/gauge.git"
    },
    "scripts": {
        "prepublish": "rm -f *~",
        "test": "standard && tap test/*.js --coverage"
    },
    "version": "2.7.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module gauge](#apidoc.module.gauge)
1.  [function <span class="apidocSignatureSpan">gauge.</span>plumbing (theme, template, width)](#apidoc.element.gauge.plumbing)
1.  [function <span class="apidocSignatureSpan">gauge.</span>template_item (values, outputLength)](#apidoc.element.gauge.template_item)
1.  [function <span class="apidocSignatureSpan">gauge.</span>themes (opts)](#apidoc.element.gauge.themes)
1.  object <span class="apidocSignatureSpan">gauge.</span>base_theme
1.  object <span class="apidocSignatureSpan">gauge.</span>error
1.  object <span class="apidocSignatureSpan">gauge.</span>plumbing.prototype
1.  object <span class="apidocSignatureSpan">gauge.</span>template_item.prototype

#### [module gauge.base_theme](#apidoc.module.gauge.base_theme)
1.  [function <span class="apidocSignatureSpan">gauge.base_theme.</span>activityIndicator (values, theme, width)](#apidoc.element.gauge.base_theme.activityIndicator)
1.  [function <span class="apidocSignatureSpan">gauge.base_theme.</span>progressbar (values, theme, width)](#apidoc.element.gauge.base_theme.progressbar)

#### [module gauge.error](#apidoc.module.gauge.error)
1.  [function <span class="apidocSignatureSpan">gauge.error.</span>Internal (msg)](#apidoc.element.gauge.error.Internal)
1.  [function <span class="apidocSignatureSpan">gauge.error.</span>MissingTemplateValue (item, values)](#apidoc.element.gauge.error.MissingTemplateValue)
1.  [function <span class="apidocSignatureSpan">gauge.error.</span>User (msg)](#apidoc.element.gauge.error.User)

#### [module gauge.plumbing](#apidoc.module.gauge.plumbing)
1.  [function <span class="apidocSignatureSpan">gauge.</span>plumbing (theme, template, width)](#apidoc.element.gauge.plumbing.plumbing)

#### [module gauge.plumbing.prototype](#apidoc.module.gauge.plumbing.prototype)
1.  [function <span class="apidocSignatureSpan">gauge.plumbing.prototype.</span>hide ()](#apidoc.element.gauge.plumbing.prototype.hide)
1.  [function <span class="apidocSignatureSpan">gauge.plumbing.prototype.</span>hideCursor ()](#apidoc.element.gauge.plumbing.prototype.hideCursor)
1.  [function <span class="apidocSignatureSpan">gauge.plumbing.prototype.</span>setTemplate (template)](#apidoc.element.gauge.plumbing.prototype.setTemplate)
1.  [function <span class="apidocSignatureSpan">gauge.plumbing.prototype.</span>setTheme (theme)](#apidoc.element.gauge.plumbing.prototype.setTheme)
1.  [function <span class="apidocSignatureSpan">gauge.plumbing.prototype.</span>setWidth (width)](#apidoc.element.gauge.plumbing.prototype.setWidth)
1.  [function <span class="apidocSignatureSpan">gauge.plumbing.prototype.</span>show (status)](#apidoc.element.gauge.plumbing.prototype.show)
1.  [function <span class="apidocSignatureSpan">gauge.plumbing.prototype.</span>showCursor ()](#apidoc.element.gauge.plumbing.prototype.showCursor)

#### [module gauge.template_item](#apidoc.module.gauge.template_item)
1.  [function <span class="apidocSignatureSpan">gauge.</span>template_item (values, outputLength)](#apidoc.element.gauge.template_item.template_item)

#### [module gauge.template_item.prototype](#apidoc.module.gauge.template_item.prototype)
1.  [function <span class="apidocSignatureSpan">gauge.template_item.prototype.</span>getBaseLength ()](#apidoc.element.gauge.template_item.prototype.getBaseLength)
1.  [function <span class="apidocSignatureSpan">gauge.template_item.prototype.</span>getLength ()](#apidoc.element.gauge.template_item.prototype.getLength)
1.  [function <span class="apidocSignatureSpan">gauge.template_item.prototype.</span>getMaxLength ()](#apidoc.element.gauge.template_item.prototype.getMaxLength)
1.  [function <span class="apidocSignatureSpan">gauge.template_item.prototype.</span>getMinLength ()](#apidoc.element.gauge.template_item.prototype.getMinLength)

#### [module gauge.themes](#apidoc.module.gauge.themes)
1.  [function <span class="apidocSignatureSpan">gauge.themes.</span>addTheme (name, parent, theme)](#apidoc.element.gauge.themes.addTheme)
1.  [function <span class="apidocSignatureSpan">gauge.themes.</span>addToAllThemes (theme)](#apidoc.element.gauge.themes.addToAllThemes)
1.  [function <span class="apidocSignatureSpan">gauge.themes.</span>getDefault (opts)](#apidoc.element.gauge.themes.getDefault)
1.  [function <span class="apidocSignatureSpan">gauge.themes.</span>getTheme (name)](#apidoc.element.gauge.themes.getTheme)
1.  [function <span class="apidocSignatureSpan">gauge.themes.</span>getThemeNames ()](#apidoc.element.gauge.themes.getThemeNames)
1.  [function <span class="apidocSignatureSpan">gauge.themes.</span>newMissingDefaultThemeError (platformName, hasUnicode, hasColor)](#apidoc.element.gauge.themes.newMissingDefaultThemeError)
1.  [function <span class="apidocSignatureSpan">gauge.themes.</span>newMissingThemeError (name)](#apidoc.element.gauge.themes.newMissingThemeError)
1.  [function <span class="apidocSignatureSpan">gauge.themes.</span>newTheme (parent, theme)](#apidoc.element.gauge.themes.newTheme)
1.  [function <span class="apidocSignatureSpan">gauge.themes.</span>newThemeSet ()](#apidoc.element.gauge.themes.newThemeSet)
1.  [function <span class="apidocSignatureSpan">gauge.themes.</span>setDefault (opts, name)](#apidoc.element.gauge.themes.setDefault)
1.  object <span class="apidocSignatureSpan">gauge.</span>themes
1.  object <span class="apidocSignatureSpan">gauge.themes.</span>baseTheme
1.  object <span class="apidocSignatureSpan">gauge.themes.</span>defaults



# <a name="apidoc.module.gauge"></a>[module gauge](#apidoc.module.gauge)

#### <a name="apidoc.element.gauge.plumbing"></a>[function <span class="apidocSignatureSpan">gauge.</span>plumbing (theme, template, width)](#apidoc.element.gauge.plumbing)
- description and source-code
```javascript
plumbing = function (theme, template, width) {
  if (!width) width = 80
  validate('OAN', [theme, template, width])
  this.showing = false
  this.theme = theme
  this.width = width
  this.template = template
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gauge.template_item"></a>[function <span class="apidocSignatureSpan">gauge.</span>template_item (values, outputLength)](#apidoc.element.gauge.template_item)
- description and source-code
```javascript
function TemplateItem(values, outputLength) {
  this.overallOutputLength = outputLength
  this.finished = false
  this.type = null
  this.value = null
  this.length = null
  this.maxLength = null
  this.minLength = null
  this.kerning = null
  this.align = 'left'
  this.padLeft = 0
  this.padRight = 0
  this.index = null
  this.first = null
  this.last = null
  if (typeof values === 'string') {
    this.value = values
  } else {
    for (var prop in values) this[prop] = values[prop]
  }
  // Realize percents
  if (isPercent(this.length)) {
    this.length = Math.round(this.overallOutputLength * percent(this.length))
  }
  if (isPercent(this.minLength)) {
    this.minLength = Math.round(this.overallOutputLength * percent(this.minLength))
  }
  if (isPercent(this.maxLength)) {
    this.maxLength = Math.round(this.overallOutputLength * percent(this.maxLength))
  }
  return this
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gauge.themes"></a>[function <span class="apidocSignatureSpan">gauge.</span>themes (opts)](#apidoc.element.gauge.themes)
- description and source-code
```javascript
themes = function (opts) {
  return themeset.getDefault(opts)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gauge.base_theme"></a>[module gauge.base_theme](#apidoc.module.gauge.base_theme)

#### <a name="apidoc.element.gauge.base_theme.activityIndicator"></a>[function <span class="apidocSignatureSpan">gauge.base_theme.</span>activityIndicator (values, theme, width)](#apidoc.element.gauge.base_theme.activityIndicator)
- description and source-code
```javascript
activityIndicator = function (values, theme, width) {
  if (values.spun == null) return
  return spin(theme, values.spun)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gauge.base_theme.progressbar"></a>[function <span class="apidocSignatureSpan">gauge.base_theme.</span>progressbar (values, theme, width)](#apidoc.element.gauge.base_theme.progressbar)
- description and source-code
```javascript
progressbar = function (values, theme, width) {
  if (values.completed == null) return
  return progressBar(theme, width, values.completed)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gauge.error"></a>[module gauge.error](#apidoc.module.gauge.error)

#### <a name="apidoc.element.gauge.error.Internal"></a>[function <span class="apidocSignatureSpan">gauge.error.</span>Internal (msg)](#apidoc.element.gauge.error.Internal)
- description and source-code
```javascript
function Internal(msg) {
  var err = new Error(msg)
  Error.captureStackTrace(err, Internal)
  err.code = 'EGAUGEINTERNAL'
  return err
}
```
- example usage
```shell
...
function consumeSpace (length) {
  if (length > remainingSpace) length = remainingSpace
  outputLength += length
  remainingSpace -= length
}

function finishSizing (item, length) {
  if (item.finished) throw new error.Internal('Tried to finish template item that was already finished')
  if (length === Infinity) throw new error.Internal('Length of template item cannot be infinity')
  if (length != null) item.length = length
  item.minLength = null
  item.maxLength = null
  --variableCount
  item.finished = true
  if (item.length == null) item.length = item.getBaseLength()
...
```

#### <a name="apidoc.element.gauge.error.MissingTemplateValue"></a>[function <span class="apidocSignatureSpan">gauge.error.</span>MissingTemplateValue (item, values)](#apidoc.element.gauge.error.MissingTemplateValue)
- description and source-code
```javascript
function MissingTemplateValue(item, values) {
  var err = new User(util.format('Missing template value "%s"', item.type))
  Error.captureStackTrace(err, MissingTemplateValue)
  err.template = item
  err.values = values
  return err
}
```
- example usage
```shell
...
function prepareItems (width, template, values) {
function cloneAndObjectify (item, index, arr) {
  var cloned = new TemplateItem(item, width)
  var type = cloned.type
  if (cloned.value == null) {
    if (!(type in values)) {
      if (cloned.default == null) {
        throw new error.MissingTemplateValue(cloned, values)
      } else {
        cloned.value = cloned.default
      }
    } else {
      cloned.value = values[type]
    }
  }
...
```

#### <a name="apidoc.element.gauge.error.User"></a>[function <span class="apidocSignatureSpan">gauge.error.</span>User (msg)](#apidoc.element.gauge.error.User)
- description and source-code
```javascript
function User(msg) {
  var err = new Error(msg)
  Error.captureStackTrace(err, User)
  err.code = 'EGAUGE'
  return err
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gauge.plumbing"></a>[module gauge.plumbing](#apidoc.module.gauge.plumbing)

#### <a name="apidoc.element.gauge.plumbing.plumbing"></a>[function <span class="apidocSignatureSpan">gauge.</span>plumbing (theme, template, width)](#apidoc.element.gauge.plumbing.plumbing)
- description and source-code
```javascript
plumbing = function (theme, template, width) {
  if (!width) width = 80
  validate('OAN', [theme, template, width])
  this.showing = false
  this.theme = theme
  this.width = width
  this.template = template
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gauge.plumbing.prototype"></a>[module gauge.plumbing.prototype](#apidoc.module.gauge.plumbing.prototype)

#### <a name="apidoc.element.gauge.plumbing.prototype.hide"></a>[function <span class="apidocSignatureSpan">gauge.plumbing.prototype.</span>hide ()](#apidoc.element.gauge.plumbing.prototype.hide)
- description and source-code
```javascript
hide = function () {
  return consoleControl.gotoSOL() + consoleControl.eraseLine()
}
```
- example usage
```shell
...

var gauge = new Gauge()

gauge.show("test", 0.20)

gauge.pulse("this")

gauge.hide()
'''

![](gauge-demo.gif)


### CHANGES FROM 1.x
...
```

#### <a name="apidoc.element.gauge.plumbing.prototype.hideCursor"></a>[function <span class="apidocSignatureSpan">gauge.plumbing.prototype.</span>hideCursor ()](#apidoc.element.gauge.plumbing.prototype.hideCursor)
- description and source-code
```javascript
function hideCursor() {
  return prefix + '?25l'
}
```
- example usage
```shell
...

Change the width to render at.

#### 'gauge.hide()'

Return the string necessary to hide the progress bar

#### 'gauge.hideCursor()'

Return a string to hide the cursor.

#### 'gauge.showCursor()'

Return a string to show the cursor.
...
```

#### <a name="apidoc.element.gauge.plumbing.prototype.setTemplate"></a>[function <span class="apidocSignatureSpan">gauge.plumbing.prototype.</span>setTemplate (template)](#apidoc.element.gauge.plumbing.prototype.setTemplate)
- description and source-code
```javascript
setTemplate = function (template) {
  validate('A', [template])
  this.template = template
}
```
- example usage
```shell
...
* A configuration object with any of 'hasUnicode', 'hasColor' or
  'platform' keys, which if wlll be used to override our guesses when making
  a default theme selection.

If no theme is selected then a default is picked using a combination of our
best guesses at your OS, color support and unicode support.

#### 'gauge.setTemplate(template)'

Change the active template, will be displayed with the next show or pulse

### Tracking Completion

If you have more than one thing going on that you want to track completion
of, you may find the related [are-we-there-yet] helpful.  It's 'change'
...
```

#### <a name="apidoc.element.gauge.plumbing.prototype.setTheme"></a>[function <span class="apidocSignatureSpan">gauge.plumbing.prototype.</span>setTheme (theme)](#apidoc.element.gauge.plumbing.prototype.setTheme)
- description and source-code
```javascript
setTheme = function (theme) {
  validate('O', [theme])
  this.theme = theme
}
```
- example usage
```shell
...
Returns true if the gauge is enabled.

#### 'gauge.setThemeset(themes)'

Change the themeset to select a theme from. The same as the 'themes' option
used in the constructor. The theme will be reselected from this themeset.

#### 'gauge.setTheme(theme)'

Change the active theme, will be displayed with the next show or pulse. This can be:

* Theme object, in which case the **themes** is not used.
* The name of a theme, which will be looked up in the current *themes*
  object.
* A configuration object with any of 'hasUnicode', 'hasColor' or
...
```

#### <a name="apidoc.element.gauge.plumbing.prototype.setWidth"></a>[function <span class="apidocSignatureSpan">gauge.plumbing.prototype.</span>setWidth (width)](#apidoc.element.gauge.plumbing.prototype.setWidth)
- description and source-code
```javascript
setWidth = function (width) {
  validate('N', [width])
  this.width = width
}
```
- example usage
```shell
...

Change the active theme.

#### 'gauge.setTemplate(template)'

Change the active template.

#### 'gauge.setWidth(width)'

Change the width to render at.

#### 'gauge.hide()'

Return the string necessary to hide the progress bar
...
```

#### <a name="apidoc.element.gauge.plumbing.prototype.show"></a>[function <span class="apidocSignatureSpan">gauge.plumbing.prototype.</span>show (status)](#apidoc.element.gauge.plumbing.prototype.show)
- description and source-code
```javascript
show = function (status) {
  var values = Object.create(this.theme)
  for (var key in status) {
    values[key] = status[key]
  }

  return renderTemplate(this.width, this.template, values).trim() +
         consoleControl.eraseLine() + consoleControl.gotoSOL()
}
```
- example usage
```shell
...
A nearly stateless terminal based horizontal gauge / progress bar.

'''javascript
var Gauge = require("gauge")

var gauge = new Gauge()

gauge.show("test", 0.20)

gauge.pulse("this")

gauge.hide()
'''

![](gauge-demo.gif)
...
```

#### <a name="apidoc.element.gauge.plumbing.prototype.showCursor"></a>[function <span class="apidocSignatureSpan">gauge.plumbing.prototype.</span>showCursor ()](#apidoc.element.gauge.plumbing.prototype.showCursor)
- description and source-code
```javascript
function showCursor() {
  return prefix + '?25h'
}
```
- example usage
```shell
...

Return the string necessary to hide the progress bar

#### 'gauge.hideCursor()'

Return a string to hide the cursor.

#### 'gauge.showCursor()'

Return a string to show the cursor.

#### 'gauge.show(status)'

Using 'status' for values, render the provided template with the theme and return
a string that is suitable for printing to update the gauge.
...
```



# <a name="apidoc.module.gauge.template_item"></a>[module gauge.template_item](#apidoc.module.gauge.template_item)

#### <a name="apidoc.element.gauge.template_item.template_item"></a>[function <span class="apidocSignatureSpan">gauge.</span>template_item (values, outputLength)](#apidoc.element.gauge.template_item.template_item)
- description and source-code
```javascript
function TemplateItem(values, outputLength) {
  this.overallOutputLength = outputLength
  this.finished = false
  this.type = null
  this.value = null
  this.length = null
  this.maxLength = null
  this.minLength = null
  this.kerning = null
  this.align = 'left'
  this.padLeft = 0
  this.padRight = 0
  this.index = null
  this.first = null
  this.last = null
  if (typeof values === 'string') {
    this.value = values
  } else {
    for (var prop in values) this[prop] = values[prop]
  }
  // Realize percents
  if (isPercent(this.length)) {
    this.length = Math.round(this.overallOutputLength * percent(this.length))
  }
  if (isPercent(this.minLength)) {
    this.minLength = Math.round(this.overallOutputLength * percent(this.minLength))
  }
  if (isPercent(this.maxLength)) {
    this.maxLength = Math.round(this.overallOutputLength * percent(this.maxLength))
  }
  return this
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gauge.template_item.prototype"></a>[module gauge.template_item.prototype](#apidoc.module.gauge.template_item.prototype)

#### <a name="apidoc.element.gauge.template_item.prototype.getBaseLength"></a>[function <span class="apidocSignatureSpan">gauge.template_item.prototype.</span>getBaseLength ()](#apidoc.element.gauge.template_item.prototype.getBaseLength)
- description and source-code
```javascript
getBaseLength = function () {
  var length = this.length
  if (length == null && typeof this.value === 'string' && this.maxLength == null && this.minLength == null) {
    length = stringWidth(this.value)
  }
  return length
}
```
- example usage
```shell
...
  if (item.finished) throw new error.Internal('Tried to finish template item that was already finished')
  if (length === Infinity) throw new error.Internal('Length of template item cannot be infinity')
  if (length != null) item.length = length
  item.minLength = null
  item.maxLength = null
  --variableCount
  item.finished = true
  if (item.length == null) item.length = item.getBaseLength()
  if (item.length == null) throw new error.Internal('Finished template items must have a length')
  consumeSpace(item.getLength())
}

output.forEach(function (item) {
  if (!item.kerning) return
  var prevPadRight = item.first ? 0 : output[item.index - 1].padRight
...
```

#### <a name="apidoc.element.gauge.template_item.prototype.getLength"></a>[function <span class="apidocSignatureSpan">gauge.template_item.prototype.</span>getLength ()](#apidoc.element.gauge.template_item.prototype.getLength)
- description and source-code
```javascript
getLength = function () {
  var length = this.getBaseLength()
  if (length == null) return null
  return length + this.padLeft + this.padRight
}
```
- example usage
```shell
...
  if (length != null) item.length = length
  item.minLength = null
  item.maxLength = null
  --variableCount
  item.finished = true
  if (item.length == null) item.length = item.getBaseLength()
  if (item.length == null) throw new error.Internal('Finished template items must have a length')
  consumeSpace(item.getLength())
}

output.forEach(function (item) {
  if (!item.kerning) return
  var prevPadRight = item.first ? 0 : output[item.index - 1].padRight
  if (!item.first && prevPadRight < item.kerning) item.padLeft = item.kerning - prevPadRight
  if (!item.last) item.padRight = item.kerning
...
```

#### <a name="apidoc.element.gauge.template_item.prototype.getMaxLength"></a>[function <span class="apidocSignatureSpan">gauge.template_item.prototype.</span>getMaxLength ()](#apidoc.element.gauge.template_item.prototype.getMaxLength)
- description and source-code
```javascript
getMaxLength = function () {
  if (this.maxLength == null) return null
  return this.maxLength + this.padLeft + this.padRight
}
```
- example usage
```shell
...
var hunkSize
do {
  resizing = false
  hunkSize = Math.round(remainingSpace / variableCount)
  output.forEach(function (item) {
    if (item.finished) return
    if (!item.maxLength) return
    if (item.getMaxLength() < hunkSize) {
      finishSizing(item, item.maxLength)
      resizing = true
    }
  })
} while (resizing && resized++ < output.length)
if (resizing) throw new error.Internal('Resize loop iterated too many times while determining maxLength')
...
```

#### <a name="apidoc.element.gauge.template_item.prototype.getMinLength"></a>[function <span class="apidocSignatureSpan">gauge.template_item.prototype.</span>getMinLength ()](#apidoc.element.gauge.template_item.prototype.getMinLength)
- description and source-code
```javascript
getMinLength = function () {
  if (this.minLength == null) return null
  return this.minLength + this.padLeft + this.padRight
}
```
- example usage
```shell
...
resized = 0
do {
  resizing = false
  hunkSize = Math.round(remainingSpace / variableCount)
  output.forEach(function (item) {
    if (item.finished) return
    if (!item.minLength) return
    if (item.getMinLength() >= hunkSize) {
      finishSizing(item, item.minLength)
      resizing = true
    }
  })
} while (resizing && resized++ < output.length)
if (resizing) throw new error.Internal('Resize loop iterated too many times while determining minLength')
...
```



# <a name="apidoc.module.gauge.themes"></a>[module gauge.themes](#apidoc.module.gauge.themes)

#### <a name="apidoc.element.gauge.themes.addTheme"></a>[function <span class="apidocSignatureSpan">gauge.themes.</span>addTheme (name, parent, theme)](#apidoc.element.gauge.themes.addTheme)
- description and source-code
```javascript
addTheme = function (name, parent, theme) {
  this.themes[name] = this.newTheme(parent, theme)
}
```
- example usage
```shell
...
  available a non-color theme will be used.
* **platform** (optional) - Defaults to 'process.platform'.  If no
  platform match is available then 'fallback' is used instead.

If no compatible theme can be found then an error will be thrown with a
'code' of 'EMISSINGTHEME'.

#### themes.addTheme(themeName, themeObj)
#### themes.addTheme(themeName, [parentTheme], newTheme)

Adds a named theme to the themeset.  You can pass in either a theme object,
as returned by 'themes.newTheme' or the arguments you'd pass to
'themes.newTheme'.

#### themes.getThemeNames()
...
```

#### <a name="apidoc.element.gauge.themes.addToAllThemes"></a>[function <span class="apidocSignatureSpan">gauge.themes.</span>addToAllThemes (theme)](#apidoc.element.gauge.themes.addToAllThemes)
- description and source-code
```javascript
addToAllThemes = function (theme) {
  var themes = this.themes
  Object.keys(themes).forEach(function (name) {
    objectAssign(themes[name], theme)
  })
  objectAssign(this.baseTheme, theme)
}
```
- example usage
```shell
...
* **pre** - Is shown prior to the property, if its displayed.
* **post** - Is shown after the property, if its displayed.

And one special suffix:

* **Theme** - Its value is passed to a function-type item as the theme.

#### themes.addToAllThemes(theme)

This *mixes-in* 'theme' into all themes currently defined. It also adds it
to the default parent theme for this themeset, so future themes added to
this themeset will get the values from 'theme' by default.

#### themes.newThemeset()
...
```

#### <a name="apidoc.element.gauge.themes.getDefault"></a>[function <span class="apidocSignatureSpan">gauge.themes.</span>getDefault (opts)](#apidoc.element.gauge.themes.getDefault)
- description and source-code
```javascript
getDefault = function (opts) {
  if (!opts) opts = {}
  var platformName = opts.platform || process.platform
  var platform = this.defaults[platformName] || this.defaults.fallback
  var hasUnicode = !!opts.hasUnicode
  var hasColor = !!opts.hasColor
  if (!platform) throw this.newMissingDefaultThemeError(platformName, hasUnicode, hasColor)
  if (!platform[hasUnicode][hasColor]) {
    if (hasUnicode && hasColor && platform[!hasUnicode][hasColor]) {
      hasUnicode = false
    } else if (hasUnicode && hasColor && platform[hasUnicode][!hasColor]) {
      hasColor = false
    } else if (hasUnicode && hasColor && platform[!hasUnicode][!hasColor]) {
      hasUnicode = false
      hasColor = false
    } else if (hasUnicode && !hasColor && platform[!hasUnicode][hasColor]) {
      hasUnicode = false
    } else if (!hasUnicode && hasColor && platform[hasUnicode][!hasColor]) {
      hasColor = false
    } else if (platform === this.defaults.fallback) {
      throw this.newMissingDefaultThemeError(platformName, hasUnicode, hasColor)
    }
  }
  if (platform[hasUnicode][hasColor]) {
    return this.getTheme(platform[hasUnicode][hasColor])
  } else {
    return this.getDefault(objectAssign({}, opts, {platform: 'fallback'}))
  }
}
```
- example usage
```shell
...
var themes = new ThemeSet()
// or
var themes = require('gauge/themes')
var mythemes = themes.newThemeset() // creates a new themeset based on the default themes
'''

#### themes(opts)
#### themes.getDefault(opts)

Theme objects are a function that fetches the default theme based on
platform, unicode and color support.

Options is an object with the following properties:

* **hasUnicode** - If true, fetch a unicode theme, if no unicode theme is
...
```

#### <a name="apidoc.element.gauge.themes.getTheme"></a>[function <span class="apidocSignatureSpan">gauge.themes.</span>getTheme (name)](#apidoc.element.gauge.themes.getTheme)
- description and source-code
```javascript
getTheme = function (name) {
  if (!this.themes[name]) throw this.newMissingThemeError(name)
  return this.themes[name]
}
```
- example usage
```shell
...
Adds a named theme to the themeset.  You can pass in either a theme object,
as returned by 'themes.newTheme' or the arguments you'd pass to
'themes.newTheme'.

#### themes.getThemeNames()

Return a list of all of the names of the themes in this themeset. Suitable
for use in 'themes.getTheme(…)'.

#### themes.getTheme(name)

Returns the theme object from this theme set named 'name'.

If 'name' does not exist in this themeset an error will be thrown with
a 'code' of 'EMISSINGTHEME'.
...
```

#### <a name="apidoc.element.gauge.themes.getThemeNames"></a>[function <span class="apidocSignatureSpan">gauge.themes.</span>getThemeNames ()](#apidoc.element.gauge.themes.getThemeNames)
- description and source-code
```javascript
getThemeNames = function () {
  return Object.keys(this.themes)
}
```
- example usage
```shell
...
#### themes.addTheme(themeName, themeObj)
#### themes.addTheme(themeName, [parentTheme], newTheme)

Adds a named theme to the themeset.  You can pass in either a theme object,
as returned by 'themes.newTheme' or the arguments you'd pass to
'themes.newTheme'.

#### themes.getThemeNames()

Return a list of all of the names of the themes in this themeset. Suitable
for use in 'themes.getTheme(…)'.

#### themes.getTheme(name)

Returns the theme object from this theme set named 'name'.
...
```

#### <a name="apidoc.element.gauge.themes.newMissingDefaultThemeError"></a>[function <span class="apidocSignatureSpan">gauge.themes.</span>newMissingDefaultThemeError (platformName, hasUnicode, hasColor)](#apidoc.element.gauge.themes.newMissingDefaultThemeError)
- description and source-code
```javascript
function newMissingDefaultThemeError(platformName, hasUnicode, hasColor) {
  var err = new Error(
    'Could not find a gauge theme for your platform/unicode/color use combo:\n' +
    '    platform = ' + platformName + '\n' +
    '    hasUnicode = ' + hasUnicode + '\n' +
    '    hasColor = ' + hasColor)
  Error.captureStackTrace.call(err, newMissingDefaultThemeError)
  err.platform = platformName
  err.hasUnicode = hasUnicode
  err.hasColor = hasColor
  err.code = 'EMISSINGTHEME'
  return err
}
```
- example usage
```shell
...

ThemeSetProto.getDefault = function (opts) {
if (!opts) opts = {}
var platformName = opts.platform || process.platform
var platform = this.defaults[platformName] || this.defaults.fallback
var hasUnicode = !!opts.hasUnicode
var hasColor = !!opts.hasColor
if (!platform) throw this.newMissingDefaultThemeError(platformName, hasUnicode, hasColor)
if (!platform[hasUnicode][hasColor]) {
  if (hasUnicode && hasColor && platform[!hasUnicode][hasColor]) {
    hasUnicode = false
  } else if (hasUnicode && hasColor && platform[hasUnicode][!hasColor]) {
    hasColor = false
  } else if (hasUnicode && hasColor && platform[!hasUnicode][!hasColor]) {
    hasUnicode = false
...
```

#### <a name="apidoc.element.gauge.themes.newMissingThemeError"></a>[function <span class="apidocSignatureSpan">gauge.themes.</span>newMissingThemeError (name)](#apidoc.element.gauge.themes.newMissingThemeError)
- description and source-code
```javascript
function newMissingThemeError(name) {
  var err = new Error('Could not find a gauge theme named "' + name + '"')
  Error.captureStackTrace.call(err, newMissingThemeError)
  err.theme = name
  err.code = 'EMISSINGTHEME'
  return err
}
```
- example usage
```shell
...
Object.keys(themes).forEach(function (name) {
  objectAssign(themes[name], theme)
})
objectAssign(this.baseTheme, theme)
}

ThemeSetProto.getTheme = function (name) {
if (!this.themes[name]) throw this.newMissingThemeError(name)
return this.themes[name]
}

ThemeSetProto.setDefault = function (opts, name) {
if (name == null) {
  name = opts
  opts = {}
...
```

#### <a name="apidoc.element.gauge.themes.newTheme"></a>[function <span class="apidocSignatureSpan">gauge.themes.</span>newTheme (parent, theme)](#apidoc.element.gauge.themes.newTheme)
- description and source-code
```javascript
newTheme = function (parent, theme) {
  if (!theme) {
    theme = parent
    parent = this.baseTheme
  }
  return objectAssign({}, parent, theme)
}
```
- example usage
```shell
...
var ourTheme = themes({hasUnicode: true, hasColor: true})

// fetch the default non-color unicode theme for osx
var ourTheme = themes({hasUnicode: true, hasColor: false, platform: 'darwin'})

// create a new theme based on the color ascii theme for this platform
// that brackets the progress bar with arrows
var ourTheme = themes.newTheme(theme(hasUnicode: false, hasColor: true}), {
  preProgressbar: '→',
  postProgressbar: '←'
})
'''

The object returned by 'gauge/themes' is an instance of the 'ThemeSet' class.
...
```

#### <a name="apidoc.element.gauge.themes.newThemeSet"></a>[function <span class="apidocSignatureSpan">gauge.themes.</span>newThemeSet ()](#apidoc.element.gauge.themes.newThemeSet)
- description and source-code
```javascript
newThemeSet = function () {
  var themeset = function (opts) {
    return themeset.getDefault(opts)
  }
  return objectAssign(themeset, ThemeSetProto, {
    themes: objectAssign({}, this.themes),
    baseTheme: objectAssign({}, this.baseTheme),
    defaults: JSON.parse(JSON.stringify(this.defaults || {}))
  })
}
```
- example usage
```shell
...



'use strict'
var objectAssign = require('object-assign')

module.exports = function () {
  return ThemeSetProto.newThemeSet()
}

var ThemeSetProto = {}

ThemeSetProto.baseTheme = require('./base-theme.js')

ThemeSetProto.newTheme = function (parent, theme) {
...
```

#### <a name="apidoc.element.gauge.themes.setDefault"></a>[function <span class="apidocSignatureSpan">gauge.themes.</span>setDefault (opts, name)](#apidoc.element.gauge.themes.setDefault)
- description and source-code
```javascript
setDefault = function (opts, name) {
  if (name == null) {
    name = opts
    opts = {}
  }
  var platform = opts.platform == null ? 'fallback' : opts.platform
  var hasUnicode = !!opts.hasUnicode
  var hasColor = !!opts.hasColor
  if (!this.defaults[platform]) this.defaults[platform] = {true: {}, false: {}}
  this.defaults[platform][hasUnicode][hasColor] = name
}
```
- example usage
```shell
...
#### themes.getTheme(name)

Returns the theme object from this theme set named 'name'.

If 'name' does not exist in this themeset an error will be thrown with
a 'code' of 'EMISSINGTHEME'.

#### themes.setDefault([opts], themeName)

'opts' is an object with the following properties.

* **platform** - Defaults to ''fallback''.  If your theme is platform
  specific, specify that here with the platform from 'process.platform', eg,
  'win32', 'darwin', etc.
* **hasUnicode** - Defaults to 'false'. If your theme uses unicode you
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
