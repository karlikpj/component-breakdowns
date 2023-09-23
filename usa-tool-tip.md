# usa-tooltip

## Packages

`@forward "usa-tooltip";`

## Mixins

- `uswds-core/_functionsOLD.scss`
  - color
  - radius
  - size
  - units

## Tokens

| mixin/class                 | selector                                                    |
| :-------------------------- | :---------------------------------------------------------- |
| `internal var`              | `$triangle-size: 5px;`                                      |
| `.usa-tooltip__body, --top` | `background-color: color($theme-tooltip-background-color);` |
|                             | `border-radius: radius($theme-button-border-radius);`       |
|                             | `color: color($theme-tooltip-font-color);`                  |
|                             | `font-size: size("ui", $theme-tooltip-font-size);`          |

### Class Names

- `.usa-tooltip`
- `.usa-tooltip__trigger`
- `.usa-tooltip__body`
- `.usa-tooltip__body--top`
- `.usa-tooltip__body--wrap`
- `.usa-tooltip__body.is-set`
- `.usa-tooltip__body.is-visible`
- `.usa-tooltip__body--bottom`
- `.usa-tooltip__body--left`
- `.usa-tooltip__body--right`
- `.usa-tooltip__body--top`
