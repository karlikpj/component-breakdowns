![version](https://img.shields.io/badge/ncids-2.3.0-bd0246.svg?style=flat)

# Settings Variables

### Theme font

```js
  // sans-serif
+ $theme-font-type-sans: "open-sans" !default;
 
  // serif
+ $theme-font-type-serif: "poppins" !default;
```

### Theme font weight

```js
  $theme-font-weight-normal: 400 !default;
  $theme-font-weight-medium: false !default;
  $theme-font-weight-semibold: false !default;
+ $theme-font-weight-bold: 600 !default;
  $theme-font-weight-heavy: false !default;
```

### Theme font body 

```js
  $theme-body-font-family: "body" !default;
+ $theme-body-font-size: "xs" !default;
  $theme-body-line-height: 5 !default;
```

### Text and prose

```js
  $theme-text-measure-narrow: 1 !default;
+ $theme-text-measure: 6 !default;
  $theme-text-measure-wide: 6 !default;
  $theme-prose-font-family: "body" !default;
```

### Lead text

```js
+ $theme-lead-font-family: "body" !default;
  $theme-lead-font-size: "lg" !default;
+ $theme-lead-line-height: 4 !default;
  $theme-lead-measure: 6 !default;
```

### Theme scale

```js
  $theme-type-scale-3xs: 2 !default;
  $theme-type-scale-2xs: 3 !default;
+ $theme-type-scale-xs: 5 !default;
+ $theme-type-scale-sm: 7 !default;
+ $theme-type-scale-md: 8 !default;
  $theme-type-scale-lg: 9 !default;
+ $theme-type-scale-xl: 10 !default;
+ $theme-type-scale-2xl: 11 !default;
+ $theme-type-scale-3xl: 12 !default;
```

### Grid

```js
$theme-grid-container-max-width: "widescreen" !default;
```

### Breakpoints
```js
$theme-utility-breakpoints: (
  "desktop-lg": false,
+ "widescreen": true
) !default;
 ```