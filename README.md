# api documentation for  [protractor (v5.1.1)](https://github.com/angular/protractor)  [![npm package](https://img.shields.io/npm/v/npmdoc-protractor.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-protractor) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-protractor.svg)](https://travis-ci.org/npmdoc/node-npmdoc-protractor)
#### Webdriver E2E test wrapper for Angular.

[![NPM](https://nodei.co/npm/protractor.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/protractor)

[![apidoc](https://npmdoc.github.io/node-npmdoc-protractor/build/screenCapture.buildCi.browser.apidoc.html.png)](https://npmdoc.github.io/node-npmdoc-protractor/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-protractor/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-protractor/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Julie Ralph"
    },
    "bin": {
        "protractor": "bin/protractor",
        "webdriver-manager": "bin/webdriver-manager"
    },
    "bugs": {
        "url": "https://github.com/angular/protractor/issues"
    },
    "dependencies": {
        "@types/node": "^6.0.46",
        "@types/q": "^0.0.32",
        "@types/selenium-webdriver": "~2.53.39",
        "blocking-proxy": "0.0.5",
        "chalk": "^1.1.3",
        "glob": "^7.0.3",
        "jasmine": "^2.5.3",
        "jasminewd2": "^2.0.0",
        "optimist": "~0.6.0",
        "q": "1.4.1",
        "saucelabs": "~1.3.0",
        "selenium-webdriver": "3.0.1",
        "source-map-support": "~0.4.0",
        "webdriver-js-extender": "^1.0.0",
        "webdriver-manager": "^12.0.1"
    },
    "description": "Webdriver E2E test wrapper for Angular.",
    "devDependencies": {
        "@types/chalk": "^0.4.28",
        "@types/glob": "^5.0.29",
        "@types/jasmine": "^2.5.38",
        "@types/jasminewd2": "^2.0.0",
        "@types/minimatch": "^2.0.28",
        "@types/minimist": "^1.1.28",
        "@types/optimist": "^0.0.29",
        "body-parser": "~1.15.2",
        "chai": "~3.5.0",
        "chai-as-promised": "~5.3.0",
        "clang-format": "^1.0.34",
        "expect.js": "~0.3.1",
        "express": "~4.14.0",
        "gulp": "^3.9.1",
        "gulp-clang-format": "^1.0.23",
        "gulp-tslint": "^7.0.1",
        "jshint": "^2.9.2",
        "lodash": "^4.5.1",
        "marked": "^0.3.3",
        "mocha": "2.5.3",
        "rimraf": "~2.5.3",
        "run-sequence": "^1.1.5",
        "semver": "^5.3.0",
        "tslint": "~4.3.0",
        "tslint-eslint-rules": "^3.2.0",
        "typescript": "~2.0.0",
        "vrsource-tslint-rules": "^4.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "10c4e336571b28875b8acc3ae3e4e1e40ef7e986",
        "tarball": "https://registry.npmjs.org/protractor/-/protractor-5.1.1.tgz"
    },
    "engines": {
        "node": ">=6.9.x"
    },
    "gitHead": "ba544224f6cfe07b8bf3a75772835d72f397cabc",
    "homepage": "https://github.com/angular/protractor",
    "keywords": [
        "angular",
        "test",
        "testing",
        "webdriver",
        "webdriverjs",
        "selenium"
    ],
    "license": "MIT",
    "main": "built/index.js",
    "maintainers": [
        {
            "name": "juliemr"
        },
        {
            "name": "angularcore"
        }
    ],
    "name": "protractor",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/angular/protractor.git"
    },
    "scripts": {
        "format": "gulp format",
        "install_testapp": "cd testapp && npm install",
        "prepublish": "gulp prepublish",
        "pretest": "gulp pretest",
        "start": "cd testapp && npm start",
        "test": "node scripts/test.js",
        "website": "cd website && npm start"
    },
    "typings": "built/index.d.ts",
    "version": "5.1.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module protractor](#apidoc.module.protractor)
1.  [function <span class="apidocSignatureSpan">protractor.</span>ActionSequence (driver)](#apidoc.element.protractor.ActionSequence)
1.  [function <span class="apidocSignatureSpan">protractor.</span>Builder ()](#apidoc.element.protractor.Builder)
1.  [function <span class="apidocSignatureSpan">protractor.</span>Capabilities (Capabilities|Map<string, ?>|Object)](#apidoc.element.protractor.Capabilities)
1.  [function <span class="apidocSignatureSpan">protractor.</span>Command (name)](#apidoc.element.protractor.Command)
1.  [function <span class="apidocSignatureSpan">protractor.</span>ElementArrayFinder (browser_, getWebElements = null, locator_, actionResults_ = null)](#apidoc.element.protractor.ElementArrayFinder)
1.  [function <span class="apidocSignatureSpan">protractor.</span>ElementFinder (browser_, elementArrayFinder)](#apidoc.element.protractor.ElementFinder)
1.  [function <span class="apidocSignatureSpan">protractor.</span>EventEmitter (type, var_args)](#apidoc.element.protractor.EventEmitter)
1.  [function <span class="apidocSignatureSpan">protractor.</span>FileDetector (driver, path)](#apidoc.element.protractor.FileDetector)
1.  [function <span class="apidocSignatureSpan">protractor.</span>ProtractorBrowser (webdriverInstance, opt_baseUrl, opt_rootElement, opt_untrackOutstandingTimeouts, opt_blockingProxyUrl)](#apidoc.element.protractor.ProtractorBrowser)
1.  [function <span class="apidocSignatureSpan">protractor.</span>ProtractorBy (by.locatorName(args)](#apidoc.element.protractor.ProtractorBy)
1.  [function <span class="apidocSignatureSpan">protractor.</span>ProtractorExpectedConditions (browser)](#apidoc.element.protractor.ProtractorExpectedConditions)
1.  [function <span class="apidocSignatureSpan">protractor.</span>Ptor ()](#apidoc.element.protractor.Ptor)
1.  [function <span class="apidocSignatureSpan">protractor.</span>Session (Object|Capabilities)](#apidoc.element.protractor.Session)
1.  [function <span class="apidocSignatureSpan">protractor.</span>WebDriver (Session|IThenable<!Session>)](#apidoc.element.protractor.WebDriver)
1.  [function <span class="apidocSignatureSpan">protractor.</span>WebElement (!IThenable<string>|string)](#apidoc.element.protractor.WebElement)
1.  [function <span class="apidocSignatureSpan">protractor.</span>WebElementPromise (driver, el)](#apidoc.element.protractor.WebElementPromise)
1.  object <span class="apidocSignatureSpan">protractor.</span>Browser
1.  object <span class="apidocSignatureSpan">protractor.</span>Button
1.  object <span class="apidocSignatureSpan">protractor.</span>Capability
1.  object <span class="apidocSignatureSpan">protractor.</span>CommandName
1.  object <span class="apidocSignatureSpan">protractor.</span>Key
1.  object <span class="apidocSignatureSpan">protractor.</span>error
1.  object <span class="apidocSignatureSpan">protractor.</span>logging
1.  object <span class="apidocSignatureSpan">protractor.</span>promise
1.  object <span class="apidocSignatureSpan">protractor.</span>until
1.  object <span class="apidocSignatureSpan">protractor.</span>utils

#### [module protractor.Key](#apidoc.module.protractor.Key)
1.  [function <span class="apidocSignatureSpan">protractor.Key.</span>chord (var_args)](#apidoc.element.protractor.Key.chord)
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>ADD
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>ALT
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>ARROW_DOWN
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>ARROW_LEFT
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>ARROW_RIGHT
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>ARROW_UP
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>BACK_SPACE
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>CANCEL
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>CLEAR
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>COMMAND
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>CONTROL
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>DECIMAL
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>DELETE
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>DIVIDE
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>DOWN
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>END
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>ENTER
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>EQUALS
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>ESCAPE
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>F1
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>F10
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>F11
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>F12
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>F2
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>F3
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>F4
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>F5
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>F6
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>F7
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>F8
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>F9
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>HELP
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>HOME
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>INSERT
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>LEFT
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>META
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>MULTIPLY
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>NULL
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>NUMPAD0
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>NUMPAD1
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>NUMPAD2
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>NUMPAD3
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>NUMPAD4
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>NUMPAD5
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>NUMPAD6
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>NUMPAD7
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>NUMPAD8
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>NUMPAD9
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>PAGE_DOWN
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>PAGE_UP
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>PAUSE
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>RETURN
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>RIGHT
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>SEMICOLON
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>SEPARATOR
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>SHIFT
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>SPACE
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>SUBTRACT
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>TAB
1.  string <span class="apidocSignatureSpan">protractor.Key.</span>UP

#### [module protractor.error](#apidoc.module.protractor.error)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>ElementNotSelectableError (opt_error)](#apidoc.element.protractor.error.ElementNotSelectableError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>ElementNotVisibleError (opt_error)](#apidoc.element.protractor.error.ElementNotVisibleError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>InvalidArgumentError (opt_error)](#apidoc.element.protractor.error.InvalidArgumentError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>InvalidCookieDomainError (opt_error)](#apidoc.element.protractor.error.InvalidCookieDomainError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>InvalidElementCoordinatesError (opt_error)](#apidoc.element.protractor.error.InvalidElementCoordinatesError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>InvalidElementStateError (opt_error)](#apidoc.element.protractor.error.InvalidElementStateError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>InvalidSelectorError (opt_error)](#apidoc.element.protractor.error.InvalidSelectorError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>JavascriptError (opt_error)](#apidoc.element.protractor.error.JavascriptError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>MoveTargetOutOfBoundsError (opt_error)](#apidoc.element.protractor.error.MoveTargetOutOfBoundsError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>NoSuchAlertError (opt_error)](#apidoc.element.protractor.error.NoSuchAlertError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>NoSuchElementError (opt_error)](#apidoc.element.protractor.error.NoSuchElementError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>NoSuchFrameError (opt_error)](#apidoc.element.protractor.error.NoSuchFrameError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>NoSuchSessionError (opt_error)](#apidoc.element.protractor.error.NoSuchSessionError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>NoSuchWindowError (opt_error)](#apidoc.element.protractor.error.NoSuchWindowError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>ScriptTimeoutError (opt_error)](#apidoc.element.protractor.error.ScriptTimeoutError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>SessionNotCreatedError (opt_error)](#apidoc.element.protractor.error.SessionNotCreatedError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>StaleElementReferenceError (opt_error)](#apidoc.element.protractor.error.StaleElementReferenceError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>TimeoutError (opt_error)](#apidoc.element.protractor.error.TimeoutError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>UnableToCaptureScreenError (opt_error)](#apidoc.element.protractor.error.UnableToCaptureScreenError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>UnableToSetCookieError (opt_error)](#apidoc.element.protractor.error.UnableToSetCookieError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>UnexpectedAlertOpenError (opt_error, opt_text)](#apidoc.element.protractor.error.UnexpectedAlertOpenError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>UnknownCommandError (opt_error)](#apidoc.element.protractor.error.UnknownCommandError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>UnknownMethodError (opt_error)](#apidoc.element.protractor.error.UnknownMethodError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>UnsupportedOperationError (opt_error)](#apidoc.element.protractor.error.UnsupportedOperationError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>WebDriverError (opt_error)](#apidoc.element.protractor.error.WebDriverError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>checkLegacyResponse (responseObj)](#apidoc.element.protractor.error.checkLegacyResponse)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>checkResponse (data)](#apidoc.element.protractor.error.checkResponse)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>encodeError (err)](#apidoc.element.protractor.error.encodeError)
1.  [function <span class="apidocSignatureSpan">protractor.error.</span>throwDecodedError (data)](#apidoc.element.protractor.error.throwDecodedError)
1.  object <span class="apidocSignatureSpan">protractor.error.</span>ErrorCode

#### [module protractor.logging](#apidoc.module.protractor.logging)
1.  [function <span class="apidocSignatureSpan">protractor.logging.</span>Entry (!Level|string|number)](#apidoc.element.protractor.logging.Entry)
1.  [function <span class="apidocSignatureSpan">protractor.logging.</span>Level (name, level)](#apidoc.element.protractor.logging.Level)
1.  [function <span class="apidocSignatureSpan">protractor.logging.</span>LogManager ()](#apidoc.element.protractor.logging.LogManager)
1.  [function <span class="apidocSignatureSpan">protractor.logging.</span>Logger (name, opt_level)](#apidoc.element.protractor.logging.Logger)
1.  [function <span class="apidocSignatureSpan">protractor.logging.</span>Preferences ()](#apidoc.element.protractor.logging.Preferences)
1.  [function <span class="apidocSignatureSpan">protractor.logging.</span>addConsoleHandler (opt_logger)](#apidoc.element.protractor.logging.addConsoleHandler)
1.  [function <span class="apidocSignatureSpan">protractor.logging.</span>getLevel (nameOrValue)](#apidoc.element.protractor.logging.getLevel)
1.  [function <span class="apidocSignatureSpan">protractor.logging.</span>getLogger (name)](#apidoc.element.protractor.logging.getLogger)
1.  [function <span class="apidocSignatureSpan">protractor.logging.</span>installConsoleHandler ()](#apidoc.element.protractor.logging.installConsoleHandler)
1.  [function <span class="apidocSignatureSpan">protractor.logging.</span>removeConsoleHandler (opt_logger)](#apidoc.element.protractor.logging.removeConsoleHandler)
1.  object <span class="apidocSignatureSpan">protractor.logging.</span>Type

#### [module protractor.promise](#apidoc.module.protractor.promise)
1.  boolean <span class="apidocSignatureSpan">protractor.promise.</span>LONG_STACK_TRACES
1.  boolean <span class="apidocSignatureSpan">protractor.promise.</span>USE_PROMISE_MANAGER
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>CancellableThenable (new: CancellableThenable, ...?)](#apidoc.element.protractor.promise.CancellableThenable)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>CancellationError (opt_msg)](#apidoc.element.protractor.promise.CancellationError)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>ControlFlow ()](#apidoc.element.protractor.promise.ControlFlow)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>Deferred (opt_flow)](#apidoc.element.protractor.promise.Deferred)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>MultipleUnhandledRejectionError (Set<*>)](#apidoc.element.protractor.promise.MultipleUnhandledRejectionError)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>Promise ( * function((T|IThenable<T>|Thenable)](#apidoc.element.protractor.promise.Promise)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>Scheduler ()](#apidoc.element.protractor.promise.Scheduler)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>Thenable (new: Thenable, ...?)](#apidoc.element.protractor.promise.Thenable)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>all (arr)](#apidoc.element.protractor.promise.all)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>asap (value, callback, opt_errback)](#apidoc.element.protractor.promise.asap)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>captureStackTrace (name, msg, opt_topFn)](#apidoc.element.protractor.promise.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>checkedNodeCall (fn, var_args)](#apidoc.element.protractor.promise.checkedNodeCall)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>consume (generatorFn, opt_self, ...var_args)](#apidoc.element.protractor.promise.consume)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>controlFlow ()](#apidoc.element.protractor.promise.controlFlow)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>createFlow (callback)](#apidoc.element.protractor.promise.createFlow)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>defer ()](#apidoc.element.protractor.promise.defer)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>delayed (ms)](#apidoc.element.protractor.promise.delayed)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>filter (arr, fn, opt_self)](#apidoc.element.protractor.promise.filter)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>finally (promise, callback)](#apidoc.element.protractor.promise.finally)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>fulfilled (opt_value)](#apidoc.element.protractor.promise.fulfilled)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>fullyResolved (value)](#apidoc.element.protractor.promise.fullyResolved)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>isGenerator (fn)](#apidoc.element.protractor.promise.isGenerator)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>isPromise (value)](#apidoc.element.protractor.promise.isPromise)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>map (arr, fn, opt_self)](#apidoc.element.protractor.promise.map)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>rejected (opt_reason)](#apidoc.element.protractor.promise.rejected)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>setDefaultFlow (flow)](#apidoc.element.protractor.promise.setDefaultFlow)
1.  [function <span class="apidocSignatureSpan">protractor.promise.</span>when (value, opt_callback, opt_errback)](#apidoc.element.protractor.promise.when)

#### [module protractor.until](#apidoc.module.protractor.until)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>ableToSwitchToFrame (frame)](#apidoc.element.protractor.until.ableToSwitchToFrame)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>alertIsPresent ()](#apidoc.element.protractor.until.alertIsPresent)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>elementIsDisabled (element)](#apidoc.element.protractor.until.elementIsDisabled)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>elementIsEnabled (element)](#apidoc.element.protractor.until.elementIsEnabled)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>elementIsNotSelected (element)](#apidoc.element.protractor.until.elementIsNotSelected)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>elementIsNotVisible (element)](#apidoc.element.protractor.until.elementIsNotVisible)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>elementIsSelected (element)](#apidoc.element.protractor.until.elementIsSelected)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>elementIsVisible (element)](#apidoc.element.protractor.until.elementIsVisible)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>elementLocated (locator)](#apidoc.element.protractor.until.elementLocated)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>elementTextContains (element, substr)](#apidoc.element.protractor.until.elementTextContains)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>elementTextIs (element, text)](#apidoc.element.protractor.until.elementTextIs)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>elementTextMatches (element, regex)](#apidoc.element.protractor.until.elementTextMatches)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>elementsLocated (locator)](#apidoc.element.protractor.until.elementsLocated)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>stalenessOf (element)](#apidoc.element.protractor.until.stalenessOf)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>titleContains (substr)](#apidoc.element.protractor.until.titleContains)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>titleIs (title)](#apidoc.element.protractor.until.titleIs)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>titleMatches (regex)](#apidoc.element.protractor.until.titleMatches)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>urlContains (substrUrl)](#apidoc.element.protractor.until.urlContains)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>urlIs (url)](#apidoc.element.protractor.until.urlIs)
1.  [function <span class="apidocSignatureSpan">protractor.until.</span>urlMatches (regex)](#apidoc.element.protractor.until.urlMatches)



# <a name="apidoc.module.protractor"></a>[module protractor](#apidoc.module.protractor)

#### <a name="apidoc.element.protractor.ActionSequence"></a>[function <span class="apidocSignatureSpan">protractor.</span>ActionSequence (driver)](#apidoc.element.protractor.ActionSequence)
- description and source-code
```javascript
class ActionSequence {
<span class="apidocCodeCommentSpan">  /**
   * @param {!./webdriver.WebDriver} driver The driver that should be used to
   *     perform this action sequence.
   */
</span>  constructor(driver) {
    /** @private {!./webdriver.WebDriver} */
    this.driver_ = driver;

    /** @private {!Array<{description: string, command: !command.Command}>} */
    this.actions_ = [];
  }

  /**
   * Schedules an action to be executed each time {@link #perform} is called on
   * this instance.
   *
   * @param {string} description A description of the command.
   * @param {!command.Command} command The command.
   * @private
   */
  schedule_(description, command) {
    this.actions_.push({
      description: description,
      command: command
    });
  }

  /**
   * Executes this action sequence.
   *
   * @return {!./promise.Thenable} A promise that will be resolved once
   *     this sequence has completed.
   */
  perform() {
    // Make a protected copy of the scheduled actions. This will protect against
    // users defining additional commands before this sequence is actually
    // executed.
    let actions = this.actions_.concat();
    let driver = this.driver_;
    return driver.controlFlow().execute(function() {
      let results = actions.map(action => {
        return driver.schedule(action.command, action.description);
      });
      return Promise.all(results);
    }, 'ActionSequence.perform');
  }

  /**
   * Moves the mouse.  The location to move to may be specified in terms of the
   * mouse's current location, an offset relative to the top-left corner of an
   * element, or an element (in which case the middle of the element is used).
   *
   * @param {(!./webdriver.WebElement|{x: number, y: number})} location The
   *     location to drag to, as either another WebElement or an offset in
   *     pixels.
   * @param {{x: number, y: number}=} opt_offset If the target {@code location}
   *     is defined as a {@link ./webdriver.WebElement}, this parameter defines
   *     an offset within that element. The offset should be specified in pixels
   *     relative to the top-left corner of the element's bounding box. If
   *     omitted, the element's center will be used as the target offset.
   * @return {!ActionSequence} A self reference.
   */
  mouseMove(location, opt_offset) {
    let cmd = new command.Command(command.Name.MOVE_TO);

    if (typeof location.x === 'number') {
      setOffset(/** @type {{x: number, y: number}} */(location));
    } else {
      cmd.setParameter('element', location.getId());
      if (opt_offset) {
        setOffset(opt_offset);
      }
    }

    this.schedule_('mouseMove', cmd);
    return this;

    /** @param {{x: number, y: number}} offset The offset to use. */
    function setOffset(offset) {
      cmd.setParameter('xoffset', offset.x || 0);
      cmd.setParameter('yoffset', offset.y || 0);
    }
  }

  /**
   * Schedules a mouse action.
   * @param {string} description A simple descriptive label for the scheduled
   *     action.
   * @param {!command.Name} commandName The name of the command.
   * @param {(./webdriver.WebElement|input.Button)=} opt_elementOrButton Either
   *     the element to interact with or the button to click with.
   *     Defaults to {@link input.Button.LEFT} if neither an element nor
   *     button is specified.
   * @param {input.Button=} opt_button The button to use. Defaults to
   *     {@link input.Button.LEFT}. Ignored if the previous argument is
   *     provided as a button.
   * @return {!ActionSequence} A self reference.
   * @private
   */
  scheduleMouseAction_(
      description, commandName, opt_elementOrButton, opt_button) {
    let button;
    if (typeof opt_elementOrButton === 'number') {
      button = opt_elementOrButton;
    } else {
      if (opt_elementOrButton) {
        this.mouseMove(
            /** @type {!./webdriver.WebElement} */ (opt_elementOrButton));
      }
      button = opt_button !== void(0) ? opt_button : input.Button.LEFT;
    }

    let cmd = new command.Command(commandName).
        setParameter('button', button);
    this.schedule_(d ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.Builder"></a>[function <span class="apidocSignatureSpan">protractor.</span>Builder ()](#apidoc.element.protractor.Builder)
- description and source-code
```javascript
class Builder {
  constructor() {
<span class="apidocCodeCommentSpan">    /** @private @const */
</span>    this.log_ = logging.getLogger('webdriver.Builder');

    /** @private {promise.ControlFlow} */
    this.flow_ = null;

    /** @private {string} */
    this.url_ = '';

    /** @private {?string} */
    this.proxy_ = null;

    /** @private {!Capabilities} */
    this.capabilities_ = new Capabilities();

    /** @private {chrome.Options} */
    this.chromeOptions_ = null;

    /** @private {firefox.Options} */
    this.firefoxOptions_ = null;

    /** @private {opera.Options} */
    this.operaOptions_ = null;

    /** @private {ie.Options} */
    this.ieOptions_ = null;

    /** @private {safari.Options} */
    this.safariOptions_ = null;

    /** @private {edge.Options} */
    this.edgeOptions_ = null;

    /** @private {boolean} */
    this.ignoreEnv_ = false;

    /** @private {http.Agent} */
    this.agent_ = null;
  }

  /**
   * Configures this builder to ignore any environment variable overrides and to
   * only use the configuration specified through this instance's API.
   *
   * @return {!Builder} A self reference.
   */
  disableEnvironmentOverrides() {
    this.ignoreEnv_ = true;
    return this;
  }

  /**
   * Sets the URL of a remote WebDriver server to use. Once a remote URL has
   * been specified, the builder direct all new clients to that server. If this
   * method is never called, the Builder will attempt to create all clients
   * locally.
   *
   * As an alternative to this method, you may also set the
   * 'SELENIUM_REMOTE_URL' environment variable.
   *
   * @param {string} url The URL of a remote server to use.
   * @return {!Builder} A self reference.
   */
  usingServer(url) {
    this.url_ = url;
    return this;
  }

  /**
   * @return {string} The URL of the WebDriver server this instance is
   *     configured to use.
   */
  getServerUrl() {
    return this.url_;
  }

  /**
   * Sets the URL of the proxy to use for the WebDriver's HTTP connections.
   * If this method is never called, the Builder will create a connection
   * without a proxy.
   *
   * @param {string} proxy The URL of a proxy to use.
   * @return {!Builder} A self reference.
   */
  usingWebDriverProxy(proxy) {
    this.proxy_ = proxy;
    return this;
  }

  /**
   * @return {?string} The URL of the proxy server to use for the WebDriver's
   *    HTTP connections, or 'null' if not set.
   */
  getWebDriverProxy() {
    return this.proxy_;
  }

  /**
   * Sets the http agent to use for each request.
   * If this method is not called, the Builder will use http.globalAgent by default.
   *
   * @param {http.Agent} agent The agent to use for each request.
   * @return {!Builder} A self reference.
   */
  usingHttpAgent(agent) {
    this.agent_ = agent;
    return this;
  }

  /**
   * @return {http.Agent} The http agent used for each request
   */
  getHttpAgent() {
    return this.agent_;
  }

  /**
   * Sets the desired capabilities when requesting a new session. This will
   * overwrite any previously set capabilities.
   * @param {!(Object|Capabilities)} capabilities The desired capabilities for
   *     a new session.
   * @return {!Builder} A self reference.
   */
  withCapabilities(capabilities) {
    this.capabilities_ = new Capabilities(capabilities);
    return this;
  }

  /**
   * Returns the base set of capabilities this instance is currently configured
   * to use.
   * @return {!Capabilities} The current capabilities for this builder.
   */
  getCapabilities() {
    return this.capabilities_;
  }

  /**
   * Configures the target browser for clients created by this instance.
   * Any calls to {@link #withCapabilities} after this function will
   * overwrite these settings.
   *
   * You may also define the target browser using the {@code SELENIUM_BROWSER}
   * environment variable. If set, this environment variable should be of the
   * form 'browser[:[version][:platform]]'.
   *
   * @param {(string|Browser)} name The name of the target browser;
   *     common defaults are available on the {@link webdriver.Browser} enum.
   * @param {string=} o ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.Capabilities"></a>[function <span class="apidocSignatureSpan">protractor.</span>Capabilities (Capabilities|Map<string, ?>|Object)](#apidoc.element.protractor.Capabilities)
- description and source-code
```javascript
class Capabilities extends Map {
<span class="apidocCodeCommentSpan">  /**
   * @param {(Capabilities|Map<string, ?>|Object)=} opt_other Another set of
   *     capabilities to initialize this instance from.
   */
</span>  constructor(opt_other) {
    if (opt_other && !(opt_other instanceof Map)) {
      opt_other = toMap(opt_other);
    }
    super(opt_other);
  }

  /**
   * @return {!Capabilities} A basic set of capabilities for Android.
   */
  static android() {
    return new Capabilities()
        .set(Capability.BROWSER_NAME, Browser.ANDROID)
        .set(Capability.PLATFORM, 'ANDROID');
  }

  /**
   * @return {!Capabilities} A basic set of capabilities for Chrome.
   */
  static chrome() {
    return new Capabilities().set(Capability.BROWSER_NAME, Browser.CHROME);
  }

  /**
   * @return {!Capabilities} A basic set of capabilities for Microsoft Edge.
   */
  static edge() {
    return new Capabilities()
        .set(Capability.BROWSER_NAME, Browser.EDGE)
        .set(Capability.PLATFORM, 'WINDOWS');
  }

  /**
   * @return {!Capabilities} A basic set of capabilities for Firefox.
   */
  static firefox() {
    return new Capabilities().set(Capability.BROWSER_NAME, Browser.FIREFOX);
  }

  /**
   * @return {!Capabilities} A basic set of capabilities for Internet Explorer.
   */
  static ie() {
    return new Capabilities().
        set(Capability.BROWSER_NAME, Browser.INTERNET_EXPLORER).
        set(Capability.PLATFORM, 'WINDOWS');
  }

  /**
   * @return {!Capabilities} A basic set of capabilities for iPad.
   */
  static ipad() {
    return new Capabilities().
        set(Capability.BROWSER_NAME, Browser.IPAD).
        set(Capability.PLATFORM, 'MAC');
  }

  /**
   * @return {!Capabilities} A basic set of capabilities for iPhone.
   */
  static iphone() {
    return new Capabilities().
        set(Capability.BROWSER_NAME, Browser.IPHONE).
        set(Capability.PLATFORM, 'MAC');
  }

  /**
   * @return {!Capabilities} A basic set of capabilities for Opera.
   */
  static opera() {
    return new Capabilities().
        set(Capability.BROWSER_NAME, Browser.OPERA);
  }

  /**
   * @return {!Capabilities} A basic set of capabilities for PhantomJS.
   */
  static phantomjs() {
    return new Capabilities().
        set(Capability.BROWSER_NAME, Browser.PHANTOM_JS);
  }

  /**
   * @return {!Capabilities} A basic set of capabilities for Safari.
   */
  static safari() {
    return new Capabilities().
        set(Capability.BROWSER_NAME, Browser.SAFARI).
        set(Capability.PLATFORM, 'MAC');
  }

  /**
   * @return {!Capabilities} A basic set of capabilities for HTMLUnit.
   */
  static htmlunit() {
    return new Capabilities().
        set(Capability.BROWSER_NAME, Browser.HTMLUNIT);
  }

  /**
   * @return {!Capabilities} A basic set of capabilities for HTMLUnit
   *     with enabled Javascript.
   */
  static htmlunitwithjs() {
    return new Capabilities().
        set(Capability.BROWSER_NAME, Browser.HTMLUNIT).
        set(Capability.SUPPORTS_JAVASCRIPT, true);
  }

  /**
   * @return {!Object<string, ?>} The JSON representation of this instance.
   *     Note, the returned object may contain nested promised values.
   * @suppress {checkTypes} Suppress [] access on a struct (state inherited from
   *     Map).
   */
  [Symbols.serialize]() {
    return serialize(this);
  }

  /**
   * Merges another set of capabilities into this instance.
   * @param {!(Capabilities|Map<String, ?>|Object<string, ?>)} other The other
   *     set of capabilities to merge.
   * @return {!Capabilities} A self reference.
   */
  merge(other) {
    if (!other) {
      throw new TypeError('no capabilities provided for merge');
    }

    if (!(other instanceof Map)) {
      other = toMap(other);
    }

    for (let key of other.keys()) {
      this.set(key, other.get(key));
    }

    return this;
  }

  /**
   * @param {string} key The capability key.
   * @param {*} value The capability value.
   * @return {!Capabilities} A self reference.
   * @throws {TypeError} If the 'key' is not a string.
   * @override
   */
  set(key, value) {
    if (typeof key !== 'string') { ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.Command"></a>[function <span class="apidocSignatureSpan">protractor.</span>Command (name)](#apidoc.element.protractor.Command)
- description and source-code
```javascript
class Command {
<span class="apidocCodeCommentSpan">  /** @param {string} name The name of this command. */
</span>  constructor(name) {
    /** @private {string} */
    this.name_ = name;

    /** @private {!Object<*>} */
    this.parameters_ = {};
  }

  /** @return {string} This command's name. */
  getName() {
    return this.name_;
  }

  /**
   * Sets a parameter to send with this command.
   * @param {string} name The parameter name.
   * @param {*} value The parameter value.
   * @return {!Command} A self reference.
   */
  setParameter(name, value) {
    this.parameters_[name] = value;
    return this;
  }

  /**
   * Sets the parameters for this command.
   * @param {!Object<*>} parameters The command parameters.
   * @return {!Command} A self reference.
   */
  setParameters(parameters) {
    this.parameters_ = parameters;
    return this;
  }

  /**
   * Returns a named command parameter.
   * @param {string} key The parameter key to look up.
   * @return {*} The parameter value, or undefined if it has not been set.
   */
  getParameter(key) {
    return this.parameters_[key];
  }

  /**
   * @return {!Object<*>} The parameters to send with this command.
   */
  getParameters() {
    return this.parameters_;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.ElementArrayFinder"></a>[function <span class="apidocSignatureSpan">protractor.</span>ElementArrayFinder (browser_, getWebElements = null, locator_, actionResults_ = null)](#apidoc.element.protractor.ElementArrayFinder)
- description and source-code
```javascript
class ElementArrayFinder extends WebdriverWebElement {
    constructor(browser_, getWebElements = null, locator_, actionResults_ = null) {
        super();
        this.browser_ = browser_;
        this.getWebElements = getWebElements;
        this.locator_ = locator_;
        this.actionResults_ = actionResults_;
        // TODO(juliemr): might it be easier to combine this with our docs and just
        // wrap each one explicity with its own documentation?
        WEB_ELEMENT_FUNCTIONS.forEach((fnName) => {
            this[fnName] = (...args) => {
                let actionFn = (webElem) => {
                    return webElem[fnName].apply(webElem, args);
                };
                return this.applyAction_(actionFn);
            };
        });
    }
<span class="apidocCodeCommentSpan">    /**
     * Create a shallow copy of ElementArrayFinder.
     *
     * @returns {!ElementArrayFinder} A shallow copy of this.
     */
</span>    clone() {
        // A shallow copy is all we need since the underlying fields can never be
        // modified. (Locator can be modified by the user, but that should
        // rarely/never happen and it doesn't affect functionalities).
        return new ElementArrayFinder(this.browser_, this.getWebElements, this.locator_, this.actionResults_);
    }
    /**
     * Calls to ElementArrayFinder may be chained to find an array of elements
     * using the current elements in this ElementArrayFinder as the starting
     * point. This function returns a new ElementArrayFinder which would contain
     * the children elements found (and could also be empty).
     *
     * @alias element.all(locator).all(locator)
     * @view
     * <div id='id1' class="parent">
     *   <ul>
     *     <li class="foo">1a</li>
     *     <li class="baz">1b</li>
     *   </ul>
     * </div>
     * <div id='id2' class="parent">
     *   <ul>
     *     <li class="foo">2a</li>
     *     <li class="bar">2b</li>
     *   </ul>
     * </div>
     *
     * @example
     * let foo = element.all(by.css('.parent')).all(by.css('.foo'));
     * expect(foo.getText()).toEqual(['1a', '2a']);
     * let baz = element.all(by.css('.parent')).all(by.css('.baz'));
     * expect(baz.getText()).toEqual(['1b']);
     * let nonexistent = element.all(by.css('.parent'))
     *   .all(by.css('.NONEXISTENT'));
     * expect(nonexistent.getText()).toEqual(['']);
     *
     * // Or using the shortcut $$() notation instead of element.all(by.css()):
     *
     * let foo = $$('.parent').$$('.foo');
     * expect(foo.getText()).toEqual(['1a', '2a']);
     * let baz = $$('.parent').$$('.baz');
     * expect(baz.getText()).toEqual(['1b']);
     * let nonexistent = $$('.parent').$$('.NONEXISTENT');
     * expect(nonexistent.getText()).toEqual(['']);
     *
     * @param {webdriver.Locator} subLocator
     * @returns {ElementArrayFinder}
     */
    all(locator) {
        let ptor = this.browser_;
        let getWebElements = () => {
            if (this.getWebElements === null) {
                // This is the first time we are looking for an element
                return ptor.waitForAngular('Locator: ' + locator)
                    .then(() => {
                    if (locators_1.isProtractorLocator(locator)) {
                        return locator.findElementsOverride(ptor.driver, null, ptor.rootEl);
                    }
                    else {
                        return ptor.driver.findElements(locator);
                    }
                });
            }
            else {
                return this.getWebElements().then((parentWebElements) => {
                    // For each parent web element, find their children and construct
                    // a list of Promise<List<child_web_element>>
                    let childrenPromiseList = parentWebElements.map((parentWebElement) => {
                        return locators_1.isProtractorLocator(locator) ?
                            locator.findElementsOverride(ptor.driver, parentWebElement, ptor.rootEl) :
                            parentWebElement.findElements(locator);
                    }); ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.ElementFinder"></a>[function <span class="apidocSignatureSpan">protractor.</span>ElementFinder (browser_, elementArrayFinder)](#apidoc.element.protractor.ElementFinder)
- description and source-code
```javascript
class ElementFinder extends WebdriverWebElement {
    constructor(browser_, elementArrayFinder) {
        super();
        this.browser_ = browser_;
        this.then = null;
        if (!elementArrayFinder) {
            throw new Error('BUG: elementArrayFinder cannot be empty');
        }
        this.parentElementArrayFinder = elementArrayFinder;
        // Only have a 'then' method if the parent element array finder
        // has action results.
        if (this.parentElementArrayFinder.actionResults_) {
            // Access the underlying actionResult of ElementFinder.
            this.then =
                    (fn, errorFn) => {
                    return this.elementArrayFinder_.then((actionResults) => {
                        if (!fn) {
                            return actionResults[0];
                        }
                        return fn(actionResults[0]);
                    }, errorFn);
                };
        }
        // This filter verifies that there is only 1 element returned by the
        // elementArrayFinder. It will warn if there are more than 1 element and
        // throw an error if there are no elements.
        let getWebElements = () => {
            return elementArrayFinder.getWebElements().then((webElements) => {
                if (webElements.length === 0) {
                    throw new selenium_webdriver_1.error.NoSuchElementError('No element found using locator: ' + elementArrayFinder
.locator().toString());
                }
                else {
                    if (webElements.length > 1) {
                        logger.warn('more than one element found for locator ' +
                            elementArrayFinder.locator().toString() + ' - the first result will be used');
                    }
                    return [webElements[0]];
                }
            });
        };
        // Store a copy of the underlying elementArrayFinder, but with the more
        // restrictive getWebElements (which checks that there is only 1 element).
        this.elementArrayFinder_ = new ElementArrayFinder(this.browser_, getWebElements, elementArrayFinder.locator(), elementArrayFinder
.actionResults_);
        WEB_ELEMENT_FUNCTIONS.forEach((fnName) => {
            (this)[fnName] = (...args) => {
                return (this.elementArrayFinder_)[fnName]
                    .apply(this.elementArrayFinder_, args)
                    .toElementFinder_();
            };
        });
    }
    static fromWebElement_(browser, webElem, locator) {
        let getWebElements = () => {
            return selenium_webdriver_1.promise.when([webElem]);
        };
        return new ElementArrayFinder(browser, getWebElements, locator).toElementFinder_();
    }
<span class="apidocCodeCommentSpan">    /**
     * Create a shallow copy of ElementFinder.
     *
     * @returns {!ElementFinder} A shallow copy of this.
     */
</span>    clone() {
        // A shallow copy is all we need since the underlying fields can never be
        // modified
        return new ElementFinder(this.browser_, this.parentElementArrayFinder);
    }
    /**
     * @see ElementArrayFinder.prototype.locator
     *
     * @returns {webdriver.Locator}
     */
    locator() {
        return this.elementArrayFinder_.locator();
    }
    /**
     * Returns the WebElement represented by this ElementFinder.
     * Throws the WebDriver error if the element doesn't exist.
     *
     * @alias element(locator).getWebElement()
     * @view
     * <div class="parent">
     *   some text
     * </div>
     *
     * @example
     * // The following four expressions are equivalent.
     * $('.parent').getWebElement();
     * element(by.css('.parent')).getWebElement();
     * browser.driver.findElement(by.css('.parent'));
     * browser.findElement(by.css('.parent'));
     *
     * @returns {webdriver.WebElementPromise}
     */
    getWebElement() {
        let id = this.elementArrayFinder_.getWebElements().then((parentWebElements) => {
            return parentWebElements[0];
        });
        return new selenium_webdriver_1.WebElementPromise(this.browser_.driver, ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.EventEmitter"></a>[function <span class="apidocSignatureSpan">protractor.</span>EventEmitter (type, var_args)](#apidoc.element.protractor.EventEmitter)
- description and source-code
```javascript
class EventEmitter {
<span class="apidocCodeCommentSpan">  /**
   * Fires an event and calls all listeners.
   * @param {string} type The type of event to emit.
   * @param {...*} var_args Any arguments to pass to each listener.
   */
</span>  emit(type, var_args) {
    let events = EVENTS.get(this);
    if (!events) {
      return;
    }

    let args = Array.prototype.slice.call(arguments, 1);

    let listeners = events.get(type);
    if (listeners) {
      for (let listener of listeners) {
        listener.fn.apply(listener.scope, args);
        if (listener.oneshot) {
          listeners.delete(listener);
        }
      }
    }
  }

  /**
   * Returns a mutable list of listeners for a specific type of event.
   * @param {string} type The type of event to retrieve the listeners for.
   * @return {!Set<!Listener>} The registered listeners for the given event
   *     type.
   */
  listeners(type) {
    let events = EVENTS.get(this);
    if (!events) {
      events = new Map;
      EVENTS.set(this, events);
    }

    let listeners = events.get(type);
    if (!listeners) {
      listeners = new Set;
      events.set(type, listeners);
    }
    return listeners;
  }

  /**
   * Registers a listener.
   * @param {string} type The type of event to listen for.
   * @param {!Function} fn The function to invoke when the event is fired.
   * @param {Object=} opt_self The object in whose scope to invoke the listener.
   * @param {boolean=} opt_oneshot Whether the listener should b (e removed after
   *    the first event is fired.
   * @return {!EventEmitter} A self reference.
   * @private
   */
  addListener_(type, fn, opt_self, opt_oneshot) {
    let listeners = this.listeners(type);
    for (let listener of listeners) {
      if (listener.fn === fn) {
        return this;
      }
    }
    listeners.add(new Listener(fn, opt_self || undefined, !!opt_oneshot));
    return this;
  }

  /**
   * Registers a listener.
   * @param {string} type The type of event to listen for.
   * @param {!Function} fn The function to invoke when the event is fired.
   * @param {Object=} opt_self The object in whose scope to invoke the listener.
   * @return {!EventEmitter} A self reference.
   */
  addListener(type, fn, opt_self) {
    return this.addListener_(type, fn, opt_self, false);
  }

  /**
   * Registers a one-time listener which will be called only the first time an
   * event is emitted, after which it will be removed.
   * @param {string} type The type of event to listen for.
   * @param {!Function} fn The function to invoke when the event is fired.
   * @param {Object=} opt_self The object in whose scope to invoke the listener.
   * @return {!EventEmitter} A self reference.
   */
  once(type, fn, opt_self) {
    return this.addListener_(type, fn, opt_self, true);
  }

  /**
   * An alias for {@link #addListener() addListener()}.
   * @param {string} type The type of event to listen for.
   * @param {!Function} fn The function to invoke when the event is fired.
   * @param {Object=} opt_self The object in whose scope to invoke the listener.
   * @return {!EventEmitter} A self reference.
   */
  on(type, fn, opt_self) {
    return this.addListener(type, fn, opt_self);
  }

  /**
   * Removes a previously registered event listener.
   * @param {string} type The type of event to unregister.
   * @param {!Function} listenerFn The handler function to remove.
   * @return {!EventEmitter} A self reference.
   */
  removeListener(type, listenerFn) {
    if (typeof type !== 'string' || typeof listenerFn !== 'function') {
      throw TypeError('invalid args: expected (string, function), got ('
          + (typeof type) + ', ' + (typeof listenerFn) + ')');
    }

    let events = EVENTS.get(this);
    if (!events) {
      return this;
    }

    let listeners = events.get(type);
    if (!listeners) {
      return this;
    }

    let match;
    for (let listener of listeners) {
      if (listener.fn === listenerFn) {
        match = listener;
        break;
      }
    }
    if (match) {
      listeners.delete(match);
      if (!listeners.size) {
        events.delete(type);
      } ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.FileDetector"></a>[function <span class="apidocSignatureSpan">protractor.</span>FileDetector (driver, path)](#apidoc.element.protractor.FileDetector)
- description and source-code
```javascript
class FileDetector {

<span class="apidocCodeCommentSpan">  /**
   * Handles the file specified by the given path, preparing it for use with
   * the current browser. If the path does not refer to a valid file, it will
   * be returned unchanged, otherwisee a path suitable for use with the current
   * browser will be returned.
   *
   * This default implementation is a no-op. Subtypes may override this function
   * for custom tailored file handling.
   *
   * @param {!./webdriver.WebDriver} driver The driver for the current browser.
   * @param {string} path The path to process.
   * @return {!Promise<string>} A promise for the processed file path.
   * @package
   */
</span>  handleFile(driver, path) {
    return Promise.resolve(path);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.ProtractorBrowser"></a>[function <span class="apidocSignatureSpan">protractor.</span>ProtractorBrowser (webdriverInstance, opt_baseUrl, opt_rootElement, opt_untrackOutstandingTimeouts, opt_blockingProxyUrl)](#apidoc.element.protractor.ProtractorBrowser)
- description and source-code
```javascript
class ProtractorBrowser extends AbstractExtendedWebDriver {
    constructor(webdriverInstance, opt_baseUrl, opt_rootElement, opt_untrackOutstandingTimeouts, opt_blockingProxyUrl) {
        super();
        // These functions should delegate to the webdriver instance, but should
        // wait for Angular to sync up before performing the action. This does not
        // include functions which are overridden by protractor below.
        let methodsToSync = ['getCurrentUrl', 'getPageSource', 'getTitle'];
        let extendWDInstance;
        try {
            extendWDInstance = webdriver_js_extender_1.extend(webdriverInstance);
        }
        catch (e) {
            // Probably not a driver that can be extended (e.g. gotten using
            // 'directConnect: true' in the config)
            extendWDInstance = webdriverInstance;
        }
        // Mix all other driver functionality into Protractor.
        Object.getOwnPropertyNames(selenium_webdriver_1.WebDriver.prototype).forEach(method => {
            if (!this[method] && typeof extendWDInstance[method] === 'function') {
                if (methodsToSync.indexOf(method) !== -1) {
                    ptorMixin(this, extendWDInstance, method, this.waitForAngular.bind(this));
                }
                else {
                    ptorMixin(this, extendWDInstance, method);
                }
            }
        });
        this.driver = extendWDInstance;
        if (opt_blockingProxyUrl) {
            logger.info('Starting BP client for ' + opt_blockingProxyUrl);
            this.bpClient = new blocking_proxy_1.BPClient(opt_blockingProxyUrl);
        }
        this.element = buildElementHelper(this);
        this.$ = element_1.build$(this.element, selenium_webdriver_1.By);
        this.$$ = element_1.build$$(this.element, selenium_webdriver_1.By);
        this.baseUrl = opt_baseUrl || '';
        this.getPageTimeout = DEFAULT_GET_PAGE_TIMEOUT;
        this.params = {};
        this.resetUrl = DEFAULT_RESET_URL;
        this.debugHelper = new debugger_1.DebugHelper(this);
        let ng12Hybrid_ = false;
        Object.defineProperty(this, 'ng12Hybrid', {
            get: function () {
                return ng12Hybrid_;
            },
            set: function (ng12Hybrid) {
                if (ng12Hybrid) {
                    logger.warn('You have set ng12Hybrid.  As of Protractor 4.1.0, ' +
                        'Protractor can automatically infer if you are using an ' +
                        'ngUpgrade app (as long as ng1 is loaded before you call ' +
                        'platformBrowserDynamic()), and this flag is no longer needed ' +
                        'for most users');
                }
                ng12Hybrid_ = ng12Hybrid;
            }
        });
        this.ready = this.angularAppRoot(opt_rootElement || '')
            .then(() => {
            return this.driver.getSession();
        })
            .then((session) => {
            // Internet Explorer does not accept data URLs, which are the default
            // reset URL for Protractor.
            // Safari accepts data urls, but SafariDriver fails after one is used.
            // PhantomJS produces a "Detected a page unload event" if we use data urls
            let browserName = session.getCapabilities().get('browserName');
            if (browserName === 'internet explorer' || browserName === 'safari' ||
                browserName === 'phantomjs' || browserName === 'MicrosoftEdge') {
                this.resetUrl = 'about:blank';
            }
            return this;
        });
        this.trackOutstandingTimeouts_ = !opt_untrackOutstandingTimeouts;
        this.mockModules_ = [];
        this.addBaseMockModules_();
        // set up expected conditions
        this.ExpectedConditions = new expectedConditions_1.ProtractorExpectedConditions(this);
    }
    /**
     * The css selector for an element on which to find Angular. This is usually
     * 'body' but if your ng-app is on a subsection of the page it may be
     * a subelement.
     *
     * This property is dep ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.ProtractorBy"></a>[function <span class="apidocSignatureSpan">protractor.</span>ProtractorBy (by.locatorName(args)](#apidoc.element.protractor.ProtractorBy)
- description and source-code
```javascript
class ProtractorBy extends WebdriverBy {
<span class="apidocCodeCommentSpan">    /**
     * Add a locator to this instance of ProtractorBy. This locator can then be
     * used with element(by.locatorName(args)).
     *
     * @view
     * <button ng-click="doAddition()">Go!</button>
     *
     * @example
     * // Add the custom locator.
     * by.addLocator('buttonTextSimple',
     *     function(buttonText, opt_parentElement, opt_rootSelector) {
     *   // This function will be serialized as a string and will execute in the
     *   // browser. The first argument is the text for the button. The second
     *   // argument is the parent element, if any.
     *   var using = opt_parentElement || document,
     *       buttons = using.querySelectorAll('button');
     *
     *   // Return an array of buttons with the text.
     *   return Array.prototype.filter.call(buttons, function(button) {
     *     return button.textContent === buttonText;
     *   });
     * });
     *
     * // Use the custom locator.
     * element(by.buttonTextSimple('Go!')).click();
     *
     * @alias by.addLocator(locatorName, functionOrScript)
     * @param {string} name The name of the new locator.
     * @param {Function|string} script A script to be run in the context of
     *     the browser. This script will be passed an array of arguments
     *     that contains any args passed into the locator followed by the
     *     element scoping the search and the css selector for the root angular
     *     element. It should return an array of elements.
     */
</span>    addLocator(name, script) {
        this[name] = (...args) => {
            let locatorArguments = args;
            return {
                findElementsOverride: (driver, using, rootSelector) => {
                    let findElementArguments = [script];
                    for (let i = 0; i < locatorArguments.length; i++) {
                        findElementArguments.push(locatorArguments[i]);
                    }
                    findElementArguments.push(using);
                    findElementArguments.push(rootSelector);
                    return driver.findElements(selenium_webdriver_1.By.js.apply(selenium_webdriver_1.By, findElementArguments));
                },
                toString: () => {
                    return 'by.' + name + '("' + Array.prototype.join.call(locatorArguments, '", "') + '")';
                }
            };
        };
    }
    ;
    /**
     * Find an element by text binding. Does a partial match, so any elements
     * bound to variables containing the input string will be returned.
     *
     * Note: For AngularJS version 1.2, the interpolation brackets, (usually
     * {{}}), are optionally allowed in the binding description string. For
     * Angular version 1.3+, they are not allowed, and no elements will be found
     * if they are used.
     *
     * @view
     * <span>{{person.name}}</span>
     * <span ng-bind="person.email"></span>
     *
     * @example
     * var span1 = element(by.binding('person.name'));
     * expect(span1.getText()).toBe('Foo');
     *
     * var span2 = element(by.binding('person.email'));
     * expect(span2.getText()).toBe('foo@bar.com');
     *
     * // You can also use a substring for a partial match
     * var span1alt = element(by.binding('name'));
     * expect(span1alt.getText()).toBe('Foo');
     *
     * // This works for sites using Angular 1.2 but NOT 1.3
     * var deprecatedSyntax = element(by.binding('{{person.name}}'));
     *
     * @param {string} bindingDescriptor
     * @returns {ProtractorLocator} location strategy
     */
    binding(bindingDescriptor) {
        return {
            findElementsOverride: (driver, using, rootSelector) => {
                return driver.findElements(selenium_webdriver_1.By.js(clientSideScripts.findBindings, bindingDescriptor, false,
using, rootSelector));
            },
            toString: () => {
                return 'by.binding("' + bindingDescriptor + '")';
            }
        };
    }
    ;
    /**
     * Find an element by exact binding.
     *
     * @view
     * <span> ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.ProtractorExpectedConditions"></a>[function <span class="apidocSignatureSpan">protractor.</span>ProtractorExpectedConditions (browser)](#apidoc.element.protractor.ProtractorExpectedConditions)
- description and source-code
```javascript
class ProtractorExpectedConditions {
    constructor(browser) {
        this.browser = browser;
    }
    ;
<span class="apidocCodeCommentSpan">    /**
     * Negates the result of a promise.
     *
     * @example
     * var EC = protractor.ExpectedConditions;
     * var titleIsNotFoo = EC.not(EC.titleIs('Foo'));
     * // Waits for title to become something besides 'foo'.
     * browser.wait(titleIsNotFoo, 5000);
     *
     * @alias ExpectedConditions.not
     * @param {!function} expectedCondition
     *
     * @returns {!function} An expected condition that returns the negated value.
     */
</span>    not(expectedCondition) {
        return () => {
            return expectedCondition().then((bool) => {
                return !bool;
            });
        };
    }
    /**
     * Helper function that is equivalent to the logical_and if defaultRet==true,
     * or logical_or if defaultRet==false
     *
     * @private
     * @param {boolean} defaultRet
     * @param {Array.<Function>} fns An array of expected conditions to chain.
     *
     * @returns {!function} An expected condition that returns a promise which
     *     evaluates to the result of the logical chain.
     */
    logicalChain_(defaultRet, fns) {
        let self = this;
        return () => {
            if (fns.length === 0) {
                return defaultRet;
            }
            let fn = fns[0];
            return fn().then((bool) => {
                if (bool === defaultRet) {
                    return self.logicalChain_(defaultRet, fns.slice(1))();
                }
                else {
                    return !defaultRet;
                }
            });
        };
    }
    /**
     * Chain a number of expected conditions using logical_and, short circuiting
     * at the first expected condition that evaluates to false.
     *
     * @example
     * var EC = protractor.ExpectedConditions;
     * var titleContainsFoo = EC.titleContains('Foo');
     * var titleIsNotFooBar = EC.not(EC.titleIs('FooBar'));
     * // Waits for title to contain 'Foo', but is not 'FooBar'
     * browser.wait(EC.and(titleContainsFoo, titleIsNotFooBar), 5000);
     *
     * @alias ExpectedConditions.and
     * @param {Array.<Function>} fns An array of expected conditions to 'and'
     * together.
     *
     * @returns {!function} An expected condition that returns a promise which
     *     evaluates to the result of the logical and.
     */
    and(...args) {
        return this.logicalChain_(true, args);
    }
    /**
     * Chain a number of expected conditions using logical_or, short circuiting
     * at the first expected condition that evaluates to true.
     *
     * @alias ExpectedConditions.or
     * @example
     * var EC = protractor.ExpectedConditions;
     * var titleContainsFoo = EC.titleContains('Foo');
     * var titleContainsBar = EC.titleContains('Bar');
     * // Waits for title to contain either 'Foo' or 'Bar'
     * browser.wait(EC.or(titleContainsFoo, titleContainsBar), 5000);
     *
     * @param {Array.<Function>} fns An array of expected conditions to 'or'
     * together.
     *
     * @returns {!function} An expected condition that returns a promise which
     *     evaluates to the result of the logical or.
     */
    or(...args) {
        return this.logicalChain_(false, args);
    }
    /**
     * Expect an alert to be present.
     *
     * @example
     * var EC = protractor.ExpectedConditions;
     * // Waits for an alert pops up.
     * browser.wait(EC.alertIsPresent(), 5000);
     *
     * @alias ExpectedConditions.alertIsPresent
     * @returns {!function} An expected condition that returns a promise
     *     representing whether an alert is present.
     */
    alertIsPresent() {
        return () => {
            return this.browser.driver.switchTo().alert().then(() => {
                return true;
            }, (err) => {
                if (err instanceof selenium_webdriver_1.error.NoSuchAlertError) {
                    return false;
                }
                else {
                    throw err;
                }
            });
        }; ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.Ptor"></a>[function <span class="apidocSignatureSpan">protractor.</span>Ptor ()](#apidoc.element.protractor.Ptor)
- description and source-code
```javascript
class Ptor {
    constructor() {
        this.$ = function (search) {
            return null;
        };
        this.$$ = function (search) {
            return null;
        };
        // Export protractor classes.
        this.ProtractorBrowser = require('./browser').ProtractorBrowser;
        this.ElementFinder = require('./element').ElementFinder;
        this.ElementArrayFinder = require('./element').ElementArrayFinder;
        this.ProtractorBy = require('./locators').ProtractorBy;
        this.ProtractorExpectedConditions = require('./expectedConditions').ProtractorExpectedConditions;
        // Export selenium webdriver.
        this.ActionSequence = webdriver.ActionSequence;
        this.Browser = webdriver.Browser;
        this.Builder = webdriver.Builder;
        this.Button = webdriver.Button;
        this.Capabilities = webdriver.Capabilities;
        this.Capability = webdriver.Capability;
        this.EventEmitter = webdriver.EventEmitter;
        this.FileDetector = webdriver.FileDetector;
        this.Key = webdriver.Key;
        this.Session = webdriver.Session;
        this.WebDriver = webdriver.WebDriver;
        this.WebElement = webdriver.WebElement;
        this.WebElementPromise = webdriver.WebElementPromise;
        this.error = webdriver.error;
        this.logging = webdriver.logging;
        this.promise = webdriver.promise;
        this.until = webdriver.until;
        this.Command = require('selenium-webdriver/lib/command').Command;
        this.CommandName = require('selenium-webdriver/lib/command').Name;
        this.utils = { firefox: firefox, http: http, remote: remote, chrome: chrome };
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.Session"></a>[function <span class="apidocSignatureSpan">protractor.</span>Session (Object|Capabilities)](#apidoc.element.protractor.Session)
- description and source-code
```javascript
class Session {

<span class="apidocCodeCommentSpan">  /**
   * @param {string} id The session ID.
   * @param {!(Object|Capabilities)} capabilities The session
   *     capabilities.
   */
</span>  constructor(id, capabilities) {
    /** @private {string} */
    this.id_ = id;

    /** @private {!Capabilities} */
    this.caps_ = capabilities instanceof Capabilities
        ? /** @type {!Capabilities} */(capabilities)
        : new Capabilities(capabilities);
  }

  /**
   * @return {string} This session's ID.
   */
  getId() {
    return this.id_;
  }

  /**
   * @return {!Capabilities} This session's capabilities.
   */
  getCapabilities() {
    return this.caps_;
  }

  /**
   * Retrieves the value of a specific capability.
   * @param {string} key The capability to retrieve.
   * @return {*} The capability value.
   */
  getCapability(key) {
    return this.caps_.get(key);
  }

  /**
   * Returns the JSON representation of this object, which is just the string
   * session ID.
   * @return {string} The JSON representation of this Session.
   */
  toJSON() {
    return this.getId();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.WebDriver"></a>[function <span class="apidocSignatureSpan">protractor.</span>WebDriver (Session|IThenable<!Session>)](#apidoc.element.protractor.WebDriver)
- description and source-code
```javascript
class WebDriver {
<span class="apidocCodeCommentSpan">  /**
   * @param {!(Session|IThenable<!Session>)} session Either a known session or a
   *     promise that will be resolved to a session.
   * @param {!command.Executor} executor The executor to use when sending
   *     commands to the browser.
   * @param {promise.ControlFlow=} opt_flow The flow to
   *     schedule commands through. Defaults to the active flow object.
   * @param {(function(this: void): ?)=} opt_onQuit A function to call, if any,
   *     when the session is terminated.
   */
</span>  constructor(session, executor, opt_flow, opt_onQuit) {
    /** @private {!promise.ControlFlow} */
    this.flow_ = opt_flow || promise.controlFlow();

    /** @private {!promise.Thenable<!Session>} */
    this.session_ = this.flow_.promise(resolve => resolve(session));

    /** @private {!command.Executor} */
    this.executor_ = executor;

    /** @private {input.FileDetector} */
    this.fileDetector_ = null;

    /** @private @const {(function(this: void): ?|undefined)} */
    this.onQuit_ = opt_onQuit;
  }

  /**
   * Creates a new WebDriver client for an existing session.
   * @param {!command.Executor} executor Command executor to use when querying
   *     for session details.
   * @param {string} sessionId ID of the session to attach to.
   * @param {promise.ControlFlow=} opt_flow The control flow all
   *     driver commands should execute under. Defaults to the
   *     {@link promise.controlFlow() currently active}  control flow.
   * @return {!WebDriver} A new client for the specified session.
   */
  static attachToSession(executor, sessionId, opt_flow) {
    let flow = opt_flow || promise.controlFlow();
    let cmd = new command.Command(command.Name.DESCRIBE_SESSION)
        .setParameter('sessionId', sessionId);
    let session = flow.execute(
        () => executeCommand(executor, cmd).catch(err => {
          // The DESCRIBE_SESSION command is not supported by the W3C spec, so
          // if we get back an unknown command, just return a session with
          // unknown capabilities.
          if (err instanceof error.UnknownCommandError) {
            return new Session(sessionId, new Capabilities);
          }
          throw err;
        }),
        'WebDriver.attachToSession()');
    return new WebDriver(session, executor, flow);
  }

  /**
   * Creates a new WebDriver session.
   *
   * By default, the requested session 'capabilities' are merely "desired" and
   * the remote end will still create a new session even if it cannot satisfy
   * all of the requested capabilities. You can query which capabilities a
   * session actually has using the
   * {@linkplain #getCapabilities() getCapabilities()} method on the returned
   * WebDriver instance.
   *
   * To define _required capabilities_, provide the 'capabilities' as an object
   * literal with 'required' and 'desired' keys. The 'desired' key may be
   * omitted if all capabilities are required, and vice versa. If the server
   * cannot create a session with all of the required capabilities, it will
   * return an {@linkplain error.SessionNotCreatedError}.
   *
   *     let required = new Capabilities().set('browserName', 'firefox');
   *     let desired = new Capabilities().set('version', '45');
   *     let driver = WebDriver.createSession(executor, {required, desired});
   *
   * This function will always return a WebDriver instance. If there is an error
   * creating the session, such as the aforementioned SessionNotCreatedError,
   * the driver will have a rejected {@linkplain #getSession session} promise.
   * It is recommended that this promise is left _unhandled_ so it will
   * propagate through the {@linkplain promise.ControlFlow control flow} and
   * cause subsequent commands to fail.
   *
   *     let required = Capabilities.firefox();
   *     let driver = WebDriver.createSession(executor, {required});
   *
   *     // If the createSession operation failed, then this command will also
   *     // also fail, propagating the creation failure.
   *     driver.get('http://www.google.com').catch(e => console.log(e));
   * ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.WebElement"></a>[function <span class="apidocSignatureSpan">protractor.</span>WebElement (!IThenable<string>|string)](#apidoc.element.protractor.WebElement)
- description and source-code
```javascript
class WebElement {
<span class="apidocCodeCommentSpan">  /**
   * @param {!WebDriver} driver the parent WebDriver instance for this element.
   * @param {(!IThenable<string>|string)} id The server-assigned opaque ID for
   *     the underlying DOM element.
   */
</span>  constructor(driver, id) {
    /** @private {!WebDriver} */
    this.driver_ = driver;

    /** @private {!promise.Thenable<string>} */
    this.id_ = driver.controlFlow().promise(resolve => resolve(id));
  }

  /**
   * @param {string} id The raw ID.
   * @param {boolean=} opt_noLegacy Whether to exclude the legacy element key.
   * @return {!Object} The element ID for use with WebDriver's wire protocol.
   */
  static buildId(id, opt_noLegacy) {
    return opt_noLegacy
        ? {[ELEMENT_ID_KEY]: id}
        : {[ELEMENT_ID_KEY]: id, [LEGACY_ELEMENT_ID_KEY]: id};
  }

  /**
   * Extracts the encoded WebElement ID from the object.
   *
   * @param {?} obj The object to extract the ID from.
   * @return {string} the extracted ID.
   * @throws {TypeError} if the object is not a valid encoded ID.
   */
  static extractId(obj) {
    if (obj && typeof obj === 'object') {
      if (typeof obj[ELEMENT_ID_KEY] === 'string') {
        return obj[ELEMENT_ID_KEY];
      } else if (typeof obj[LEGACY_ELEMENT_ID_KEY] === 'string') {
        return obj[LEGACY_ELEMENT_ID_KEY];
      }
    }
    throw new TypeError('object is not a WebElement ID');
  }

  /**
   * @param {?} obj the object to test.
   * @return {boolean} whether the object is a valid encoded WebElement ID.
   */
  static isId(obj) {
    return obj && typeof obj === 'object'
        && (typeof obj[ELEMENT_ID_KEY] === 'string'
            || typeof obj[LEGACY_ELEMENT_ID_KEY] === 'string');
  }

  /**
   * Compares two WebElements for equality.
   *
   * @param {!WebElement} a A WebElement.
   * @param {!WebElement} b A WebElement.
   * @return {!promise.Thenable<boolean>} A promise that will be
   *     resolved to whether the two WebElements are equal.
   */
  static equals(a, b) {
    if (a === b) {
      return a.driver_.controlFlow().promise(resolve => resolve(true));
    }
    let ids = [a.getId(), b.getId()];
    return promise.all(ids).then(function(ids) {
      // If the two element's have the same ID, they should be considered
      // equal. Otherwise, they may still be equivalent, but we'll need to
      // ask the server to check for us.
      if (ids[0] === ids[1]) {
        return true;
      }

      let cmd = new command.Command(command.Name.ELEMENT_EQUALS);
      cmd.setParameter('id', ids[0]);
      cmd.setParameter('other', ids[1]);
      return a.driver_.schedule(cmd, 'WebElement.equals()');
    });
  }

  /** @return {!WebDriver} The parent driver for this instance. */
  getDriver() {
    return this.driver_;
  }

  /**
   * @return {!promise.Thenable<string>} A promise that resolves to
   *     the server-assigned opaque ID assigned to this element.
   */
  getId() {
    return this.id_;
  }

  /**
   * @return {!Object} Returns the serialized representation of this WebElement.
   */
  [Symbols.serialize]() {
    return this.getId().then(WebElement.buildId);
  }

  /**
   * Schedules a command that targets this element with the parent WebDriver
   * instance. Will ensure this element's ID is included in the command
   * parameters under the "id" key.
   *
   * @param {!command.Command} command The command to schedule.
   * @param {string} description A description of the command for debugging.
   * @return {!promise.Thenable<T>} A promise that will be resolved
   *     with the command result.
   * @template T
   * @see WebDriver#schedule
   * @private
   */
  schedule_(command, description) {
    command.setParameter('id', this);
    return this.driver_.schedule(command, description);
  }

  /**
   * Schedule a command to find a descendant of this element. If the element
   * cannot be found, the returned promise will be rejected with a
   * {@linkplain error.NoSuchElementError NoSuchElementError}.
   *
   * The search criteria for an element may be defined using one of the static
   * factories on the {@link by.By} class, or ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.WebElementPromise"></a>[function <span class="apidocSignatureSpan">protractor.</span>WebElementPromise (driver, el)](#apidoc.element.protractor.WebElementPromise)
- description and source-code
```javascript
class WebElementPromise extends WebElement {
<span class="apidocCodeCommentSpan">  /**
   * @param {!WebDriver} driver The parent WebDriver instance for this
   *     element.
   * @param {!promise.Thenable<!WebElement>} el A promise
   *     that will resolve to the promised element.
   */
</span>  constructor(driver, el) {
    super(driver, 'unused');

    /**
     * Cancel operation is only supported if the wrapped thenable is also
     * cancellable.
     * @param {(string|Error)=} opt_reason
     * @override
     */
    this.cancel = function(opt_reason) {
      if (promise.CancellableThenable.isImplementation(el)) {
        /** @type {!promise.CancellableThenable} */(el).cancel(opt_reason);
      }
    }

    /** @override */
    this.then = el.then.bind(el);

    /** @override */
    this.catch = el.catch.bind(el);

    /**
     * Defers returning the element ID until the wrapped WebElement has been
     * resolved.
     * @override
     */
    this.getId = function() {
      return el.then(function(el) {
        return el.getId();
      });
    };
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.protractor.Key"></a>[module protractor.Key](#apidoc.module.protractor.Key)

#### <a name="apidoc.element.protractor.Key.chord"></a>[function <span class="apidocSignatureSpan">protractor.Key.</span>chord (var_args)](#apidoc.element.protractor.Key.chord)
- description and source-code
```javascript
chord = function (var_args) {
  return Array.prototype.slice.call(arguments, 0).join('') + Key.NULL;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.protractor.error"></a>[module protractor.error](#apidoc.module.protractor.error)

#### <a name="apidoc.element.protractor.error.ElementNotSelectableError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>ElementNotSelectableError (opt_error)](#apidoc.element.protractor.error.ElementNotSelectableError)
- description and source-code
```javascript
class ElementNotSelectableError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.ElementNotVisibleError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>ElementNotVisibleError (opt_error)](#apidoc.element.protractor.error.ElementNotVisibleError)
- description and source-code
```javascript
class ElementNotVisibleError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.InvalidArgumentError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>InvalidArgumentError (opt_error)](#apidoc.element.protractor.error.InvalidArgumentError)
- description and source-code
```javascript
class InvalidArgumentError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.InvalidCookieDomainError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>InvalidCookieDomainError (opt_error)](#apidoc.element.protractor.error.InvalidCookieDomainError)
- description and source-code
```javascript
class InvalidCookieDomainError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.InvalidElementCoordinatesError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>InvalidElementCoordinatesError (opt_error)](#apidoc.element.protractor.error.InvalidElementCoordinatesError)
- description and source-code
```javascript
class InvalidElementCoordinatesError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.InvalidElementStateError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>InvalidElementStateError (opt_error)](#apidoc.element.protractor.error.InvalidElementStateError)
- description and source-code
```javascript
class InvalidElementStateError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.InvalidSelectorError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>InvalidSelectorError (opt_error)](#apidoc.element.protractor.error.InvalidSelectorError)
- description and source-code
```javascript
class InvalidSelectorError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.JavascriptError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>JavascriptError (opt_error)](#apidoc.element.protractor.error.JavascriptError)
- description and source-code
```javascript
class JavascriptError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.MoveTargetOutOfBoundsError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>MoveTargetOutOfBoundsError (opt_error)](#apidoc.element.protractor.error.MoveTargetOutOfBoundsError)
- description and source-code
```javascript
class MoveTargetOutOfBoundsError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.NoSuchAlertError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>NoSuchAlertError (opt_error)](#apidoc.element.protractor.error.NoSuchAlertError)
- description and source-code
```javascript
class NoSuchAlertError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.NoSuchElementError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>NoSuchElementError (opt_error)](#apidoc.element.protractor.error.NoSuchElementError)
- description and source-code
```javascript
class NoSuchElementError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.NoSuchFrameError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>NoSuchFrameError (opt_error)](#apidoc.element.protractor.error.NoSuchFrameError)
- description and source-code
```javascript
class NoSuchFrameError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.NoSuchSessionError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>NoSuchSessionError (opt_error)](#apidoc.element.protractor.error.NoSuchSessionError)
- description and source-code
```javascript
class NoSuchSessionError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.NoSuchWindowError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>NoSuchWindowError (opt_error)](#apidoc.element.protractor.error.NoSuchWindowError)
- description and source-code
```javascript
class NoSuchWindowError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.ScriptTimeoutError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>ScriptTimeoutError (opt_error)](#apidoc.element.protractor.error.ScriptTimeoutError)
- description and source-code
```javascript
class ScriptTimeoutError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.SessionNotCreatedError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>SessionNotCreatedError (opt_error)](#apidoc.element.protractor.error.SessionNotCreatedError)
- description and source-code
```javascript
class SessionNotCreatedError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.StaleElementReferenceError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>StaleElementReferenceError (opt_error)](#apidoc.element.protractor.error.StaleElementReferenceError)
- description and source-code
```javascript
class StaleElementReferenceError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.TimeoutError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>TimeoutError (opt_error)](#apidoc.element.protractor.error.TimeoutError)
- description and source-code
```javascript
class TimeoutError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.UnableToCaptureScreenError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>UnableToCaptureScreenError (opt_error)](#apidoc.element.protractor.error.UnableToCaptureScreenError)
- description and source-code
```javascript
class UnableToCaptureScreenError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.UnableToSetCookieError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>UnableToSetCookieError (opt_error)](#apidoc.element.protractor.error.UnableToSetCookieError)
- description and source-code
```javascript
class UnableToSetCookieError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.UnexpectedAlertOpenError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>UnexpectedAlertOpenError (opt_error, opt_text)](#apidoc.element.protractor.error.UnexpectedAlertOpenError)
- description and source-code
```javascript
class UnexpectedAlertOpenError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /**
   * @param {string=} opt_error the error message, if any.
   * @param {string=} opt_text the text of the open dialog, if available.
   */
</span>  constructor(opt_error, opt_text) {
    super(opt_error);

    /** @private {(string|undefined)} */
    this.text_ = opt_text;
  }

  /**
   * @return {(string|undefined)} The text displayed with the unhandled alert,
   *     if available.
   */
  getAlertText() {
    return this.text_;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.UnknownCommandError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>UnknownCommandError (opt_error)](#apidoc.element.protractor.error.UnknownCommandError)
- description and source-code
```javascript
class UnknownCommandError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.UnknownMethodError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>UnknownMethodError (opt_error)](#apidoc.element.protractor.error.UnknownMethodError)
- description and source-code
```javascript
class UnknownMethodError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.UnsupportedOperationError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>UnsupportedOperationError (opt_error)](#apidoc.element.protractor.error.UnsupportedOperationError)
- description and source-code
```javascript
class UnsupportedOperationError extends WebDriverError {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.WebDriverError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>WebDriverError (opt_error)](#apidoc.element.protractor.error.WebDriverError)
- description and source-code
```javascript
class WebDriverError extends Error {
<span class="apidocCodeCommentSpan">  /** @param {string=} opt_error the error message, if any. */
</span>  constructor(opt_error) {
    super(opt_error);

    /** @override */
    this.name = this.constructor.name;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.checkLegacyResponse"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>checkLegacyResponse (responseObj)](#apidoc.element.protractor.error.checkLegacyResponse)
- description and source-code
```javascript
function checkLegacyResponse(responseObj) {
  // Handle the legacy Selenium error response format.
  if (responseObj
      && typeof responseObj === 'object'
      && typeof responseObj['status'] === 'number'
      && responseObj['status'] !== 0) {
    let status = responseObj['status'];
    let ctor = LEGACY_ERROR_CODE_TO_TYPE.get(status) || WebDriverError;

    let value = responseObj['value'];

    if (!value || typeof value !== 'object') {
      throw new ctor(value + '');
    } else {
      let message = value['message'] + '';
      if (ctor !== UnexpectedAlertOpenError) {
        throw new ctor(message);
      }

      let text = '';
      if (value['alert'] && typeof value['alert']['text'] === 'string') {
        text = value['alert']['text'];
      }
      throw new UnexpectedAlertOpenError(message, text);
    }
  }
  return responseObj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.checkResponse"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>checkResponse (data)](#apidoc.element.protractor.error.checkResponse)
- description and source-code
```javascript
function checkResponse(data) {
  if (data && typeof data.error === 'string') {
    let ctor = ERROR_CODE_TO_TYPE.get(data.error) || WebDriverError;
    throw new ctor(data.message);
  }
  return data;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.encodeError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>encodeError (err)](#apidoc.element.protractor.error.encodeError)
- description and source-code
```javascript
function encodeError(err) {
  let type = WebDriverError;
  if (err instanceof WebDriverError
      && TYPE_TO_ERROR_CODE.has(err.constructor)) {
    type = err.constructor;
  }

  let message = err instanceof Error
      ? err.message
      : err + '';

  let code = /** @type {string} */(TYPE_TO_ERROR_CODE.get(type));
  return {'error': code, 'message': message};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.error.throwDecodedError"></a>[function <span class="apidocSignatureSpan">protractor.error.</span>throwDecodedError (data)](#apidoc.element.protractor.error.throwDecodedError)
- description and source-code
```javascript
function throwDecodedError(data) {
  if (data && typeof data === 'object' && typeof data.error === 'string') {
    let ctor = ERROR_CODE_TO_TYPE.get(data.error) || WebDriverError;
    throw new ctor(data.message);
  }
  throw new WebDriverError('Unknown error: ' + JSON.stringify(data));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.protractor.logging"></a>[module protractor.logging](#apidoc.module.protractor.logging)

#### <a name="apidoc.element.protractor.logging.Entry"></a>[function <span class="apidocSignatureSpan">protractor.logging.</span>Entry (!Level|string|number)](#apidoc.element.protractor.logging.Entry)
- description and source-code
```javascript
class Entry {
<span class="apidocCodeCommentSpan">  /**
   * @param {(!Level|string|number)} level The entry level.
   * @param {string} message The log message.
   * @param {number=} opt_timestamp The time this entry was generated, in
   *     milliseconds since 0:00:00, January 1, 1970 UTC. If omitted, the
   *     current time will be used.
   * @param {string=} opt_type The log type, if known.
   */
</span>  constructor(level, message, opt_timestamp, opt_type) {
    this.level = level instanceof Level ? level : getLevel(level);
    this.message = message;
    this.timestamp =
        typeof opt_timestamp === 'number' ? opt_timestamp : Date.now();
    this.type = opt_type || '';
  }

  /**
   * @return {{level: string, message: string, timestamp: number,
   *           type: string}} The JSON representation of this entry.
   */
  toJSON() {
    return {
      'level': this.level.name,
      'message': this.message,
      'timestamp': this.timestamp,
      'type': this.type
    };
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.logging.Level"></a>[function <span class="apidocSignatureSpan">protractor.logging.</span>Level (name, level)](#apidoc.element.protractor.logging.Level)
- description and source-code
```javascript
class Level {
<span class="apidocCodeCommentSpan">  /**
   * @param {string} name the level's name.
   * @param {number} level the level's numeric value.
   */
</span>  constructor(name, level) {
    if (level < 0) {
      throw new TypeError('Level must be >= 0');
    }

    /** @private {string} */
    this.name_ = name;

    /** @private {number} */
    this.value_ = level;
  }

  /** This logger's name. */
  get name() {
    return this.name_;
  }

  /** The numeric log level. */
  get value() {
    return this.value_;
  }

  /** @override */
  toString() {
    return this.name;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.logging.LogManager"></a>[function <span class="apidocSignatureSpan">protractor.logging.</span>LogManager ()](#apidoc.element.protractor.logging.LogManager)
- description and source-code
```javascript
class LogManager {
  constructor() {
<span class="apidocCodeCommentSpan">    /** @private {!Map<string, !Logger>} */
</span>    this.loggers_ = new Map;
    this.root_ = new Logger('', Level.OFF);
  }

  /**
   * Retrieves a named logger, creating it in the process. This function will
   * implicitly create the requested logger, and any of its parents, if they
   * do not yet exist.
   *
   * @param {string} name the logger's name.
   * @return {!Logger} the requested logger.
   */
  getLogger(name) {
    if (!name) {
      return this.root_;
    }
    let parent = this.root_;
    for (let i = name.indexOf('.'); i != -1; i = name.indexOf('.', i + 1)) {
      let parentName = name.substr(0, i);
      parent = this.createLogger_(parentName, parent);
    }
    return this.createLogger_(name, parent);
  }

  /**
   * Creates a new logger.
   *
   * @param {string} name the logger's name.
   * @param {!Logger} parent the logger's parent.
   * @return {!Logger} the new logger.
   * @private
   */
  createLogger_(name, parent) {
    if (this.loggers_.has(name)) {
      return /** @type {!Logger} */(this.loggers_.get(name));
    }
    let logger = new Logger(name, null);
    logger.parent_ = parent;
    this.loggers_.set(name, logger);
    return logger;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.logging.Logger"></a>[function <span class="apidocSignatureSpan">protractor.logging.</span>Logger (name, opt_level)](#apidoc.element.protractor.logging.Logger)
- description and source-code
```javascript
class Logger {
<span class="apidocCodeCommentSpan">  /**
   * @param {string} name the name of this logger.
   * @param {Level=} opt_level the initial level for this logger.
   */
</span>  constructor(name, opt_level) {
    /** @private {string} */
    this.name_ = name;

    /** @private {Level} */
    this.level_ = opt_level || null;

    /** @private {Logger} */
    this.parent_ = null;

    /** @private {Set<function(!Entry)>} */
    this.handlers_ = null;
  }

  /** @return {string} the name of this logger. */
  getName() {
    return this.name_;
  }

  /**
   * @param {Level} level the new level for this logger, or 'null' if the logger
   *     should inherit its level from its parent logger.
   */
  setLevel(level) {
    this.level_ = level;
  }

  /** @return {Level} the log level for this logger. */
  getLevel() {
    return this.level_;
  }

  /**
   * @return {!Level} the effective level for this logger.
   */
  getEffectiveLevel() {
    let logger = this;
    let level;
    do {
      level = logger.level_;
      logger = logger.parent_;
    } while (logger && !level);
    return level || Level.OFF;
  }

  /**
   * @param {!Level} level the level to check.
   * @return {boolean} whether messages recorded at the given level are loggable
   *     by this instance.
   */
  isLoggable(level) {
    return level.value !== Level.OFF.value
        && level.value >= this.getEffectiveLevel().value;
  }

  /**
   * Adds a handler to this logger. The handler will be invoked for each message
   * logged with this instance, or any of its descendants.
   *
   * @param {function(!Entry)} handler the handler to add.
   */
  addHandler(handler) {
    if (!this.handlers_) {
      this.handlers_ = new Set;
    }
    this.handlers_.add(handler);
  }

  /**
   * Removes a handler from this logger.
   *
   * @param {function(!Entry)} handler the handler to remove.
   * @return {boolean} whether a handler was successfully removed.
   */
  removeHandler(handler) {
    if (!this.handlers_) {
      return false;
    }
    return this.handlers_.delete(handler);
  }

  /**
   * Logs a message at the given level. The message may be defined as a string
   * or as a function that will return the message. If a function is provided,
   * it will only be invoked if this logger's
   * {@linkplain #getEffectiveLevel() effective log level} includes the given
   * 'level'.
   *
   * @param {!Level} level the level at which to log the message.
   * @param {(string|function(): string)} loggable the message to log, or a
   *     function that will return the message.
   */
  log(level, loggable) {
    if (!this.isLoggable(level)) {
      return;
    }
    let message = '[' + this.name_ + '] '
        + (typeof loggable === 'function' ? loggable() : loggable);
    let entry = new Entry(level, message, Date.now());
    for (let logger = this; !!logger; logger = logger.parent_) {
      if (logger.handlers_) {
        for (let handler of logger.handlers_) {
          handler(entry);
        }
      }
    }
  }

  /**
   * Logs a message at the {@link Level.SEVERE} log level.
   * @param {(string|function(): string)} loggable the message to log, or a
   *     function that will return the message.
   */
  severe(loggable) {
    this.log(Level.SEVERE, loggable);
  }

  /**
   * Logs a message at the {@link Level.WARNING} log level.
   * @param {(string|function(): string)} loggable the message to log, or a
   *     function that will return the message.
   */
  warning(loggable) {
    this.log(Level.WARNING, loggable);
  }

  /**
   * Logs a message at the {@link Level.INFO} log level.
   * @param {(string|function(): string)} loggable the message to log, or a
   *     function that will return the message.
   */
  info(loggable) {
    this.log(Level.INFO, loggable);
  }

  /**
   * Logs a message at the {@link Level.DEBUG} log level.
   * @param {(string|function(): string)} loggable the message to log, or a
   *     function that will return the message.
   */
  debug(loggable) {
    this.log(Level.DEBUG, loggable);
  }

  /**
   * Logs a message at the {@link Level.FINE} log level.
   * @param { ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.logging.Preferences"></a>[function <span class="apidocSignatureSpan">protractor.logging.</span>Preferences ()](#apidoc.element.protractor.logging.Preferences)
- description and source-code
```javascript
class Preferences {
  constructor() {
<span class="apidocCodeCommentSpan">    /** @private {!Map<string, !Level>} */
</span>    this.prefs_ = new Map;
  }

  /**
   * Sets the desired logging level for a particular log type.
   * @param {(string|Type)} type The log type.
   * @param {(!Level|string|number)} level The desired log level.
   * @throws {TypeError} if 'type' is not a 'string'.
   */
  setLevel(type, level) {
    if (typeof type !== 'string') {
      throw TypeError('specified log type is not a string: ' + typeof type);
    }
    this.prefs_.set(type, level instanceof Level ? level : getLevel(level));
  }

  /**
   * Converts this instance to its JSON representation.
   * @return {!Object<string, string>} The JSON representation of this set of
   *     preferences.
   */
  toJSON() {
    let json = {};
    for (let key of this.prefs_.keys()) {
      json[key] = this.prefs_.get(key).name;
    }
    return json;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.logging.addConsoleHandler"></a>[function <span class="apidocSignatureSpan">protractor.logging.</span>addConsoleHandler (opt_logger)](#apidoc.element.protractor.logging.addConsoleHandler)
- description and source-code
```javascript
function addConsoleHandler(opt_logger) {
  let logger = opt_logger || logManager.root_;
  logger.addHandler(consoleHandler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.logging.getLevel"></a>[function <span class="apidocSignatureSpan">protractor.logging.</span>getLevel (nameOrValue)](#apidoc.element.protractor.logging.getLevel)
- description and source-code
```javascript
function getLevel(nameOrValue) {
  if (typeof nameOrValue === 'string') {
    return LEVELS_BY_NAME.get(nameOrValue) || Level.ALL;
  }
  if (typeof nameOrValue !== 'number') {
    throw new TypeError('not a string or number');
  }
  for (let level of ALL_LEVELS) {
    if (nameOrValue >= level.value) {
      return level;
    }
  }
  return Level.ALL;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.logging.getLogger"></a>[function <span class="apidocSignatureSpan">protractor.logging.</span>getLogger (name)](#apidoc.element.protractor.logging.getLogger)
- description and source-code
```javascript
function getLogger(name) {
  return logManager.getLogger(name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.logging.installConsoleHandler"></a>[function <span class="apidocSignatureSpan">protractor.logging.</span>installConsoleHandler ()](#apidoc.element.protractor.logging.installConsoleHandler)
- description and source-code
```javascript
function installConsoleHandler() {
  addConsoleHandler(logManager.root_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.logging.removeConsoleHandler"></a>[function <span class="apidocSignatureSpan">protractor.logging.</span>removeConsoleHandler (opt_logger)](#apidoc.element.protractor.logging.removeConsoleHandler)
- description and source-code
```javascript
function removeConsoleHandler(opt_logger) {
  let logger = opt_logger || logManager.root_;
  logger.removeHandler(consoleHandler);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.protractor.promise"></a>[module protractor.promise](#apidoc.module.protractor.promise)

#### <a name="apidoc.element.protractor.promise.CancellableThenable"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>CancellableThenable (new: CancellableThenable, ...?)](#apidoc.element.protractor.promise.CancellableThenable)
- description and source-code
```javascript
class CancellableThenable {
<span class="apidocCodeCommentSpan">  /**
   * @param {function(new: CancellableThenable, ...?)} ctor
   */
</span>  static addImplementation(ctor) {
    Thenable.addImplementation(ctor);
    addMarkerSymbol(ctor, CANCELLABLE_SYMBOL);
  }

  /**
   * @param {*} object
   * @return {boolean}
   */
  static isImplementation(object) {
    return hasMarkerSymbol(object, CANCELLABLE_SYMBOL);
  }

  /**
   * Requests the cancellation of the computation of this promise's value,
   * rejecting the promise in the process. This method is a no-op if the promise
   * has already been resolved.
   *
   * @param {(string|Error)=} opt_reason The reason this promise is being
   *     cancelled. This value will be wrapped in a {@link CancellationError}.
   */
  cancel(opt_reason) {}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.CancellationError"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>CancellationError (opt_msg)](#apidoc.element.protractor.promise.CancellationError)
- description and source-code
```javascript
class CancellationError extends Error {
<span class="apidocCodeCommentSpan">  /**
   * @param {string=} opt_msg The cancellation message.
   */
</span>  constructor(opt_msg) {
    super(opt_msg);

    /** @override */
    this.name = this.constructor.name;

    /** @private {boolean} */
    this.silent_ = false;
  }

  /**
   * Wraps the given error in a CancellationError.
   *
   * @param {*} error The error to wrap.
   * @param {string=} opt_msg The prefix message to use.
   * @return {!CancellationError} A cancellation error.
   */
  static wrap(error, opt_msg) {
    var message;
    if (error instanceof CancellationError) {
      return new CancellationError(
          opt_msg ? (opt_msg + ': ' + error.message) : error.message);
    } else if (opt_msg) {
      message = opt_msg;
      if (error) {
        message += ': ' + error;
      }
      return new CancellationError(message);
    }
    if (error) {
      message = error + '';
    }
    return new CancellationError(message);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.ControlFlow"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>ControlFlow ()](#apidoc.element.protractor.promise.ControlFlow)
- description and source-code
```javascript
class ControlFlow extends events.EventEmitter {
  constructor() {
    if (!usePromiseManager()) {
      throw TypeError(
          'Cannot instantiate control flow when the promise manager has'
              + ' been disabled');
    }

    super();

<span class="apidocCodeCommentSpan">    /** @private {boolean} */
</span>    this.propagateUnhandledRejections_ = true;

    /** @private {TaskQueue} */
    this.activeQueue_ = null;

    /** @private {Set<TaskQueue>} */
    this.taskQueues_ = null;

    /**
     * Micro task that controls shutting down the control flow. Upon shut down,
     * the flow will emit an
     * {@link ControlFlow.EventType.IDLE} event. Idle events
     * always follow a brief timeout in order to catch latent errors from the
     * last completed task. If this task had a callback registered, but no
     * errback, and the task fails, the unhandled failure would not be reported
     * by the promise system until the next turn of the event loop:
     *
     *   // Schedule 1 task that fails.
     *   var result = promise.controlFlow().schedule('example',
     *       function() { return promise.rejected('failed'); });
     *   // Set a callback on the result. This delays reporting the unhandled
     *   // failure for 1 turn of the event loop.
     *   result.then(function() {});
     *
     * @private {MicroTask}
     */
    this.shutdownTask_ = null;

    /**
     * ID for a long running interval used to keep a Node.js process running
     * while a control flow's event loop is still working. This is a cheap hack
     * required since JS events are only scheduled to run when there is
     * _actually_ something to run. When a control flow is waiting on a task,
     * there will be nothing in the JS event loop and the process would
     * terminate without this.
     * @private
     */
    this.hold_ = null;
  }

  /**
   * Returns a string representation of this control flow, which is its current
   * {@linkplain #getSchedule() schedule}, sans task stack traces.
   * @return {string} The string representation of this contorl flow.
   * @override
   */
  toString() {
    return this.getSchedule();
  }

  /**
   * Sets whether any unhandled rejections should propagate up through the
   * control flow stack and cause rejections within parent tasks. If error
   * propagation is disabled, tasks will not be aborted when an unhandled
   * promise rejection is detected, but the rejection _will_ trigger an
   * {@link ControlFlow.EventType.UNCAUGHT_EXCEPTION}
   * event.
   *
   * The default behavior is to propagate all unhandled rejections. _The use
   * of this option is highly discouraged._
   *
   * @param {boolean} propagate whether to propagate errors.
   */
  setPropagateUnhandledRejections(propagate) {
    this.propagateUnhandledRejections_ = propagate;
  }

  /**
   * @return {boolean} Whether this flow is currently idle.
   */
  isIdle() {
    return !this.shutdownTask_ && (!this.taskQueues_ || !this.taskQueues_.size);
  }

  /**
   * Resets this instance, clearing its queue and removing all event listeners.
   */
  reset() {
    this.cancelQueues_(new FlowResetError);
    this.emit(ControlFlow.EventType.RESET);
    this.removeAllListeners();
    this.cancelShutdown_();
  }

  /**
   * Generates an annotated string describing the internal state of this control
   * flow, including the currently executing as well as pending tasks. If
   * {@code opt_includeStackTraces === true}, the string will include the
   * stack trace from when each task was scheduled.
   * @param {string=} opt_includeStackTraces Whether to include the stack traces
   *     from when each task was scheduled. Defaults to false.
   * @return {string} String representation of this flow's internal state.
   */
  getSchedule(opt_includeStackTraces) {
    var ret = 'ControlFlow::' + getUid(this);
    var activeQueue = this.activeQueue_;
    if (!this.taskQueues_ || !this.taskQueues_.size) {
      return ret;
    }
    var childIndent = '| ';
    for (var q of this.taskQueues_) {
      ret += '\n' + printQ(q, childIndent);
    }
    return ret;

    function printQ(q, indent) ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.Deferred"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>Deferred (opt_flow)](#apidoc.element.protractor.promise.Deferred)
- description and source-code
```javascript
class Deferred {
<span class="apidocCodeCommentSpan">  /**
   * @param {ControlFlow=} opt_flow The control flow this instance was
   *     created under. This should only be provided during unit tests.
   */
</span>  constructor(opt_flow) {
    var fulfill, reject;

    /** @type {!ManagedPromise<T>} */
    this.promise = new ManagedPromise(function(f, r) {
      fulfill = f;
      reject = r;
    }, opt_flow);

    var self = this;
    var checkNotSelf = function(value) {
      if (value === self) {
        throw new TypeError('May not resolve a Deferred with itself');
      }
    };

    /**
     * Resolves this deferred with the given value. It is safe to call this as a
     * normal function (with no bound "this").
     * @param {(T|IThenable<T>|Thenable)=} opt_value The fulfilled value.
     */
    this.fulfill = function(opt_value) {
      checkNotSelf(opt_value);
      fulfill(opt_value);
    };

    /**
     * Rejects this promise with the given reason. It is safe to call this as a
     * normal function (with no bound "this").
     * @param {*=} opt_reason The rejection reason.
     */
    this.reject = function(opt_reason) {
      checkNotSelf(opt_reason);
      reject(opt_reason);
    };
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.MultipleUnhandledRejectionError"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>MultipleUnhandledRejectionError (Set<*>)](#apidoc.element.protractor.promise.MultipleUnhandledRejectionError)
- description and source-code
```javascript
class MultipleUnhandledRejectionError extends Error {
<span class="apidocCodeCommentSpan">  /**
   * @param {!(Set<*>)} errors The errors to report.
   */
</span>  constructor(errors) {
    super('Multiple unhandled promise rejections reported');

    /** @override */
    this.name = this.constructor.name;

    /** @type {!Set<*>} */
    this.errors = errors;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.Promise"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>Promise ( * function((T|IThenable<T>|Thenable)](#apidoc.element.protractor.promise.Promise)
- description and source-code
```javascript
class ManagedPromise {
<span class="apidocCodeCommentSpan">  /**
   * @param {function( * function((T|IThenable<T>|Thenable)=),
   *           function(*=))} resolver
   *     Function that is invoked immediately to begin computation of this
   *     promise's value. The function should accept a pair of callback
   *     functions, one for fulfilling the promise and another for rejecting it.
   * @param {ControlFlow=} opt_flow The control flow
   *     this instance was created under. Defaults to the currently active flow.
   */
</span>  constructor(resolver, opt_flow) {
    if (!usePromiseManager()) {
      throw TypeError(
        'Unable to create a managed promise instance: the promise manager has'
            + ' been disabled by the SELENIUM_PROMISE_MANAGER environment'
            + ' variable: ' + process.env['SELENIUM_PROMISE_MANAGER']);
    }
    getUid(this);

    /** @private {!ControlFlow} */
    this.flow_ = opt_flow || controlFlow();

    /** @private {Error} */
    this.stack_ = null;
    if (LONG_STACK_TRACES) {
      this.stack_ = captureStackTrace('ManagedPromise', 'new', this.constructor);
    }

    /** @private {Thenable<?>} */
    this.parent_ = null;

    /** @private {Array<!Task>} */
    this.callbacks_ = null;

    /** @private {PromiseState} */
    this.state_ = PromiseState.PENDING;

    /** @private {boolean} */
    this.handled_ = false;

    /** @private {*} */
    this.value_ = undefined;

    /** @private {TaskQueue} */
    this.queue_ = null;

    try {
      var self = this;
      resolver(function(value) {
        self.resolve_(PromiseState.FULFILLED, value);
      }, function(reason) {
        self.resolve_(PromiseState.REJECTED, reason);
      });
    } catch (ex) {
      this.resolve_(PromiseState.REJECTED, ex);
    }
  }

  /**
   * Creates a promise that is immediately resolved with the given value.
   *
   * @param {T=} opt_value The value to resolve.
   * @return {!ManagedPromise<T>} A promise resolved with the given value.
   * @template T
   */
  static resolve(opt_value) {
    if (opt_value instanceof ManagedPromise) {
      return opt_value;
    }
    return new ManagedPromise(resolve => resolve(opt_value));
  }

  /**
   * Creates a promise that is immediately rejected with the given reason.
   *
   * @param {*=} opt_reason The rejection reason.
   * @return {!ManagedPromise<?>} A new rejected promise.
   */
  static reject(opt_reason) {
    return new ManagedPromise((_, reject) => reject(opt_reason));
  }

  /** @override */
  toString() {
    return 'ManagedPromise::' + getUid(this) +
      ' {[[PromiseStatus]]: "' + this.state_ + '"}';
  }

  /**
   * Resolves this promise. If the new value is itself a promise, this function
   * will wait for it to be resolved before notifying the registered listeners.
   * @param {PromiseState} newState The promise's new state.
   * @param {*} newValue The promise's new value.
   * @throws {TypeError} If {@code newValue === this}.
   * @private
   */
  resolve_(newState, newValue) {
    if (PromiseState.PENDING !== this.state_) {
      return;
    }

    if (newValue === this) {
      // See promise a+, 2.3.1
      // http://promises-aplus.github.io/promises-spec/#point-48
      newValue = new TypeError('A promise may not resolve to itself');
      newState = PromiseState.REJECTED;
    }

    this.parent_ = null;
    this.state_ = PromiseState.BLOCKED;

    if (newState !== PromiseState.REJECTED) {
      if (Thenable.isImplementation(newValue)) {
        // 2.3.2
        newValue = /** @type {!Thenable} */(newValue);
        this.parent_ = newValue;
        newValue.then(
            this.unblockAndResolve_.bind(this, PromiseState.FULFILLED),
            this.unblockAndResolve_.bind(this, PromiseState.REJECTED));
        return;

      } else if (newValue
          && (typeof newValue === 'object' || typeof newValue === 'function')) {
        // 2.3.3

        try {
          // 2.3.3.1
          var then = newValue['then'];
        } catch (e) {
          // 2.3.3.2
          this.state_ = PromiseState.REJECTED;
          this.value_ = e;
          this.scheduleN ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.Scheduler"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>Scheduler ()](#apidoc.element.protractor.promise.Scheduler)
- description and source-code
```javascript
class Scheduler {
<span class="apidocCodeCommentSpan">  /**
   * Schedules a task for execution. If the task function is a generator, the
   * task will be executed using {@link ./promise.consume consume()}.
   *
   * @param {function(): (T|IThenable<T>)} fn The function to call to start the
   *     task.
   * @param {string=} opt_description A description of the task for debugging
   *     purposes.
   * @return {!Thenable<T>} A promise that will be resolved with the task
   *     result.
   * @template T
   */
</span>  execute(fn, opt_description) {}

  /**
   * Creates a new promise using the given resolver function.
   *
   * @param {function(
   *             function((T|IThenable<T>|Thenable|null)=),
   *             function(*=))} resolver
   * @return {!Thenable<T>}
   * @template T
   */
  promise(resolver) {}

  /**
   * Schedules a 'setTimeout' call.
   *
   * @param {number} ms The timeout delay, in milliseconds.
   * @param {string=} opt_description A description to accompany the timeout.
   * @return {!Thenable<void>} A promise that will be resolved when the timeout
   *     fires.
   */
  timeout(ms, opt_description) {}

  /**
   * Schedules a task to wait for a condition to hold.
   *
   * If the condition is defined as a function, it may return any value. Promies
   * will be resolved before testing if the condition holds (resolution time
   * counts towards the timeout). Once resolved, values are always evaluated as
   * booleans.
   *
   * If the condition function throws, or returns a rejected promise, the
   * wait task will fail.
   *
   * If the condition is defined as a promise, the scheduler will wait for it to
   * settle. If the timeout expires before the promise settles, the promise
   * returned by this function will be rejected.
   *
   * If this function is invoked with 'timeout === 0', or the timeout is
   * omitted, this scheduler will wait indefinitely for the condition to be
   * satisfied.
   *
   * @param {(!IThenable<T>|function())} condition The condition to poll,
   *     or a promise to wait on.
   * @param {number=} opt_timeout How long to wait, in milliseconds, for the
   *     condition to hold before timing out. If omitted, the flow will wait
   *     indefinitely.
   * @param {string=} opt_message An optional error message to include if the
   *     wait times out; defaults to the empty string.
   * @return {!Thenable<T>} A promise that will be fulfilled
   *     when the condition has been satisified. The promise shall be rejected
   *     if the wait times out waiting for the condition.
   * @throws {TypeError} If condition is not a function or promise or if timeout
   *     is not a number >= 0.
   * @template T
   */
  wait(condition, opt_timeout, opt_message) {}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.Thenable"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>Thenable (new: Thenable, ...?)](#apidoc.element.protractor.promise.Thenable)
- description and source-code
```javascript
class Thenable {
<span class="apidocCodeCommentSpan">  /**
   * Adds a property to a class prototype to allow runtime checks of whether
   * instances of that class implement the Thenable interface.
   * @param {function(new: Thenable, ...?)} ctor The
   *     constructor whose prototype to modify.
   */
</span>  static addImplementation(ctor) {
    addMarkerSymbol(ctor, IMPLEMENTED_BY_SYMBOL);
  }

  /**
   * Checks if an object has been tagged for implementing the Thenable
   * interface as defined by {@link Thenable.addImplementation}.
   * @param {*} object The object to test.
   * @return {boolean} Whether the object is an implementation of the Thenable
   *     interface.
   */
  static isImplementation(object) {
    return hasMarkerSymbol(object, IMPLEMENTED_BY_SYMBOL);
  }

  /**
   * Registers listeners for when this instance is resolved.
   *
   * @param {?(function(T): (R|IThenable<R>))=} opt_callback The
   *     function to call if this promise is successfully resolved. The function
   *     should expect a single argument: the promise's resolved value.
   * @param {?(function(*): (R|IThenable<R>))=} opt_errback
   *     The function to call if this promise is rejected. The function should
   *     expect a single argument: the rejection reason.
   * @return {!Thenable<R>} A new promise which will be resolved with the result
   *     of the invoked callback.
   * @template R
   */
  then(opt_callback, opt_errback) {}

  /**
   * Registers a listener for when this promise is rejected. This is synonymous
   * with the {@code catch} clause in a synchronous API:
   *
   *     // Synchronous API:
   *     try {
   *       doSynchronousWork();
   *     } catch (ex) {
   *       console.error(ex);
   *     }
   *
   *     // Asynchronous promise API:
   *     doAsynchronousWork().catch(function(ex) {
   *       console.error(ex);
   *     });
   *
   * @param {function(*): (R|IThenable<R>)} errback The
   *     function to call if this promise is rejected. The function should
   *     expect a single argument: the rejection reason.
   * @return {!Thenable<R>} A new promise which will be resolved with the result
   *     of the invoked callback.
   * @template R
   */
  catch(errback) {}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.all"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>all (arr)](#apidoc.element.protractor.promise.all)
- description and source-code
```javascript
function all(arr) {
  return createPromise(function(fulfill, reject) {
    var n = arr.length;
    var values = [];

    if (!n) {
      fulfill(values);
      return;
    }

    var toFulfill = n;
    var onFulfilled = function(index, value) {
      values[index] = value;
      toFulfill--;
      if (toFulfill == 0) {
        fulfill(values);
      }
    };

    function processPromise(index) {
      asap(arr[index], function(value) {
        onFulfilled(index, value);
      }, reject);
    }

    for (var i = 0; i < n; ++i) {
      processPromise(i);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.asap"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>asap (value, callback, opt_errback)](#apidoc.element.protractor.promise.asap)
- description and source-code
```javascript
function asap(value, callback, opt_errback) {
  if (isPromise(value)) {
    value.then(callback, opt_errback);

  } else if (callback) {
    callback(value);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.captureStackTrace"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>captureStackTrace (name, msg, opt_topFn)](#apidoc.element.protractor.promise.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(name, msg, opt_topFn) {
  var e = Error(msg);
  e.name = name;
  if (Error.captureStackTrace) {
    Error.captureStackTrace(e, opt_topFn);
  } else {
    var stack = Error().stack;
    if (stack) {
      e.stack = e.toString();
      e.stack += '\n' + stack;
    }
  }
  return e;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.checkedNodeCall"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>checkedNodeCall (fn, var_args)](#apidoc.element.protractor.promise.checkedNodeCall)
- description and source-code
```javascript
function checkedNodeCall(fn, var_args) {
  let args = Array.prototype.slice.call(arguments, 1);
  return createPromise(function(fulfill, reject) {
    try {
      args.push(function(error, value) {
        error ? reject(error) : fulfill(value);
      });
      fn.apply(undefined, args);
    } catch (ex) {
      reject(ex);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.consume"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>consume (generatorFn, opt_self, ...var_args)](#apidoc.element.protractor.promise.consume)
- description and source-code
```javascript
function consume(generatorFn, opt_self, ...var_args) {
  if (!isGenerator(generatorFn)) {
    throw new TypeError('Input is not a GeneratorFunction: ' +
        generatorFn.constructor.name);
  }

  let ret;
  return ret = createPromise((resolve, reject) => {
    let generator = generatorFn.apply(opt_self, var_args);
    callNext();

<span class="apidocCodeCommentSpan">    /** @param {*=} opt_value . */
</span>    function callNext(opt_value) {
      pump(generator.next, opt_value);
    }

    /** @param {*=} opt_error . */
    function callThrow(opt_error) {
      pump(generator.throw, opt_error);
    }

    function pump(fn, opt_arg) {
      if (ret instanceof ManagedPromise && !isPending(ret)) {
        return;  // Defererd was cancelled; silently abort.
      }

      try {
        var result = fn.call(generator, opt_arg);
      } catch (ex) {
        reject(ex);
        return;
      }

      if (result.done) {
        resolve(result.value);
        return;
      }

      asap(result.value, callNext, callThrow);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.controlFlow"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>controlFlow ()](#apidoc.element.protractor.promise.controlFlow)
- description and source-code
```javascript
function controlFlow() {
  if (!usePromiseManager()) {
    return SIMPLE_SCHEDULER;
  }

  if (activeFlows.length) {
    return activeFlows[activeFlows.length - 1];
  }

  if (!defaultFlow) {
    defaultFlow = new ControlFlow;
  }
  return defaultFlow;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.createFlow"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>createFlow (callback)](#apidoc.element.protractor.promise.createFlow)
- description and source-code
```javascript
function createFlow(callback) {
  var flow = new ControlFlow;
  return flow.execute(function() {
    return callback(flow);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.defer"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>defer ()](#apidoc.element.protractor.promise.defer)
- description and source-code
```javascript
function defer() {
  return new Deferred();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.delayed"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>delayed (ms)](#apidoc.element.protractor.promise.delayed)
- description and source-code
```javascript
function delayed(ms) {
  return createPromise(resolve => {
    setTimeout(() => resolve(), ms);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.filter"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>filter (arr, fn, opt_self)](#apidoc.element.protractor.promise.filter)
- description and source-code
```javascript
function filter(arr, fn, opt_self) {
  return createPromise(resolve => resolve(arr)).then(v => {
    if (!Array.isArray(v)) {
      throw TypeError('not an array');
    }
    var arr = /** @type {!Array} */(v);
    return createPromise(function(fulfill, reject) {
      var n = arr.length;
      var values = [];
      var valuesLength = 0;
      (function processNext(i) {
        for (; i < n; i++) {
          if (i in arr) {
            break;
          }
        }
        if (i >= n) {
          fulfill(values);
          return;
        }
        try {
          var value = arr[i];
          var include = fn.call(opt_self, value, i, /** @type {!Array} */(arr));
          asap(include, function(include) {
            if (include) {
              values[valuesLength++] = value;
            }
            processNext(i + 1);
            }, reject);
        } catch (ex) {
          reject(ex);
        }
      })(0);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.finally"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>finally (promise, callback)](#apidoc.element.protractor.promise.finally)
- description and source-code
```javascript
function thenFinally(promise, callback) {
  let error;
  let mustThrow = false;
  return promise.then(function() {
    return callback();
  }, function(err) {
    error = err;
    mustThrow = true;
    return callback();
  }).then(function() {
    if (mustThrow) {
      throw error;
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.fulfilled"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>fulfilled (opt_value)](#apidoc.element.protractor.promise.fulfilled)
- description and source-code
```javascript
function fulfilled(opt_value) {
  return ManagedPromise.resolve(opt_value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.fullyResolved"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>fullyResolved (value)](#apidoc.element.protractor.promise.fullyResolved)
- description and source-code
```javascript
function fullyResolved(value) {
  if (isPromise(value)) {
    return when(value, fullyResolveValue);
  }
  return fullyResolveValue(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.isGenerator"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>isGenerator (fn)](#apidoc.element.protractor.promise.isGenerator)
- description and source-code
```javascript
function isGenerator(fn) {
  return fn.constructor.name === 'GeneratorFunction';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.isPromise"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>isPromise (value)](#apidoc.element.protractor.promise.isPromise)
- description and source-code
```javascript
function isPromise(value) {
  try {
    // Use array notation so the Closure compiler does not obfuscate away our
    // contract.
    return value
        && (typeof value === 'object' || typeof value === 'function')
        && typeof value['then'] === 'function';
  } catch (ex) {
    return false;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.map"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>map (arr, fn, opt_self)](#apidoc.element.protractor.promise.map)
- description and source-code
```javascript
function map(arr, fn, opt_self) {
  return createPromise(resolve => resolve(arr)).then(v => {
    if (!Array.isArray(v)) {
      throw TypeError('not an array');
    }
    var arr = /** @type {!Array} */(v);
    return createPromise(function(fulfill, reject) {
      var n = arr.length;
      var values = new Array(n);
      (function processNext(i) {
        for (; i < n; i++) {
          if (i in arr) {
            break;
          }
        }
        if (i >= n) {
          fulfill(values);
          return;
        }
        try {
          asap(
              fn.call(opt_self, arr[i], i, /** @type {!Array} */(arr)),
              function(value) {
                values[i] = value;
                processNext(i + 1);
              },
              reject);
        } catch (ex) {
          reject(ex);
        }
      })(0);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.rejected"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>rejected (opt_reason)](#apidoc.element.protractor.promise.rejected)
- description and source-code
```javascript
function rejected(opt_reason) {
  return ManagedPromise.reject(opt_reason);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.setDefaultFlow"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>setDefaultFlow (flow)](#apidoc.element.protractor.promise.setDefaultFlow)
- description and source-code
```javascript
function setDefaultFlow(flow) {
  if (!usePromiseManager()) {
    throw Error(
        'You  may not change set the control flow when the promise'
            +' manager is disabled');
  }
  if (activeFlows.length) {
    throw Error('You may only change the default flow while it is active');
  }
  defaultFlow = flow;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.promise.when"></a>[function <span class="apidocSignatureSpan">protractor.promise.</span>when (value, opt_callback, opt_errback)](#apidoc.element.protractor.promise.when)
- description and source-code
```javascript
function when(value, opt_callback, opt_errback) {
  if (Thenable.isImplementation(value)) {
    return value.then(opt_callback, opt_errback);
  }

  return createPromise(resolve => resolve(value))
      .then(opt_callback, opt_errback);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.protractor.until"></a>[module protractor.until](#apidoc.module.protractor.until)

#### <a name="apidoc.element.protractor.until.ableToSwitchToFrame"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>ableToSwitchToFrame (frame)](#apidoc.element.protractor.until.ableToSwitchToFrame)
- description and source-code
```javascript
function ableToSwitchToFrame(frame) {
  var condition;
  if (typeof frame === 'number' || frame instanceof webdriver.WebElement) {
    condition = attemptToSwitchFrames;
  } else {
    condition = function(driver) {
      let locator = /** @type {!(By|Function)} */(frame);
      return driver.findElements(locator).then(function(els) {
        if (els.length) {
          return attemptToSwitchFrames(driver, els[0]);
        }
      });
    };
  }

  return new Condition('to be able to switch to frame', condition);

  function attemptToSwitchFrames(driver, frame) {
    return driver.switchTo().frame(frame).then(
        function() { return true; },
        function(e) {
          if (!(e instanceof error.NoSuchFrameError)) {
            throw e;
          }
        });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.alertIsPresent"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>alertIsPresent ()](#apidoc.element.protractor.until.alertIsPresent)
- description and source-code
```javascript
function alertIsPresent() {
  return new Condition('for alert to be present', function(driver) {
    return driver.switchTo().alert().catch(function(e) {
      if (!(e instanceof error.NoSuchAlertError
        // XXX: Workaround for GeckoDriver error 'TypeError: can't convert null
        // to object'. For more details, see
        // https://github.com/SeleniumHQ/selenium/pull/2137
        || (e instanceof error.WebDriverError
          && e.message === 'can't convert null to object')
        )) {
        throw e;
      }
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.elementIsDisabled"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>elementIsDisabled (element)](#apidoc.element.protractor.until.elementIsDisabled)
- description and source-code
```javascript
function elementIsDisabled(element) {
  return new WebElementCondition('until element is disabled', function() {
    return element.isEnabled().then(v => v ? null : element);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.elementIsEnabled"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>elementIsEnabled (element)](#apidoc.element.protractor.until.elementIsEnabled)
- description and source-code
```javascript
function elementIsEnabled(element) {
  return new WebElementCondition('until element is enabled', function() {
    return element.isEnabled().then(v => v ? element : null);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.elementIsNotSelected"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>elementIsNotSelected (element)](#apidoc.element.protractor.until.elementIsNotSelected)
- description and source-code
```javascript
function elementIsNotSelected(element) {
  return new WebElementCondition('until element is not selected', function() {
    return element.isSelected().then(v => v ? null : element);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.elementIsNotVisible"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>elementIsNotVisible (element)](#apidoc.element.protractor.until.elementIsNotVisible)
- description and source-code
```javascript
function elementIsNotVisible(element) {
  return new WebElementCondition('until element is not visible', function() {
    return element.isDisplayed().then(v => v ? null : element);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.elementIsSelected"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>elementIsSelected (element)](#apidoc.element.protractor.until.elementIsSelected)
- description and source-code
```javascript
function elementIsSelected(element) {
  return new WebElementCondition('until element is selected', function() {
    return element.isSelected().then(v => v ? element : null);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.elementIsVisible"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>elementIsVisible (element)](#apidoc.element.protractor.until.elementIsVisible)
- description and source-code
```javascript
function elementIsVisible(element) {
  return new WebElementCondition('until element is visible', function() {
    return element.isDisplayed().then(v => v ? element : null);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.elementLocated"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>elementLocated (locator)](#apidoc.element.protractor.until.elementLocated)
- description and source-code
```javascript
function elementLocated(locator) {
  locator = by.checkedLocator(locator);
  let locatorStr =
      typeof locator === 'function' ? 'by function()' : locator + '';
  return new WebElementCondition('for element to be located ' + locatorStr,
      function(driver) {
        return driver.findElements(locator).then(function(elements) {
          return elements[0];
        });
      });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.elementTextContains"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>elementTextContains (element, substr)](#apidoc.element.protractor.until.elementTextContains)
- description and source-code
```javascript
function elementTextContains(element, substr) {
  return new WebElementCondition('until element text contains', function() {
    return element.getText()
        .then(t => t.indexOf(substr) != -1 ? element : null);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.elementTextIs"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>elementTextIs (element, text)](#apidoc.element.protractor.until.elementTextIs)
- description and source-code
```javascript
function elementTextIs(element, text) {
  return new WebElementCondition('until element text is', function() {
    return element.getText().then(t => t === text ? element : null);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.elementTextMatches"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>elementTextMatches (element, regex)](#apidoc.element.protractor.until.elementTextMatches)
- description and source-code
```javascript
function elementTextMatches(element, regex) {
  return new WebElementCondition('until element text matches', function() {
    return element.getText().then(t => regex.test(t) ? element : null);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.elementsLocated"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>elementsLocated (locator)](#apidoc.element.protractor.until.elementsLocated)
- description and source-code
```javascript
function elementsLocated(locator) {
  locator = by.checkedLocator(locator);
  let locatorStr =
      typeof locator === 'function' ? 'by function()' : locator + '';
  return new Condition(
      'for at least one element to be located ' + locatorStr,
      function(driver) {
        return driver.findElements(locator).then(function(elements) {
          return elements.length > 0 ? elements : null;
        });
      });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.stalenessOf"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>stalenessOf (element)](#apidoc.element.protractor.until.stalenessOf)
- description and source-code
```javascript
function stalenessOf(element) {
  return new Condition('element to become stale', function() {
    return element.getTagName().then(
        function() { return false; },
        function(e) {
          if (e instanceof error.StaleElementReferenceError) {
            return true;
          }
          throw e;
        });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.titleContains"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>titleContains (substr)](#apidoc.element.protractor.until.titleContains)
- description and source-code
```javascript
function titleContains(substr) {
  return new Condition(
      'for title to contain ' + JSON.stringify(substr),
      function(driver) {
        return driver.getTitle().then(function(title) {
          return title.indexOf(substr) !== -1;
        });
      });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.titleIs"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>titleIs (title)](#apidoc.element.protractor.until.titleIs)
- description and source-code
```javascript
function titleIs(title) {
  return new Condition(
      'for title to be ' + JSON.stringify(title),
      function(driver) {
        return driver.getTitle().then(function(t) {
          return t === title;
        });
      });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.titleMatches"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>titleMatches (regex)](#apidoc.element.protractor.until.titleMatches)
- description and source-code
```javascript
function titleMatches(regex) {
  return new Condition('for title to match ' + regex, function(driver) {
    return driver.getTitle().then(function(title) {
      return regex.test(title);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.urlContains"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>urlContains (substrUrl)](#apidoc.element.protractor.until.urlContains)
- description and source-code
```javascript
function urlContains(substrUrl) {
  return new Condition(
      'for URL to contain ' + JSON.stringify(substrUrl),
      function(driver) {
        return driver.getCurrentUrl().then(function(url) {
          return url.indexOf(substrUrl) !== -1;
        });
      });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.urlIs"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>urlIs (url)](#apidoc.element.protractor.until.urlIs)
- description and source-code
```javascript
function urlIs(url) {
  return new Condition(
      'for URL to be ' + JSON.stringify(url),
      function(driver) {
        return driver.getCurrentUrl().then(function(u) {
          return u === url;
        });
      });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.protractor.until.urlMatches"></a>[function <span class="apidocSignatureSpan">protractor.until.</span>urlMatches (regex)](#apidoc.element.protractor.until.urlMatches)
- description and source-code
```javascript
function urlMatches(regex) {
  return new Condition('for URL to match ' + regex, function(driver) {
    return driver.getCurrentUrl().then(function(url) {
      return regex.test(url);
    });
  });
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
