A travel site...



### Running Your Local Server With Gulp

After the installation of all requirements and its dependencies, your local web development environment is ready to run. Setup your initial files with `gulp setup`. This command is only necessary the first time the project is set or if the build folder is deleted.

```bash
$ gulp setup
```

Now run your local server using the `watch` task

```bash
$ gulp watch
```

This task will open the browser window usually with the URL http://localhost:3000/. Any saved changes made to the project files, will reload automatically the browser.

![gulp task demo gif](http://res.cloudinary.com/dt4qeehms/image/upload/v1494619106/boilerplate/gif2.gif)

## Project Structure

The structure presented in this boilerplate is grouped primarily by folder content and file type. Please note that this structure is only meant to serve as a guide, it is by no means prescriptive.

```
.
├── build/                      # Store processed/minified files - your project's deployable output
├── img/                        # Main folder for image files
├── js/                         # Main folder for JS files
│   ├── vendor/                 # Store third part library files (e.g.: jquery, bootstrap)
│   └── main.js                 # Index JS code goes here
├── styles/                     # Main folder for cascade style files
│   ├── modules/                # Store third party modules and initializers (e.g.: normalize, reset)
│   ├── variables/              # Store sass variables files
│   └── main.scss               # Index Sass goes here
├── templates/                  # Main folder for pug template files
├── .bowerrc                    # Change bower library destination path from its default
├── gulpfile.js                 # Setup Gulp tasks
└── index.pug                   # Index pug markup goes here
```

### The build/ Contents

```
.
├── build/
    ├── img/                    # Contains the compressed and optimized image files
    ├── css/                    # Contains the concatenated/minified .css files and .map files
    ├── js/                     # Contains the concatenated/minified/uglyfied .js files and .map files
    │   └── vendor/             # Store third party libraries
    └── index.html              # Minified html index file
```

## The Gulp plugins

* [Autoprefixer](https://github.com/postcss/autoprefixer) : Write CSS rules without vendor prefixes.
* [beeper](https://github.com/sindresorhus/beeper) : Beeps when an error happens.
* [BrowserSync](https://github.com/browsersync/browser-sync) : Keep multiple browsers in sync after file save.
* [cache](https://github.com/jgable/gulp-cache) : Keeps an in-memory cache of files images so only changed images are compressed with Imagemin plugin.
* [clean-css](https://github.com/jakubpawlowicz/clean-css) : CSS optimizer and minifier.
* [concat](https://github.com/contra/gulp-concat) : Concatenates `.js` files into `bundle.js`.
* [imagemin](https://github.com/sindresorhus/gulp-imagemin) : Minify PNG, JPEG, GIF and SVG images.
* [notify](https://github.com/mikaelbr/gulp-notify) : Send error messages to Mac Notification Center, Linux notifications or Windows >= 8.
* [plumber](https://github.com/floatdrop/gulp-plumber) : Prevent pipe breaking caused by errors from gulp plugins.
* [Pug](https://github.com/pugjs/gulp-pug) : Compile your Pug templates into HTML.
* [rename](https://github.com/hparra/gulp-rename) : Rename minified files adding `.min` suffix.
* [SASS](https://github.com/dlmanning/gulp-sass) : Compile your SASS or SCSS into CSS.
* [sourcemaps](https://github.com/floridoo/gulp-sourcemaps) : Create CSS and JavaScript map files to debug the code within compressed files.
* [uglify](https://github.com/terinjokes/gulp-uglify) : Minify JavaScript files.
* [gutil](https://github.com/gulpjs/gulp-util) : Log the error message with red highlighting for easier reading.
