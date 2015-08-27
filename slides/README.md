# Slides
> reveal.js template stolen from Object Partners' [react-workshop](https://github.com/objectpartners/react-workshop/tree/master/slidedeck)

* [Node](http://nodejs.org/)
* [Gulp](https://github.com/gulpjs/gulp) `npm install -g gulp`
* [Bower](http://twitter.github.com/bower/) `npm install -g bower`

####Getting Started
* Run `npm install` to install node dependencies
* Run `bower install` to install client-side dependencies

####Gulp Commands
`gulp assemble`
  * Minify/uglify the javascript source and css
  * Compiles jade
  * Stages everything in the dist folder

`gulp watch`
  * Starts a server running on port 8001
  * Watches for changes on project files
  * When files change, the assemble task is re-run and
  * Livereload triggers browser update on assemble task completion

`./publish.sh`
  * Publishes slides to GitHub pages
  * Uses git subtree merge to merge the contents of dist into the gh-pages branch
