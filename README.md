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

The recommended way of using Gaudiamus is downloading it via the npm repository:

`npm i gaudiamus-css` or `yarn add gaudiamus-css`

It's also possible to do it from a CDN. However, this way does not provide all the Gaudiamus benefits neither enable its "build-your-own" CSS behavior/framework goal.

[![](https://data.jsdelivr.com/v1/package/npm/gaudiamus-css/badge)](https://www.jsdelivr.com/package/npm/gaudiamus-css)

### Basic usage

```scss
/* main.scss */
$primaryColor: #16ca24;

@import "../node_modules/gaudiamus-css/scss";
```
Make it yours - all variables:
```scss
/* main.scss */

/* Grid */
$grid-container-prefix: 'grid';
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
$position-map:("relative","absolute","fixed");

$height-width-unit-map:("p":"%");
$height-width-value-map:("25", "50", "75", "100");



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

/*
*  lighten/darken
*/

$lighten-map:(
        "light": 25%,
        "lighter": 50%,

);

$darken-map:(
        "dark": 25%,
        "darker": 50%,
);

/*
* Opacity
*/
$opacity-map: ("50":.5,"75":.75,"85":.85,"90":.9,"95":.95);

/*
* State
*/

$state-map:("focus","hover","active");


/* Shading & borders */

$depth: 3;
$spread: 4px;

$border-key: "b";
$rounded-key: "rounded";
$raise-key: "raise";



/* Typography */

$fontSize-map:(
        "sm":3,
        "default":4,
        "md":5,
        "lg":7,
        "xl":9,
        "xxl":12
);
$decoration-map:("underline","none");
$weight-map:("light":200,"strong":700);


@import "../node_modules/gaudiamus-css/scss";
```
