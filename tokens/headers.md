## uswds: do not change

```css
@mixin display {
  @include typeset(
    "heading",
    $theme-display-font-size,
    $theme-heading-line-height
  );

  font-weight: fw("bold");
}

@mixin h1 {
  @include typeset("heading", $theme-h1-font-size, $theme-heading-line-height);
  font-weight: fw("bold");
}
@mixin typeset-display {
  @include typeset-heading;
  @include display;
}

@mixin typeset-h1 {
  @include typeset-heading;
  @include h1;
}
```

## patches or ncids additions:

```css
.nci-heading-display {
  @include typeset-h2 // xl
  @include u-margin-bottom-0
  on tablet-lg { @include display } // 3xl
}
.nci-heading-h1 {
  @include typeset-h2 // xl
  on tablet-lg{ @include h1 } // 2xl
}
.usa-prose > h1 {
  // extends nci-heading-h1
}
.nci-heading--label {
  padding-bottom
  border-bottom
}
```

## Token Updates

```css
$theme-h1-font-size: "2xl" !default;
$theme-h2-font-size: "xl" !default;
$theme-h3-font-size: "lg" !default;
$theme-h4-font-size: "sm" !default;
$theme-h5-font-size: "xs" !default;
$theme-h6-font-size: "3xs" !default;
$theme-heading-line-height: 2 !default;
$theme-small-font-size: "2xs" !default;
$theme-display-font-size: "3xl" !default;
 $theme-type-scale-3xs: 2 !default;
 $theme-type-scale-2xs: 3 !default;
+$theme-type-scale-xs: 5 !default;
+$theme-type-scale-sm: 7 !default;
+$theme-type-scale-md: 8 !default;
 $theme-type-scale-lg: 9 !default;
+$theme-type-scale-xl: 10 !default;
+$theme-type-scale-2xl: 11 !default;
+$theme-type-scale-3xl: 12 !default;
```

## cgdp changes:

```css
.cgdp-title-area {
    @include u-text('center');
    @include u-padding-top(3);

    &__subheading {
        @include u-display('block');
        @include u-font(body, 'md');
        @include u-margin-top(1);

        @include at-media(tablet-lg) {
            @include u-margin-top(1.5);
            @include u-font(body, 'xl');
        }
    }
}
```

### Changes to the above stuff
Only display will be responsive
heading token changes that will need to be updated:

```css
nci-heading-h4 md - normal h4 - 8 /20px
nci-heading-h5 sm - normal h5 - 7 / 18px
nci-heading-h6 xs - normal h6 - 5 / 16px
```