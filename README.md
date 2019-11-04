# Quantum — A Front End Starter Kit
Quantum is a Bootstrapped, Gulp-powered, Sassified, front end boilerplate with Browsersync, hot reloading, Slick carousel, and the Bourbon Sass library. All built on top of Handlebars.js for easy HTML templating.

### Baked-in Features

* Bootstrap 4
* Gulp 4
* Sass
* Bourbon
* Handlebars HTML templating
* Slick Carousel
* Compilation
* Autoprefixing
* Sourcemaps
* Concatenation
* Minification
* Linting
* Accessibility reports
* Browsersync w/ hot reloading
* Mobile first

Changes should be commited to `src/` files only!

### How to use

Primary Gulp tasks to run are:
`gulp dev` for general development
`gulp prod` for production builds (compiles, minifies, concatenates everything etc.)

There is also:
`gulp linters` to run all linting tasks for HTML, SCSS, and JS
`gulp accessibility` to run accessibility tasks that creates an accessibility report .txt file in a folder called `reports`

### Details

Quantum is a small starter kit that's built with Sass and Gulp build systems that have the following features:

-	Handlebars HTML templates with Panini– Panini is a super simple flat file generator for use with Gulp. It compiles a series of HTML pages using a common layout. These pages can also include HTML partials, external Handlebars helpers, or external data as JSON.
-	Sass compilation, prefixing with Autoprefixer, and JavaScript concatenation
-	Built-in BrowserSync server - Will automatically reload your page when files are changed. It also live-injects CSS changes when you save a Sass file. This task runs continuously. Defaults to localhost.
-	For production builds - CSS compression, JavaScript compression, Image compression and more..

### Requirements

To use Quantum, you'll need:

-	Node.js | Test: run ` node -v ` in the terminal
-	npm | (Node comes with npm installed). Test: run ` npm -v`  in the terminal
-	Gulp | `npm install -g gulp`

### Installing:

- Clone this repo: `git clone https://github.com/dmoncado/quantum`
- Navigate into the repo directory: `cd quantum`
- Install all node packages: `npm install` or `sudo npm install`
- Run `gulp dev`
- Your site is now viewable at: http://localhost:3000
- Build something great!

NOTE:
- To create compressed, concatenated, production-ready assets, run `gulp prod`. This will delete everything in the `dist` folder and recreate all of your complied files instantly. Never make updates directly into the dist folder as these files get overridden each time. Also, The dist folder is not kept in source control.

### Folder Structure:

- `dist/` - compiled files (minified and concatenated only with `gulp prod`)
- `node_modules` - front-end dependencies (.gitignore'd)
- `src/` - contains all of your core, working files—static assets, pages, templates, etc.
- `src/assets/` - scss files, JS files, images, and fonts
- `src/layouts/` - HTML layouts templates
- `src/pages/` - site pages
- `src/partials/` - handlebars partials files.
- `gulpfile.js` - all task definitions
- `package.json` - handles the front-end dependencies
- `.htmllintrc` - handles the HTML lint rules
- `.sass-lint.yml` - handles the SCSS lint rules
- `reports` - txt generated file for accessibility issues
