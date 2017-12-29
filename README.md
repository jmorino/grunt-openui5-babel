> # DEPRECATED
>
> This plugin has been created to work around [this bug](https://github.com/r-murphy/babel-plugin-transform-modules-ui5/issues/1). This bug has been fixed with version [6.16.1](https://github.com/r-murphy/babel-plugin-transform-modules-ui5/tree/e60d574210b11e7ec99209f8e4e39d876f803032). Then, this Grunt plugin becomes obsolete: consider using [the official grunt-babel plugin](https://github.com/babel/grunt-babel) instead.


# grunt-openui5-babel
> Grunt plugin to transpile UI5 sources with Babel

**_WARNING:_ This is an EXPERIMENTAL Grunt plugin. Use at your own risks!**

Special thanks to:
- [Ryan Murphy](https://github.com/r-murphy) for his work on [babel-plugin-transform-modules-ui5](https://github.com/r-murphy/babel-plugin-transform-modules-ui5)


## Getting Started
This plugin requires Grunt `~0.4.5`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-openui5-babel --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-openui5-babel');
```

## The "openui5_babel" task

### Overview
In your project's Gruntfile, add a section named `openui5_babel` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  openui5_babel: {
    options: {
      // babel-plugin-transform-modules-ui5 options go here.
    },
    your_target: {
      // Target-specific file lists and/or options go here.
    },
  },
});
```

### Options

See [https://github.com/r-murphy/babel-plugin-transform-modules-ui5#options](https://github.com/r-murphy/babel-plugin-transform-modules-ui5#options) for supported options


### Usage Examples

```js
grunt.initConfig({
  openui5_babel: {
    options: {
	  namespacePrefix: 'my.ui5.component'
	},
    files: [{
	  expand : true,
	  cwd : 'src',
	  src : ['**/*.js'],
	  dest : 'dist'
    }],
  },
});
```
> *NOTE*
>
> Put your Babel configuration into your `.babelrc` file.


## Release History

*(nothing yet)*
