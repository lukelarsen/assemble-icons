[Assemble]:                http://assemblecss.com
[Assemble Base]:           https://github.com/lukelarsen/assemble-base
[useiconic.com]:           https://useiconic.com/open

# Assemble Icons
Assemble Icons is a component of the [Assemble] CSS Framework. It will give you a solid base for using svg icons in your project. It has some default styles that can easily be overridden so you can add your own look.

## Requirements
- Assemble Icons requires [Assemble Base].
- The iconic.js found over at [useiconic.com].

## Installation
npm install assemble-icons --save-dev

## Usage
Import the _assemble-icons.css file from your css file.
```css
@import '../node_modules/assemble-base/base';

/*
Override variables here before the Assemble Components are loaded.
*/

@import '../node_modules/assemble-icons/assemble-icons';
```

### HTML
```html
<img class="iconic" data-src="../images/lock.svg">
```
The img tag will be converted to
```html
<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:sketch="http://www.bohemiancoding.com/sketch/ns" width="12px" height="16px" viewBox="0 0 12 16" version="1.1" class="injected-svg iconic" data-src="../images/lock.svg">
    <!-- Generator: Sketch 3.3.3 (12072) - http://www.bohemiancoding.com/sketch -->
    <title>lock - FontAwesome</title>
    <desc>Created with Sketch.</desc>
    <defs></defs>
    <g id="Page-1" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd" type="MSPage">
        <path d="M3.33333333,7.23809524 L8.66666667,7.23809524 L8.66666667,5.23809524 C8.66666667,4.50198045 8.4062526,3.87351451 7.88541667,3.35267857 C7.36458073,2.83184263 6.73611479,2.57142857 6,2.57142857 C5.26388521,2.57142857 4.63541927,2.83184263 4.11458333,3.35267857 C3.5937474,3.87351451 3.33333333,4.50198045 3.33333333,5.23809524 L3.33333333,7.23809524 Z M12,8.23809524 L12,14.2380952 C12,14.5158744 11.9027787,14.7519832 11.7083333,14.9464286 C11.5138879,15.140874 11.2777792,15.2380952 11,15.2380952 L1,15.2380952 C0.722220833,15.2380952 0.486112083,15.140874 0.291666667,14.9464286 C0.09722125,14.7519832 0,14.5158744 0,14.2380952 L0,8.23809524 C0,7.96031607 0.09722125,7.72420732 0.291666667,7.5297619 C0.486112083,7.33531649 0.722220833,7.23809524 1,7.23809524 L1.33333333,7.23809524 L1.33333333,5.23809524 C1.33333333,3.96031107 1.79166208,2.86309982 2.70833333,1.94642857 C3.62500458,1.02975732 4.72221583,0.571428571 6,0.571428571 C7.27778417,0.571428571 8.37499542,1.02975732 9.29166667,1.94642857 C10.2083379,2.86309982 10.6666667,3.96031107 10.6666667,5.23809524 L10.6666667,7.23809524 L11,7.23809524 C11.2777792,7.23809524 11.5138879,7.33531649 11.7083333,7.5297619 C11.9027787,7.72420732 12,7.96031607 12,8.23809524 L12,8.23809524 Z" id="lock---FontAwesome" fill="#000000" type="MSShapeGroup"></path>
    </g>
</svg>
```
This will put the svg code right in the html so the browser doens't have to fetch another file.

## Options
Options are set with variables. These variables are already set with their default values so they will just work out of the box. If you wish to change them just define the variable you want to change before you load the _assemble-icons.css file. You may wish you see [Assemble Base] for more examples and directions for setting up a Assemble project.

### Design Variables

##### $icon-default-size
- Default icon size. Be sure to use em so the icon can scale to the size it needs.
- Default: 0.8em;
- Type: Number
```css
$icon-default-size: 1em;
```

##### $icon-default-color
- Default icon color.
- Default: #000;
- Type: Color
```css
$icon-default-color: #FFF;
```

##### $icon-header-vertical-align
- When an icon is used in a h1 - h6 set the vertical alignment.
- Default: -0.05em;
- Type: Number
```css
$icon-header-vertical-align: -1px;
```

##### $icon-close-notification-size
- Set the size of the close icon. Be sure to use em so the icon can scale to the size it needs.
- Default: 1em;
- Type: Number
```css
$icon-close-notification-size: 0.5em;
```
