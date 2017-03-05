# Complete SASS/SCSS Snippets!

Complete SASS/SCSS snippets for Sublime Text 3

## Table of Content
- [Commom(i. e. mixin, function)](#commom)
- [Miscellaneous](#misc)
- [Introspection](#introspection)
- [Selector](#selector)
- [Number](#number)
- [Maps](#maps)
- [List](#list)
- [RGB](#rgb)
- [HSL](#hsl)
- [Others Colors](#others)
- [Opacity](#opacity)
- [Strings](#strings)


## Commom

### [mix] mixin

```scss
// Name ${1:name}
// Desc
// Return
@mixin ${1:name}() {
	@content;
}
```

### [fun] function

```scss
// Name ${1:name}
// Desc
// Return
@function ${1:name}() {
	@warn 'warn me';
	@return false;
}
```

### [inc] include

```scss
@include ${1:mixin}();
```

### [ext] extend

```scss
@extend .${1:elem};
```

### [imp] import

```scss
@import '${1:this}';
```

### Snippets list

- [X] Mixin
- [X] Function
- [X] include
- [X] extend
- [X] import
- [X] each
- [X] if/elseif/else
- [X] for
- [X] while
- [X] variable
- [X] at-root
- [X] debug
- [X] warn
- [X] error
- [X] !default
- [X] variable as map
- [X] variable as list
- [X] SASS/SCSS Functions
	- [X] Miscellaneous
		- [X] if
		- [X] unique-id
	- [X] Introspection
		- [X] feature-exists
		- [X] variable-exists
		- [X] global-variable-exists
		- [X] function-exists
		- [X] mixin-exists
		- [X] inspect
		- [X] type-of
		- [X] unit
		- [X] unitless
		- [X] comparable
		- [X] call
	- [X] Selector 
		- [X] selector-nest
		- [X] selector-append
		- [X] selector-extend
		- [X] selector-replace
		- [X] selector-unify
		- [X] is-superselector
		- [X] simple-selectors
		- [X] selectors-parse
	- [X] Number
		- [X] percentage
		- [X] round
		- [X] ceil
		- [X] floor
		- [X] abs
		- [X] min
		- [X] max
		- [X] random
	- [X] Maps
		- [X] map-has-key
		- [X] map-keys
		- [X] map-values
		- [X] map-get
		- [X] map-merge
		- [X] map-remove
		- [X] keywords
	- [X] List
		- [X] length
		- [X] nth
		- [X] set-nth
		- [X] join
		- [X] append
		- [X] zip
		- [X] index
		- [X] list-separator
	- [X] RGB
		- [X] rgb
		- [X] rgba
		- [X] red
		- [X] green
		- [X] blue
		- [X] mix
	- [X] HSL
		- [X] hsl
		- [X] hsla
		- [X] hue
		- [X] saturation
		- [X] lightness
		- [X] darken
		- [X] lighten
		- [X] adjust-hue
		- [X] saturate
		- [X] desaturate
		- [X] grayscale
		- [X] complement
		- [X] invert
	- [X] Others Colors
		- [X] adjust-color
		- [X] scale-color
		- [X] change-color
		- [X] ie-hex-str
	- [X] Opacity
		- [X] alpha
		- [X] opacify
		- [X] transparentize
	- [X] String
		- [X] unquote
		- [X] quote
		- [X] str-length
		- [X] str-insert
		- [X] str-index
		- [X] str-slice
		- [X] to-upper-case
		- [X] to-lower-case