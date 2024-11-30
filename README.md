# Template: Vite + SCSS + JS

## Description

- the template is more oriented towards building with pure JS, but can be rebuilt on a framework if desired.
- suitable for both single page application and multi-page application

## What's useful?

### Vite setup

- image optimisation
- componentisation with HTML
- auto-update on html changes
- added aliases for convenience

### Styles

#### Organisation of styles

- the necessary files for the styles are placed in the appropriate folders
- global.scss - styles from the previous item are collected into the file. 
- each abstract folder (containing variables, mixins, functions) has a subfolder that contains a generic build file (it is without underscored)
- internal functions that are used only in other functions and utilities are located in abstract/utils

#### Using abilities of SCSS

- variables: screen size, font size, colours, etc.
- mixins:
	- breakpoints (mobile-first prefer) with/without px-to-rem conversion
	- counting average tablet values if you have only for mobile and desktop (works correctly with px)
 - functions:
	- find average value between two units
	- px-to-rem conversion (separately from breakpoints mixins)
	- hex-to-rgb/hex-to-rgba conversion

 More about it you can find in the **<a href="src/styles/.INSTRUCTION.scss">.INSTRUCTION.scss</a>** in the styles folder

#### What about the layout?

- it's have three main components: 
	- header
	- main
	- footer
- parent of these (body) has grid-layout
- all of these three has 100% width of  body. you need to use paddings/margins with containers to get desired result
- styles based on BEM methodology

## Support

If this was helpful to you, please put a star ❤
Thank you!