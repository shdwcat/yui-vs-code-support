# Change Log

All notable changes to the "yui-vs-code-support" extension will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

### 0.2.0
* adds recognition for ~ as the start of an expression
* removes YAML cruft that doesn't apply to YUI
	* yes/no/on/off etc are no longer highlighted as literals
	* ` and % no longer highlight as special language characters
	* [ and ] now get the correct syntax for the expression within them

### 0.1.1
* Syntax highlighting should now work correctly inside parens
	* YuiScript is now properly defined as a full syntax instead of just tacking things on top of JavaScript

### 0.1.0

* Adds syntax highlighting support for embedded YuiScript
* Adds special highlighting for the `type: name` of an element, to make a file's structure easier to understand
* Removes highlighting for a few more YAML features that YUI does not support (merging, aliases, explicit mapping keys, etc)

### 0.0.1

- Initial release