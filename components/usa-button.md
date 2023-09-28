![version](https://img.shields.io/badge/version-3.3.0-4287f5.svg?style=flat)

# usa-button

## Packages

[`@forward "usa-button";`](https://github.com/uswds/uswds/tree/v3.3.0/packages/usa-button/)

[`@forward "./internal/nci-outline-secondary";`](https://github.com/NCIOCPL/ncids/blob/develop/packages/ncids-css/packages/usa-button/internal/_nci-outline-secondary.scss)

[`@forward "./internal/nci-small";`](https://github.com/NCIOCPL/ncids/blob/develop/packages/ncids-css/packages/usa-button/internal/_nci-small.scss)

### Mixins
<details>
<summary>click to show</summary>

- [`packages/uswds-core/src/styles/mixins/typography/typeset.scss`](https://github.com/uswds/uswds/tree/v3.3.0/packages/uswds-core/src/styles/mixins/typography/typeset.scss)

  - `typeset`

- [`packages/uswds-core/src/styles/mixins/helpers/border-box-sizing.scss`](https://github.com/uswds/uswds/tree/v3.3.0/packages/uswds-core/src/styles/mixins/helpers/border-box-sizing.scss)

  - `border-box-sizing`

- [`packages/uswds-core/src/styles/mixins/helpers/set-text-and-bg.scss`](https://github.com/uswds/uswds/tree/v3.3.0/packages/uswds-core/src/styles/mixins/helpers/set-text-and-bg.scss)

  - `set-text-and-bg`

- [`packages/uswds-core/src/styles/mixins/helpers/at-media.scss`](https://github.com/uswds/uswds/tree/v3.3.0/packages/uswds-core/src/styles/mixins/helpers/at-media.scss)

  - `at-media`

- [`packages/uswds-core/srec/styles/mixins/utilities/_disabled.scss`](https://github.com/uswds/uswds/tree/v3.3.0/packages/uswds-core/srec/styles/mixins/utilities/_disabled.scss)

  - `u_disabled`

- [`packages/uswds-core/_functionsOLD.scss`](https://github.com/uswds/uswds/tree/v3.3.0/packages/uswds-core/_functionsOLD.scss)

  - `color`
  - `font-weight`
  - `font-size`
  - `get-link-tokens-from-bg`
  - `radius`
  - `units`
  
</details>

## Tokens

```css
$button-context: "Button";
$button-stroke: inset 0 0 0 units($theme-button-stroke-width);

$button-inverse-color: $theme-link-reverse-color;
$button-inverse-hover-color: $theme-link-reverse-hover-color;
$button-inverse-active-color: $theme-link-reverse-active-color;

$theme-button-stroke-width
$theme-button-font-family
$theme-button-border-radius
$border-high-contrast

/* external link variables*/
$theme-internal-domains
$theme-external-link-icon-size 
$theme-external-link-icon-color
```

### Class Names

```css
.usa-button 
.usa-button--active
.usa-button--big
.usa-button--hover
.usa-button--inverse
.usa-button--accent-cool
.usa-button--accent-warm
.usa-button--outline
.usa-button--secondary
.usa-button--nci-small
```
