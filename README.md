[Assemble]:                http://assemblecss.com
[Assemble Core]:           https://github.com/lukelarsen/assemble-core

# Assemble Code
Assemble Icons is a component of the [Assemble] CSS Framework. It will give you a solid base for using svg icons in your project. It has some default styles that can easily be overridden so you can add your own look.

## Requirements
Assemble Tables requires [Assemble Core].

## Installation
npm install assemble-icons --save-dev

## Usage
### Gulp
```js
var gulp = require('gulp');
var postcss = require('gulp-postcss');
var assembleCore = require('assemble-core');
var assembleIcons = require('assemble-icons');

gulp.task('css', function () {
    var processors = [
        assembleCore,
        assembleIcons
    ];
    return gulp.src('./src/*.css')
        .pipe(postcss(processors))
        .pipe(gulp.dest('./dest'));
});
```

## Options
Options are set with variables. These variables are already set with their default values so they will just work out of the box. If you wish to change them just define the variable you want to change before you load the _assemble-icons.css file. You may wish you see [Assemble Core] for more examples and directions for setting up a Assemble project.

### Design Variables

##### $icon-default-size
- Default: 0.8em;
- Type: Number
```css
$icon-default-size: 20px;
```

##### $icon-default-color
- Default: #000;
- Type: Color
```css
$icon-default-color: #FFF;
```

##### $icon-header-vertical-align
- Default: -0.05em;
- Type: Number
```css
$icon-header-vertical-align: -1px;
```

##### $icon-close-notification-size
- Default: 1em;
- Type: Number
```css
$icon-close-notification-size: 5px;
```
