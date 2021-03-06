 <p align="center"><img width="12.5%" src="src/media/js_gulp_gen_icon.svg"></p>
 <p align="center"><img width="60%" src="src/media/js_gulp_gen_logo.png"></p>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Bash Version](https://img.shields.io/badge/Ver.-0.1.0-brightgreen.svg?style=for-the-badge)](https://github.com/AbdulYahya/js-gulp-gen)
&nbsp;&nbsp;&nbsp;&nbsp;
[![Bash Shell](https://img.shields.io/badge/script-bash-blue.svg?style=for-the-badge)](https://en.wikipedia.org/wiki/Bash_(Unix_shell))
&nbsp;&nbsp;&nbsp;&nbsp;
[![GitHub issues](https://img.shields.io/github/issues/AbdulYahya/js-gulp-gen.svg?style=for-the-badge)](https://github.com/AbdulYahya/js-gulp-gen/issues)
&nbsp;&nbsp;&nbsp;&nbsp;
[![GitHub license](https://img.shields.io/github/license/AbdulYahya/gulp-boilerplate-gen.svg?style=for-the-badge)](https://ayahya.mit-license.org)


## Basic Overview

This bash script takes the headache that is setting up a JS project with npm/gulp/etc..etc.. and automates that process. It keeps you informed on exactly what it is doing when it's doing via terminal messages.

After the script is done generating the boilerplate project, it will run gulp jshint to make sure there are no syntactical errors. Then it will run gulp build --prod to make sure all gulp tasks are working properly. Finally it will run npm test just to verify that karma-jasmine was setup correctly.


## Install

First, clone this repo:

```sh
$ git clone https://github.com/AbdulYahya/gulp-boilerplate-gen.git
```

From your terminal, cd into the directory you just cloned:

> :children_crossing: Path below is just an example an likely doesn't exist, unless of course you cloned into you desktop.

```sh
$ cd ~/Desktop/js-gulp-gen
```

Before generating your project, you will need to decide on whether or not you would like to use a CSS framework.
And if so, which one? You have a few different options to choose from:

> :bell: Note, whatever you decide on generating, your project will be Fully functional (NPM/Gulp/Karma-Jasmine)

> Commands denoted by :construction: are currently not available, but will be in the very near future.

| Generation Commands | Framework | Description |
| :------------- | :------------- | :------------- |
|:construction: `$ ./generate` :construction:| Barebones | No CSS what so ever |        
|`$ ./generate -f bootstrap`| Bootstrap | The latest v4.x release of Bootstrap |
|:construction: `$ ./generate -f materialize` :construction:| Materialize | The latest v0.xx.x release of Materialize |
|`$ ./generate -f tailwind`| Tailwind | The latest v0.x.x release of Tailwind |

----

###### :bangbang: `$ npm test` does not work right off the bat, you have to make the following edit to your package.json.
<br />

Change the default test script:

```sh
...
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
```

With karma's test script command:
```sh
...
  "scripts": {
    "test": "karma start karma.conf.js"
  },
```

Now test it by running:

```sh
npm test
```

## License

[MIT License][Arbitrary case-insensitive reference text]

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

###### Copyright (c) 2018 Abdullah Yahya

[arbitrary case-insensitive reference text]: https://ayahya.mit-license.org
