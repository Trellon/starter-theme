# Starter-Theme

This is a zen subtheme used for starting a new theming project. It includes a Gruntfile that enables libsass, livereload, kss-stylesheets 
and a number of other features to make your theming experience more pleasurable.

The following principles guide the construction of this theme:

1. SMACSS compliant with well organized code
2. Beautiful, attractive tyopgrahy presented in a uniform way
3. Emphasis on horizontal regions spanning the width of the browser
4. Mobile first apporach supported by global breakpoints 
5. The use of global default variables for common theme conditions
6. Solution to applicability issues through selector abstraction

One of the big problems with theming is applicability. There is often a set of styles that can be applied globally, and another 
(much larger) set of styles that need to be applied to very specific selectors in very specific places. This creates situations where 
code reuse goes down, time to compile goes up, and there's an overall loss of velocity around styling a website.

This theme deals with applicability through abstraction. Common theming challenges, such as grids, icons, font styles, blocks, 
menus and other components are defined in layouts and components partials as mixins. Each mixin has variables that define selectors, 
which allows them to be applied to a range of different situations. Instead of organizing styles within layout and component 
partials, these are used to define mixins that are later applied in theme files.

The result is increased effiicency when implementing very complex themes, reduction of effort related to maintaining a theme, and more 
consistent use of styles throughout each website.

# Requirements

* Grunt - installation instructions here: http://gruntjs.com/getting-started#installing-the-cli
* Bower - installation instructions here: http://bower.io/#install-bower

# Instructions for Getting Started

Once Grunt and Bower are installed, set up your theme workflow as follows.

1. Install components with bower

2. Install components with npm

3. Start theming

## Quickstart

    // install all bower components
    bower install
    // install the grunt components
    npm install --save-dev
    grunt --force

# Included components

A number of components are included to make theming easier.

_From Grunt_

1. grunt-sass: libsass, for lightning fast SASS compilation.
2. grunt-contrib-watch: livereload support for viewing changes in your browser without refreshing the page.
3. grunt-kss: creates KSS styleguides.
4. grunt-contrib-copy: for coppying files around in your theme.

_From Bower_

1. Sassy-Buttons: for fancy buttons.
2. compass-mixins: a replacement for Compass that works with libsass.
3. compass-breakpoint: a media query mixin that sometimes works with libsass (we usually find another way).
4. zen-grids: This is Zen Grids 2, used in place of the version that comes with zen.
5. breakpoint-sass: used for creating breakpoints.

