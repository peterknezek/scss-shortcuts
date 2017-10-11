# scss-shortcuts
Useful mixins for faster and better front-end work. Just import and go.

## Getting Started
Install the module with:
`npm install scss-shortcuts`

## Usage
Import scss file before referring to mixins. ` @import 'scss-shortcuts';`

## Mixins for extended CSS

### BoxShadow:
Mixin Categoty | Example Include
------------ | -------------
BoxShadow   | `@include box-shadow(0, 2px, 5px, 0, #000000, inset);`
BoxShadow (minimal) | `@include box-shadow(0, 2px, 5px);`
BoxShadow (2shadows) | `@include box-shadow(0, 2px, 5px, 0, #000000, false,(-15px 2px 5px 0 #000000));`
BoxShadow (3shadows)  | `@include box-shadow(0, 2px, 5px, 0, #000000, false,(-15px 2px 5px 0 #000000, -15px 20px 5px 0 #000000));`

### Opacity:
Mixin Categoty | Example Include
------------ | -------------
Opacity     | `@include Opacity(0.5);`

### Linear Gradients:
Mixin Categoty | Example Include
------------ | -------------
Linear Gradients vertical | `@include gradient-vertical(#cccccc, #666666, 0%, 100%)`
Linear Gradients horizontal | `@include gradient-horizontal(#cccccc, #666666, 0%, 100%)`

### Rotate:
Mixin Categoty | Example Include
------------ | -------------
Rotate | `@include rotate(45deg);`

### Retina background:
Mixin Categoty | Example Include
------------ | -------------
Retina background | `@include background-retina(logo-@2.png", 120, 30);`

### Border Radius:
Mixin Categoty | Example Include
------------ | -------------
Border Radius | `@include border-radius(6);`

### Transition:
Mixin Categoty | Example Include
------------ | -------------
Transition | `@include transition(box-shadow ease-in 1s);`
Transition property | `@include transition-property(width);`
Transition function | `@include transition-timing-function(ease-in);`
Transition delay | `@include transition-delay(2s);`

### Input placeholder:
Mixin Categoty | Example Include
------------ | -------------
Input placeholder  | `@input-placeholder(Your name);`


## Responsive breakpoints
Breakpoints are sets by default but you can change variables. Sets for bootstrap.
```
$screen-xs-max: 768px;
$screen-sm-max: 992px;
$screen-md-max: 1200px;
```

Example for maxinum bootstrap col `col-md` you can use => {xs,sm,md}:
```
@include max-col(md) {
    ...
}
```
or up to `col-md` {xs,sm,md}:
```
@include min-col(md) {
    ...
}
```