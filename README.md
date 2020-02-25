# Code@LTH Website
The official Code@LTH website.

It currently lives at [codeatlth.org](http://codeatlth.org/). There is also a shortcut up at [lth.se/code](http://lth.se/code).

## Development
Whenever a new commit is made GitHub automatically updates the site (might take a few minutes).

If you have any issues getting things up and running, contact an existing contributor.

If you want to help develop the site, download and install [Jekyll](jekyllrb.com) which this site uses for static page generation.

### How to get started

 1. Install dependencies
    1. For Ubuntu/Debian: 
        1. `sudo apt-get install ruby ruby-dev make rake build-essential`
    1. For macOS: 
        1. Install homebrew
        1. `brew install ruby`
 1. `gem install bundle` 
 1. Clone this repository
 1. `cd` into the directory
 1. `bundle install`
 1. Run `make dev`
 1. Open up [localhost:4000](http://localhost:4000/) in your webbrowser.

**Note:** Always test your changes locally before pushing.
If you have issues with pages not rendering properly ensure you don't have a 
[BOM](https://en.wikipedia.org/wiki/Byte_order_mark) at the start of the related file. 
An example of a breaking such commit can be found [here](https://github.com/Code-at-LTH/code-at-lth.github.io/commit/350f0b34613464f8596203ce5dfb883fab0ba82f).

#### Current status of issues

[![Stories in Ready](https://badge.waffle.io/Code-at-LTH/code-at-lth.github.io.png?label=ready&title=Ready)](https://waffle.io/Code-at-LTH/code-at-lth.github.io)
[![Stories in Progress](https://badge.waffle.io/Code-at-LTH/code-at-lth.github.io.png?label=in progress&title=In Progress)](https://waffle.io/Code-at-LTH/code-at-lth.github.io)
