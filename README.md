# Complete SASS/SCSS Snippets!

Complete SASS/SCSS snippets for Sublime Text 3

## Table of Content
- [Short-list of supported functions/etc](supported.md)
- Doc
	- [Commom(mixin, function)](#commom)
	- [Miscellaneous](#miscellaneous)
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
- [Contributing](#contributing)
- [License](#license)

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

### [ea] each

```scss
@each ${1:key}, ${2:var} in $map[item1, item2, item3...] {
	.#{$key} {

	}
}
```

### [for] for

```scss
@for ${1:i} from 1 through 3 {
	.item-#{$i} {
	
	}
}
```

### [ife] if/elseif/else

```scss
@if something == true {

} @else if 0 < 1 {

} @else {

}
```

### [if] if

```scss
if(${1:condition}, $if-true, $if-false) {
	
}
```

### [wh] while

```scss
@while ${1:i} > 0 {
	.item-#{$i} {

	}
}
```

### [wr] warn

```scss
@warn 'warning must be inside of function, do not forget this';
```

### [er] error

```scss
@error 'fatal error';
```

### [de] debug

```scss
@debug ${1:debug};
```

### [$] variable

```scss
${1:var}: ${2:val};
```

### [mp] variable as map

```scss
${1:map}: (
	item1: 0
);
```

### [lt] variable as list

```scss
${1:map}: list1 list2 list3;
```

### [vd] variable as default

```scss
${1:var}: ${2:val} !default;
```

### [at] at-root

```scss
@at-root {
	 ${1:class} {  }
	 ${2:class2} {  }
}
```

-----------------

## Miscellaneous

### [i] if

```scss
@if(${1:condition}, $if-true, $if-false)
```

### [ui] unique-id

```scss
unique-id()
```

-----------------

## Introspection

### [fe] feature-exists

```scss
feature-exists(${1:feature})
```

### [ve] variable-exists

```scss
variable-exists(${1:variable})
```

### [ge] global-variable-exists

```scss
global-variable-exists(${1:variable})
```

### [fne] function-exists

```scss
function-exists(${1:function})
```

### [me] mixin-exists

```scss
mixin-exists(${1:mixin})
```

### [ins] inspect

```scss
inspect(${1:value})
```

### [ty] type-of

```scss
type-of(${1:value})
```

### [un] unit

```scss
unit(${1:number})
```

### [unl] unitless

```scss
unitless(${1:number})
```

### [cp] comparable

```scss
comparable(${1:number1}, ${2:number2})
```

### [ca] call

```scss
call(${1:name}, ${2:args})
```

-----------------

## Selector

### [sn] selector-nest

```scss
selector-nest(${1:selectors})
```

### [sa] selector-append

```scss
selector-append(${1:selectors})
```

### [se] selector-extend

```scss
selector-extend(${1:selector}, ${2:extendee}, ${3:extender})
```

### [sp] selector-parse 

```scss
selector-parse(${1:selector})
```

### [sr] selector-replace 

```scss
selector-replace(${1:selector}, ${2:original}, ${3:replacement})
```

### [su] selector-unify 

```scss
selector-unify(${1:selector1}, ${2:selector2})
```

### [is] is-superselector 

```scss
is-superselector(${1:super}, ${2:sub})
```

### [ss] simple-selectors 

```scss
simple-selectors(${1:selector})
```

-----------------

## Number

### [pr] percentage 

```scss
percentage(${1:number})
```

### [ro] round 

```scss
round(${1:number})
```

### [ce] ceil 

```scss
ceil(${1:number})
```

### [fl] floor 

```scss
floor(${1:number})
```

### [ab] abs 

```scss
abs(${1:number})
```

### [mi] min 

```scss
min(${1:number})
```

### [ma] max 

```scss
max(${1:number})
```

### [rd] random 

```scss
random(${1:limit})
```

----------------

## Maps

### [mk] map-has-key 

```scss
map-has-key(${1:map}, ${2:key})
```

### [mk] map-keys 

```scss
map-keys(${1:map})
```

### [mv] map-values 

```scss
map-values(${1:map})
```

### [mg] map-get 

```scss
map-get(${1:map}, ${2:key})
```

### [mmg] map-merge 

```scss
map-merge(${1:map1}, ${2:map2})
```

### [mr] map-remove 

```scss
map-remove(${1:map}, ${1:keys})
```

### [key] keywords 

```scss
keywords(${1:args})
```

-----------------

## List

### [ln] length 

```scss
length(${1:list})
```

### [nth] nth 

```scss
nth(${1:list}, ${2:n})
```

### [stn] set-nth 

```scss
set-nth(${1:list}, ${2:n}, ${3:value})
```

### [jo] join 

```scss
join(${1:list}, ${2:list2}, ${3:separator})
```

### [ap] append 

```scss
append(${1:list}, ${2:val}, ${3:separator})
```

### [zip] zip 

```scss
zip(${1:lists})
```

### [in] index 

```scss
index(${1:list}, ${2:val})
```

### [ls] list-separator

```scss
list-separator(${1:separator})
```

-----------------

## RGB

### [rgb] rgb 

```scss
rgb(${1:red}, ${2:green}, ${3:blue})
```

### [rgba] rgba 

```scss
rgba(${1:red}, ${2:green}, ${3:blue}, ${4:alpha})
```

### [red] red 

```scss
red(${1:color})
```

### [gr] green 

```scss
green(${1:color})
```

### [bl] blue 

```scss
blue(${1:color})
```

### [mix] mix 

```scss
mix(${1:color}, ${2:color2}, ${3:weight})
```

-----------------

## HSL

### [hsl] hsl 

```scss
hsl(${1:hue}, ${2:saturation}, ${3:lightness})
```

### [hsla] hsla 

```scss
hsla(${1:hue}, ${2:saturation}, ${3:lightness}, ${4:alpha})
```

### [hue] hue 

```scss
hue(${1:color})
```

### [st] saturation 

```scss
saturation(${1:color})
```

### [lgt] lightness 

```scss
lightness(${1:color})
```

### [dk] darken 

```scss
darken(${1:color}, ${2:amount})
```

### [lg] lighten 

```scss
lighten(${1:color}, ${2:amount})
```

### [ah] adjust-hue

```scss
adjust-hue(${1:color}, ${2:degrees})
```

### [ste] saturate

```scss
saturate(${1:color}, ${2:amount})
```

### [dst] desaturate 

```scss
desaturate(${1:color}, ${2:amount})
```

### [grs] grayscale 

```scss
grayscale(${1:color})
```

### [cpm] complement 

```scss
complement(${1:color})
```

### [iv] invert

```scss
invert(${1:color})
```

-----------------

## Others

### [ac] adjust-color 

```scss
adjust-color(${1:color}, [$red], [$green], [$blue], [$hue], [$saturation], [$lightness], [$alpha])
```

### [sc] scale-color 

```scss
scale-color(${1:color}, [$red], [$green], [$blue], [$saturation], [$lightness], [$alpha])
```

### [cc] change-color 

```scss
change-color(${1:color}, [$red], [$green], [$blue], [$hue], [$saturation], [$lightness], [$alpha])
```

### [ih] ie-hex-str

```scss
ie-hex-str(${1:color})
```

-----------------

## Opacity

### [al] alpha

```scss
alpha(${1:color})
```

### [op] opacify

```scss
opacify(${1:color}, ${2:amount})
```

### [tr] transparentize

```scss
transparentize(${1:color}, ${2:amount})
```

-----------------

## Strings

### [uq] unquote

```scss
unquote(${1:string})
```

### [qt] quote

```scss
quote(${1:string})
```

### [stl] str-length

```scss
str-length(${1:string})
```

### [sti] str-insert

```scss
str-insert(${1:string}, ${2:insert}, ${3:index})
```

### [stx] str-index

```scss
str-index(${1:string}, ${2:substring})
```

### [sts] str-slice

```scss
str-slice(${1:string}, ${2:start}, ${3:end})
```

### [tu] to-upper-case

```scss
to-upper-case(${1:string})
```

### [tl] to-lower-case

```scss
to-lower-case(${1:string})
```

-----------------

## Contributing

1. Fork
2. Create your own branch `git checkout -b new-snippet`
3. Add and commit `git add -A && commit -m 'add new-snippet'`
4. Push `git push origin new-feature`
5. Submit a [Pull Request](https://github.com/mhernandes/sublime-scss-snippets/pulls)

-----------------

## License

[MIT license](LICENSE.md)