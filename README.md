# yui-vs-code-support README

## Features

Provides syntax highlighting for .yui files (see https://github.com/shdwcat/YUI)

![image of YUI syntax highlighting in the vs code text editor](images/highlighting.png)

## Release Notes

### 0.2.0
* yuiscript:
	* adds recognition for ~ as 'host functionality' e.g. anything provided by the system (game objects, runtime functions, etc)
	* adds recognition of |> as infix call (aka hack pipe operator)
	* [ and ] now get the correct syntax for the expression within them

* yui: removes YAML cruft that doesn't apply to YUI
	* yes/no/on/off etc are no longer highlighted as literals
	* ` and % no longer highlight as special language characters
	* scalars with comments after them (e.g. `foo: bar //`) highlight correctly
	* remove scalar highlighting for unsupported data formats like base 60, time stamps, etc

### 0.1.1
* Syntax highlighting should now work correctly inside parens
	* YuiScript is now properly defined as a full syntax instead of just tacking things on top of JavaScript

### 0.1.0

* Adds syntax highlighting support for embedded YuiScript
* Adds special highlighting for the `type: name` of an element, to make a file's structure easier to understand
* Removes highlighting for a few more YAML features that YUI does not support (merging, aliases, explicit mapping keys, etc)

### 0.0.1

Initial release of yui-vs-code-support
