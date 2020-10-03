# Gaudiamus CSS

CSS framework builder using SCSS 

- CSS grid
- utility based
- more than customizable: build your own solution

Check out the 
[guide](https://gaudiamus-css.github.io)
for information on how to use Gaudiamus.

## Quick Start

See [gaudiamus-starter](https://github.com/gaudiamus-css/gaudiamus-starter) for the easiest start.

## Installation

`npm i gaudiamus-css` or `yarn add gaudiamus-css`

[![](https://data.jsdelivr.com/v1/package/npm/gaudiamus-css/badge)](https://www.jsdelivr.com/package/npm/gaudiamus-css)

### Basic usage

```scss
/* main.scss */
@import "../node_modules/gaudiamus-css/scss";
```
Make it yours:
```scss
/* main.scss */

/* Grid */
$columns: 12;
$items: 6;
$breakpoint-map: ("md":768px,"lg":1024px);


/* Spacing & utility generator */
$baseSpacing: 20px;
$spacingUnit: 'rem';
$spacingStep: .25;
$numSpacingUnits: 5;

$shorthand-map: ("t":"top","b":"bottom","r":"right","l":"left","x":(1:"left",2:"right"),"y":(1:"top",2:"bottom"));
$property-map: ("m":"margin","p":"padding");


/* Colors */
$primaryColor: #258cc7;
$accentColor: #21d593;
$successColor: #1f921f;
$warningColor: #c92d2d;
$gray: rgba(0,0,0,.2);
$white: #e8e5e5;
$black: #101010;

$color-class-map:("bg":"background-color","text":"color","b":"border-color");

$color-map:(
  "primary":$primaryColor,
  "accent":$accentColor,
  "success":$successColor,
  "warning":$warningColor,
  "transparent":transparent,
  "gray": $gray,
  "white": $white,
  "black": $black
);
$state-map:("focus","hover","active");


/* Shading & borders */

$depth: 3;
$spread: 4px;

/* Typography */
$fontSize-map:("sm":3, "default":4, "md":5, "lg":7, "xl":9, "xxl":12);


@import "../node_modules/gaudiamus-css/scss";
```
