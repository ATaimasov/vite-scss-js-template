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

- the necessary files for the styles are organised in the appropriate folders
- Each abstract folder subfolder has a common build file (it is without underscore)
- global.scss - styles from the previous item are collected into the file. 

it's global styles. you just need it to import into each style file with these: 
`@use '@styles/global' as *;`

- you can import mixins, variables, etc into components also locally

#### Using abilities of SCSS

- variables: screen size, font size, colours, etc.
- mixins:
	- breakpoint (mobile-first prefer)  with/without px-to-rem convertation (you also can use px-to-rem function separately if you want)
	- counting average tablet values if you have only for mobile and desktop (works correctly with px)
 
 About how to use mixins you can find in the instruction.scss in the styles folder

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