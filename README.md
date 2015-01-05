# tern-snabbt

[tern-snabbt](https://github.com/daniel-lundin/tern-snabbt) is a plugin which adds support for [snabbt.js](https://github.com/daniel-lundin/snabbt.js) to the JavaSript code intelligence system [Tern](http://ternjs.net/).

## Demo

You can see demo in this git project with CodeMirror in [demos/snabbt.html](https://github.com/daniel-lundin/tern-snabbt/blob/master/demos/snabbt.html) :

Here a screenshot with completion with CodeMirror snabbt completion :
 
![CodeMirror & Snabbt](https://github.com/daniel-lundin/tern-snabbt/wiki/images/TernSnabbtsWithCodeMirror.png)
 
## Installation

tern-snabbt works with the NodeJS [Tern Server][tern-server], and within a browser.

The easiest way to install tern-snabbt is to use a recent version of
[npm][npm]. In the directory where you installed the [tern package][tern-npm],
simply run

```
$ npm install tern-snabbt
```

## Configuration

`snabbt` support snabbt.

### With Node.js

In order for Tern to load the tern-snabbt plugin once it is installed, you must
include `snabbt` in the `plugins` section of your tern-config.

Here is a minimal example `.tern-project` configuration file:

```json
{
  "libs":["browser","ecma5"],
  "plugins": {
    "snabbt": {}
  }
}
```
### Eclipse IDE

If you are Eclipse user, you can use this tern plugin with [tern.java](https://github.com/angelozerr/tern.java) please read [here](https://github.com/angelozerr/tern.java/wiki/Tern-&-Snabbt-support) for more informations.

### With WebBrowser (CodeMirror)

See [demos/snabbt.html](https://github.com/daniel-lundin/tern-snabbt/blob/master/demos/snabbt.html)

## Structure

The basic structure of the project is given in the following way:

* `snabbt.js` the tern plugin.
* `demos/` demos with snabbt tern plugin which use CodeMirror.
