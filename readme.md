# Welcome, Friend!

## What am I?

Yeoman is a robust and opinionated client-side stack, comprised of tools and frameworks that can help developers quickly build beautiful web applications. We take care of providing everything needed to get started without any of the normal headaches associated with a manual setup.

Yeoman is fast, performant and is optimized to work best in modern browsers.

For more information about the project, see [http://yeoman.io](http://yeoman.io).


## Installing

* Clone this repo and `cd` into it
* Run the following command at the terminal:

```shell
./setup/install.sh
```
* Navigate to a new directory and run `yeoman init` to make sure everything is working as expected.


### Trouble-shooting

If for any reason you experience exceptions after the yeoman installation process above, you may find the
following steps resolve these issues:

```
$ cd yeoman/cli
$ sudo npm install -g
# when complete then run..
$ sudo npm link
```

## Running

Here's a small shell script that you can save as `server.sh` which opens and servers the current directory on the port specified:

```shell
port=$1
if [ $#  -ne  1 ]
then
  port=8000
fi

if [ $(uname -s) == "Darwin" ]
then
  open=open
else
  open=xdg-open
fi

$open http://localhost:$port && python -m SimpleHTTPServer $port;
```

For example, run this guy as:

```shell
./server.sh 8000
```


## Documentation

The current documentation for Yeoman can be found [here](http://yeoman.github.com/docs). If you are a new contributor and require access to this repository, feel free to ask.


## Browser Support

Yeoman supports:

* Modern browsers (latest versions of Chrome, Safari, Firefox, Opera and IE10)
* Chrome on Android
* Mobile Safari


## Platform Support

Yeoman 1.0 will support Mac OSX and will attempt to support Linux as well. We will be aiming to bring in support for Windows in a future version of the project.

## Contribute

### Repos

* [Yeoman (CLI, Insights)](http://github.com/yeoman/yeoman)
* [Yeoman I/O Holding Page](http://github.com/yeoman/yeoman.io)
* [Yeoman I/O Site](http://github.com/yeoman/yeoman.io)(site branch)
* [Yeoman Docs](http://github.com/yeoman/docs)

### Style Guide

This project follows the [jQuery Style Guide](http://docs.jquery.com/JQuery_Core_Style_Guidelines) with an exception of two space indentation and multiple var statements. Please ensure any pull requests follow this closely. If you notice existing code which doesn't follow these practices, feel free to shout and we will address this.

## About

Yeoman is an open-source project by [Google](http://google.com) which builds on top of [Grunt](https://github.com/cowboy/grunt) and [node-build-script](http://github.com/h5bp/node-build-script). We utilize a number of useful open-source solutions including:

* Twitter Bootstrap
* Html5 Boilerplate
* Modernizr
* Twitter Bower
* Node
* NPM
* Compass
* socket.io
* coffeescript
* mocha
* jasmine
* PhantomJS

and [more](https://github.com/yeoman/yeoman/wiki/Dependencies)

Version 1 of the project features the combined efforts of:

* [Paul Irish](http://paulirish.com)]
* [Addy Osmani](http://addyosmani.com)
* [Mickael Daniel](http://blog.mklog.fr/)
* [Sindre Sorhus](http://sindresorhus.com/)
* [Eric Bidelman](http://ericbidelman.com)

and other developers. 

We will be aiming to officially release the project in late July, 2012.

