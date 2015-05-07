# Code@LTH Website
The official Code@LTH website.

It currently lives at [code-at-lth.github.io/](http://code-at-lth.github.io/). There is also a shortcut up at [lth.se/code](http://lth.se/code).

This site might live on [code.lth.se](http://code.lth.se) or something similar when it is mature.

## Development
If you want to help develop the site, download and install [Jekyll](jekyllrb.com) which this site uses for static page generation.
The Jekyll docs should describe well how to use it.
Whenever a new commit is made with the project files GitHub automatically updates the site (might take a few minutes).

If you have any issues getting things up and running, contact an existing contributor.

**Note:** Always test your changes locally before pushing.
If you have issues with pages not rendering properly ensure you don't have a 
[BOM](https://en.wikipedia.org/wiki/Byte_order_mark) at the start of the related file. 
An example of a breaking such commit can be found [here](https://github.com/Code-at-LTH/code-at-lth.github.io/commit/350f0b34613464f8596203ce5dfb883fab0ba82f).

### How to get started

**NOTE:** This section is a work in progress.

It will assume you are running on an Debian based system for now (includes Ubuntu, Linux Mint).

#### How to install dependencies on a Debian-based Linux distribution

 1. `sudo apt-get install ruby ruby-dev make rake build-essential`
 1. `sudo gem install jekyll`

#### How to install dependencies on Mac OS X

**TODO**

 1. Install homebrew
 1. Something...

#### How to host the website locally

 1. Clone this repository
 1. `cd` into the directory
 1. Run `jekyll serve --watch`
 1. Open up [localhost:4000](http://localhost:4000/) in your webbrowser.


#### Current status of issues

[![Stories in Ready](https://badge.waffle.io/Code-at-LTH/code-at-lth.github.io.png?label=ready&title=Ready)](https://waffle.io/Code-at-LTH/code-at-lth.github.io)
[![Stories in Progress](https://badge.waffle.io/Code-at-LTH/code-at-lth.github.io.png?label=in progress&title=In Progress)](https://waffle.io/Code-at-LTH/code-at-lth.github.io)
