![version](https://img.shields.io/badge/ncids-2.3.0-bd0246.svg?style=flat)

# Changes

## Color Changes

#### Theme Palette

### Theme color tokens

| Sass variable                     | USWDS default  |   hex   | NCIDS change  |   hex   |
|:----------------------------------|:---------------|:-------:|:--------------|:-------:|
| $theme-color-base-lightest        | gray-5         | #f0f0f0 |               |         |
| $theme-color-base-lighter         | gray-cool-10   | #dfe1e2 |               |         |
| $theme-color-base-light           | gray-cool-30   | #a9aeb1 |               |         |
| $theme-color-base                 | gray-cool-50   | #71767a |               |         |
| $theme-color-base-dark            | gray-cool-60   | #565c65 |               |         |
| $theme-color-base-darker          | gray-cool-70   | #3d4551 |               |         |
| $theme-color-base-darkest         | gray-90        | #1b1b1b |               |         |
| $theme-color-ink                  | gray-90        | #1b1b1b |               |         |
| $theme-color-primary-lightest     | false          |         |               |         |
| $theme-color-primary-lighter      | blue-10        | #d9e8f6 | cerulean-20   | #99cae4 |
| $theme-color-primary-light        | blue-30        | #73b3e7 | cerulean-40   | #3395ca |
| $theme-color-primary              | blue-60v       | #005ea2 | cerulean-50   | #007bbd |
| $theme-color-primary-vivid        | blue-warm-60v  | #0050d8 | cerulean-50v  | #067cbc |
| $theme-color-primary-dark         | blue-warm-70v  | #1a4480 | cerulean-70   | #004e7a |
| $theme-color-primary-darker       | blue-warm-80v  | #162e51 | cerulean-80   | #003a57 |
| $theme-color-primary-darkest      | false          |         |               |         |
| $theme-color-secondary-lightest   | false          |         |               |         |
| $theme-color-secondary-lighter    | red-cool-10    | #f3e1e4 | teal-10       | #beebee |
| $theme-color-secondary-light      | red-30         | #f2938c | teal-30       | #4bbfc6 |
| $theme-color-secondary            | red-50         | #d83933 | teal-50       | #298085 |
| $theme-color-secondary-vivid      | red-cool-50v   | #e41d3d | teal-50v      | #338084 |
| $theme-color-secondary-dark       | red-60v        | #b50909 | teal-70       | #1e4c4f |
| $theme-color-secondary-darker     | red-70v        | #8b0a03 | teal-80       | #17373a |
| $theme-color-secondary-darkest    | false          |         |               |         |
| $theme-color-accent-warm-lightest | false          |         |               |         |
| $theme-color-accent-warm-lighter  | orange-10      | #f2e4d4 | golden-5      | #fdf2bf |
| $theme-color-accent-warm-light    | orange-20v     | #ffbc78 | golden-10     | #fee685 |
| $theme-color-accent-warm          | orange-30v     | #fa9441 | golden-20     | #face00 |
| $theme-color-accent-warm-dark     | orange-50v     | #c05600 | golden-30     | #ddaa01 |
| $theme-color-accent-warm-darker   | orange-60      | #775540 | golden-40     | #b38c00 |
| $theme-color-accent-warm-darkest  | false          |         |               |         |
| $theme-color-accent-cool-lightest | false          |         |               |         |
| $theme-color-accent-cool-lighter  | blue-cool-5v   | #e1f3f8 | navy-10       | #d7e5f4 |
| $theme-color-accent-cool-light    | blue-cool-20v  | #97d4ea | navy-30       | #92a9c8 |
| $theme-color-accent-cool          | cyan-30v       | #00bde3 | navy-50       | #5478ab |
| $theme-color-accent-cool-dark     | blue-cool-40v  | #28a0cb | navy-70       | #284976 |
| $theme-color-accent-cool-darker   | blue-cool-60v  | #07648d | navy-90       | #06162d |
| $theme-color-accent-cool-darkest  | false          |         |               |         |

### State color tokens

| Sass variable                    | USWDS default  |   hex   | NCIDS change  |   hex   |
|:---------------------------------|:---------------|:-------:|:--------------|:-------:|
| $theme-color-error-lighter       | red-warm-10    | #f4e3db | cranberry-10  | #fde2ea |
| $theme-color-error-light         | red-warm-30v   | #f39268 | cranberry-30v | #f27da2 |
| $theme-color-error               | red-warm-50v   | #d54309 | cranberry-50v | #e41154 |
| $theme-color-error-dark          | red-60v        | #b50909 | cranberry-60v | #b60d43 |
| $theme-color-error-darker        | red-70         | #6f3331 | cranberry-70  | #950b30 |
| $theme-color-warning-lighter     | yellow-5       | #faf3d1 | golden-5      | #fdf2bf |
| $theme-color-warning-light       | yellow-10v     | #fee685 | golden-10v    | #ffe396 |
| $theme-color-warning             | gold-20v       | #ffbe2e | golden-20v    | #ffbe2e |
| $theme-color-warning-dark        | gold-30v       | #e5a000 | golden-30v    | #e5a000 |
| $theme-color-warning-darker      | gold-50v       | #936f38 | golden-50v    | #936f38 |
| $theme-color-success-lighter     | green-cool-5   | #ecf3ec | teal-5        | #dbf2f3 |
| $theme-color-success-light       | green-cool-20v | #70e17  | teal-20v      | #67e4e8 |
| $theme-color-success             | green-cool-40v | #00a91c | teal-40v      | #42979a |
| $theme-color-success-dark        | green-cool-50v | #008817 | teal-50v      | #338084 |
| $theme-color-success-darker      | green-cool-60v | #216e1f | teal-60v      | #206b6f |
| $theme-color-info-lighter        | cyan-5         | #e7f6f8 | cerulean-10   | #d4e7f2 |
| $theme-color-info-light          | cyan-20        | #99deea | cerulean-20   | #99cae4 |
| $theme-color-info                | cyan-30v       | #00bde3 | cerulean-30v  | #51b8f0 |
| $theme-color-info-dark           | cyan-40v       | #009ec1 | cerulean-40v  | #2099df |
| $theme-color-info-darker         | blue-cool-60   | #2e6276 | cerulean-60v  | #01679d |
| $theme-color-disabled-light      | gray-10        | #e6e6e6 |               |         |
| $theme-color-disabled            | gray-20        | #c9c9c9 |               |         |
| $theme-color-disabled-dark       | gray-30        | #adadad |               |         |
| $theme-color-emergency           | red-warm-60v   | #9c3d10 | cranberry-60v | #b60d43 |
| $theme-color-emergency-dark      | red-warm-80    | #332d29 | cranberry-80  | #700824 |
| $theme-link-color                | primary        | #007bbd | cerulean-60v  | #01679d |

## Text Color

### Global color tokens

| Class name                    | USWDS default  |   hex   | NCIDS change  |   hex   |
|:------------------------------|:---------------|:-------:|:--------------|:-------:|
| .text-transparent             | transparent    |         |               |         |
| .text-black                   | black          |         |               |         |
| .text-white                   | white          |         |               |         |

### Basic color tokens

| Class name                    | USWDS default  |   hex   | NCIDS change  |   hex   |
|:------------------------------|:---------------|:-------:|:--------------|:-------:|
| .text-red                     | red-50v        | #e52207 |               |         |
| .text-orange                  | orange-40v     | #e66f0e |               |         |
| .text-gold                    | gold-20v       | #ffbe2e |               |         |
| .text-yellow                  | yellow-10v     | #fee685 |               |         |
| .text-green                   | green-50v      | #538200 |               |         |
| .text-mint                    | mint-30v       | #008659 |               |         |
| .text-cyan                    | cyan-40v       | #009ec1 |               |         |
| .text-blue                    | blue-50v       | #0076d6 |               |         |
| .text-indigo                  | indigo-50      | #676cc8 |               |         |
| .text-violet                  | violet-50      | #8168b3 |               |         |
| .text-magenta                 | magenta-50v    | #d72d79 |               |         |
| .text-teal                    |                |         | teal-50v      | #338084 |
| .text-cerulean                |                |         | cerulean-50v  | #067cbc |
| .text-cranberry               |                |         | cranberry-50v | #e41154 |
| .text-navy                    |                |         | navy-50v      | #4177c3 |
| .text-golden                  |                |         | golden-50v    | #936f38 |

### Grayscale color tokens

| Class name                    | USWDS default  |   hex   | NCIDS change  |   hex   |
|:------------------------------|:---------------|:-------:|:--------------|:-------:|
| .text-gray-5                  | gray-5         | #f0f0f0 |               |         |
| .text-gray-10                 | gray-10        | #e6e6e6 |               |         |
| .text-gray-30                 | gray-30        | #adadad |               |         |
| .text-gray-50                 | gray-50        | #757575 |               |         |
| .text-gray-70                 | gray-70        | #454545 |               |         |
| .text-gray-90                 | gray-90        | #1b1b1b |               |         |

### Theme color tokens

| Class name                    | USWDS default  |   hex   | NCIDS change  |   hex   |
|:------------------------------|:---------------|:-------:|:--------------|:-------:|
| .text-base-lightest           | gray-5         | #f0f0f0 |               |         |
| .text-base-lighter            | gray-cool-10   | #dfe1e2 |               |         |
| .text-base-light              | gray-cool-30   | #a9aeb1 |               |         |
| .text-base                    | gray-cool-50   | #71767a |               |         |
| .text-base-dark               | gray-cool-60   | #565c65 |               |         |
| .text-base-darker             | gray-cool-70   | #3d4551 |               |         |
| .text-base-darkest            | gray-90        | #1b1b1b |               |         |
| .text-ink                     | gray-90        | #1b1b1b |               |         |
| .text-primary-lightest        | false          |         |               |         |
| .text-primary-lighter         | blue-10        | #d9e8f6 | cerulean-20   | #99cae4 |
| .text-primary-light           | blue-30        | #73b3e7 | cerulean-40   | #3395ca |
| .text-primary                 | blue-60v       | #005ea2 | cerulean-50   | #007bbd |
| .text-primary-vivid           | blue-warm-60v  | #0050d8 | cerulean-50v  | #067cbc |
| .text-primary-dark            | blue-warm-70v  | #1a4480 | cerulean-70   | #004e7a |
| .text-primary-darker          | blue-warm-80v  | #162e51 | cerulean-80   | #003a57 |
| .text-primary-darkest         | false          |         |               |         |
| .text-secondary-lightest      | false          |         |               |         |
| .text-secondary-lighter       | red-cool-10    | #f3e1e4 | teal-10       | #beebee |
| .text-secondary-light         | red-30         | #f2938c | teal-30       | #4bbfc6 |
| .text-secondary               | red-50         | #d83933 | teal-50       | #298085 |
| .text-secondary-vivid         | red-cool-50v   | #e41d3d | teal-50v      | #338084 |
| .text-secondary-dark          | red-60v        | #b50909 | teal-70       | #1e4c4f |
| .text-secondary-darker        | red-70v        | #8b0a03 | teal-80       | #17373a |
| .text-secondary-darkest       | false          |         |               |         |
| .text-accent-warm-lightest    | false          |         |               |         |
| .text-accent-warm-lighter     | orange-10      | #f2e4d4 | golden-5      | #fdf2bf |
| .text-accent-warm-light       | orange-20v     | #ffbc78 | golden-10     | #fee685 |
| .text-accent-warm             | orange-30v     | #fa9441 | golden-20     | #face00 |
| .text-accent-warm-dark        | orange-50v     | #c05600 | golden-30     | #ddaa01 |
| .text-accent-warm-darker      | orange-60      | #775540 | golden-40     | #b38c00 |
| .text-accent-warm-darkest     | false          |         |               |         |
| .text-accent-cool-lightest    | false          |         |               |         |
| .text-accent-cool-lighter     | blue-cool-5v   | #e1f3f8 | navy-10       | #d7e5f4 |
| .text-accent-cool-light       | blue-cool-20v  | #97d4ea | navy-30       | #92a9c8 |
| .text-accent-cool             | cyan-30v       | #00bde3 | navy-50       | #5478ab |
| .text-accent-cool-dark        | blue-cool-40v  | #28a0cb | navy-70       | #284976 |
| .text-accent-cool-darker      | blue-cool-60v  | #07648d | navy-90       | #06162d |
| .text-accent-cool-darkest     | false          |         |               |         |

### State color tokens

| Class name                    | USWDS default  |   hex   | NCIDS change  |   hex   |
|:------------------------------|:---------------|:-------:|:--------------|:-------:|
| .text-error-lighter           | red-warm-10    | #f4e3db | cranberry-10  | #fde2ea |
| .text-error-light             | red-warm-30v   | #f39268 | cranberry-30v | #f27da2 |
| .text-error                   | red-warm-50v   | #d54309 | cranberry-50v | #e41154 |
| .text-error-dark              | red-60v        | #b50909 | cranberry-60v | #b60d43 |
| .text-error-darker            | red-70         | #6f3331 | cranberry-70  | #950b30 |
| .text-warning-lighter         | yellow-5       | #faf3d1 | golden-5      | #fdf2bf |
| .text-warning-light           | yellow-10v     | #fee685 | golden-10v    | #ffe396 |
| .text-warning                 | gold-20v       | #ffbe2e | golden-20v    | #ffbe2e |
| .text-warning-dark            | gold-30v       | #e5a000 | golden-30v    | #e5a000 |
| .text-warning-darker          | gold-50v       | #936f38 | golden-50v    | #936f38 |
| .text-success-lighter         | green-cool-5   | #ecf3ec | teal-5        | #dbf2f3 |
| .text-success-light           | green-cool-20v | #70e17  | teal-20v      | #67e4e8 |
| .text-success                 | green-cool-40v | #00a91c | teal-40v      | #42979a |
| .text-success-dark            | green-cool-50v | #008817 | teal-50v      | #338084 |
| .text-success-darker          | green-cool-60v | #216e1f | teal-60v      | #206b6f |
| .text-info-lighter            | cyan-5         | #e7f6f8 | cerulean-10   | #d4e7f2 |
| .text-info-light              | cyan-20        | #99deea | cerulean-20   | #99cae4 |
| .text-info                    | cyan-30v       | #00bde3 | cerulean-30v  | #51b8f0 |
| .text-info-dark               | cyan-40v       | #009ec1 | cerulean-40v  | #2099df |
| .text-info-darker             | blue-cool-60   | #2e6276 | cerulean-60v  | #01679d |
| .text-disabled-light          | gray-10        | #e6e6e6 |               |         |
| .text-disabled                | gray-20        | #c9c9c9 |               |         |
| .text-disabled-dark           | gray-30        | #adadad |               |         |
| .text-emergency               | red-warm-60v   | #9c3d10 | cranberry-60v | #b60d43 |
| .text-emergency-dark          | red-warm-80    | #332d29 | cranberry-80  | #700824 |

## Background Color

### Global color tokens

| Class name                    | USWDS default  |   hex   | NCIDS change  |   hex   |
|:------------------------------|:---------------|:-------:|:--------------|:-------:|
| .bg-transparent               | transparent    |         |               |         |
| .bg-black                     | black          |         |               |         |
| .bg-white                     | white          |         |               |         |

### Basic color tokens

| Class name                    | USWDS default  |   hex   | NCIDS change  |   hex   |
|:------------------------------|:---------------|:-------:|:--------------|:-------:|
| .bg-red                       | red-50v        | #e52207 |               |         |
| .bg-orange                    | orange-40v     | #e66f0e |               |         |
| .bg-gold                      | gold-20v       | #ffbe2e |               |         |
| .bg-yellow                    | yellow-10v     | #fee685 |               |         |
| .bg-green                     | green-50v      | #538200 |               |         |
| .bg-mint                      | mint-30v       | #008659 |               |         |
| .bg-cyan                      | cyan-40v       | #009ec1 |               |         |
| .bg-blue                      | blue-50v       | #0076d6 |               |         |
| .bg-indigo                    | indigo-50      | #676cc8 |               |         |
| .bg-violet                    | violet-50      | #8168b3 |               |         |
| .bg-magenta                   | magenta-50v    | #d72d79 |               |         |
| .bg-teal                      |                |         | teal-50v      | #338084 |
| .bg-cerulean                  |                |         | cerulean-50v  | #067cbc |
| .bg-cranberry                 |                |         | cranberry-50v | #e41154 |
| .bg-navy                      |                |         | navy-50v      | #4177c3 |
| .bg-golden                    |                |         | golden-50v    | #936f38 |

### Grayscale color tokens

| Class name                    | USWDS default  |   hex   | NCIDS change  |   hex   |
|:------------------------------|:---------------|:-------:|:--------------|:-------:|
| .bg-gray-5                    | gray-5         | #f0f0f0 |               |         |
| .bg-gray-10                   | gray-10        | #e6e6e6 |               |         |
| .bg-gray-30                   | gray-30        | #adadad |               |         |
| .bg-gray-50                   | gray-50        | #757575 |               |         |
| .bg-gray-70                   | gray-70        | #454545 |               |         |
| .bg-gray-90                   | gray-90        | #1b1b1b |               |         |

### Theme color tokens

| Class name                    | USWDS default  |   hex   | NCIDS change  |   hex   |
|:------------------------------|:---------------|:-------:|:--------------|:-------:|
| .bg-base-lightest             | gray-5         | #f0f0f0 |               |         |
| .bg-base-lighter              | gray-cool-10   | #dfe1e2 |               |         |
| .bg-base-light                | gray-cool-30   | #a9aeb1 |               |         |
| .bg-base                      | gray-cool-50   | #71767a |               |         |
| .bg-base-dark                 | gray-cool-60   | #565c65 |               |         |
| .bg-base-darker               | gray-cool-70   | #3d4551 |               |         |
| .bg-base-darkest              | gray-90        | #1b1b1b |               |         |
| .bg-ink                       | gray-90        | #1b1b1b |               |         |
| .bg-primary-lightest          | false          |         |               |         |
| .bg-primary-lighter           | blue-10        | #d9e8f6 | cerulean-20   | #99cae4 |
| .bg-primary-light             | blue-30        | #73b3e7 | cerulean-40   | #3395ca |
| .bg-primary                   | blue-60v       | #005ea2 | cerulean-50   | #007bbd |
| .bg-primary-vivid             | blue-warm-60v  | #0050d8 | cerulean-50v  | #067cbc |
| .bg-primary-dark              | blue-warm-70v  | #1a4480 | cerulean-70   | #004e7a |
| .bg-primary-darker            | blue-warm-80v  | #162e51 | cerulean-80   | #003a57 |
| .bg-primary-darkest           | false          |         |               |         |
| .bg-secondary-lightest        | false          |         |               |         |
| .bg-secondary-lighter         | red-cool-10    | #f3e1e4 | teal-10       | #beebee |
| .bg-secondary-light           | red-30         | #f2938c | teal-30       | #4bbfc6 |
| .bg-secondary                 | red-50         | #d83933 | teal-50       | #298085 |
| .bg-secondary-vivid           | red-cool-50v   | #e41d3d | teal-50v      | #338084 |
| .bg-secondary-dark            | red-60v        | #b50909 | teal-70       | #1e4c4f |
| .bg-secondary-darker          | red-70v        | #8b0a03 | teal-80       | #17373a |
| .bg-secondary-darkest         | false          |         |               |         |
| .bg-accent-warm-lightest      | false          |         |               |         |
| .bg-accent-warm-lighter       | orange-10      | #f2e4d4 | golden-5      | #fdf2bf |
| .bg-accent-warm-light         | orange-20v     | #ffbc78 | golden-10     | #fee685 |
| .bg-accent-warm               | orange-30v     | #fa9441 | golden-20     | #face00 |
| .bg-accent-warm-dark          | orange-50v     | #c05600 | golden-30     | #ddaa01 |
| .bg-accent-warm-darker        | orange-60      | #775540 | golden-40     | #b38c00 |
| .bg-accent-warm-darkest       | false          |         |               |         |
| .bg-accent-cool-lightest      | false          |         |               |         |
| .bg-accent-cool-lighter       | blue-cool-5v   | #e1f3f8 | navy-10       | #d7e5f4 |
| .bg-accent-cool-light         | blue-cool-20v  | #97d4ea | navy-30       | #92a9c8 |
| .bg-accent-cool               | cyan-30v       | #00bde3 | navy-50       | #5478ab |
| .bg-accent-cool-dark          | blue-cool-40v  | #28a0cb | navy-70       | #284976 |
| .bg-accent-cool-darker        | blue-cool-60v  | #07648d | navy-90       | #06162d |
| .bg-accent-cool-darkest       | false          |         |               |         |

### State color tokens

| Class name                    | USWDS default  |   hex   | NCIDS change  |   hex   |
|:------------------------------|:---------------|:-------:|:--------------|:-------:|
| .bg-error-lighter             | red-warm-10    | #f4e3db | cranberry-10  | #fde2ea |
| .bg-error-light               | red-warm-30v   | #f39268 | cranberry-30v | #f27da2 |
| .bg-error                     | red-warm-50v   | #d54309 | cranberry-50v | #e41154 |
| .bg-error-dark                | red-60v        | #b50909 | cranberry-60v | #b60d43 |
| .bg-error-darker              | red-70         | #6f3331 | cranberry-70  | #950b30 |
| .bg-warning-lighter           | yellow-5       | #faf3d1 | golden-5      | #fdf2bf |
| .bg-warning-light             | yellow-10v     | #fee685 | golden-10v    | #ffe396 |
| .bg-warning                   | gold-20v       | #ffbe2e | golden-20v    | #ffbe2e |
| .bg-warning-dark              | gold-30v       | #e5a000 | golden-30v    | #e5a000 |
| .bg-warning-darker            | gold-50v       | #936f38 | golden-50v    | #936f38 |
| .bg-success-lighter           | green-cool-5   | #ecf3ec | teal-5        | #dbf2f3 |
| .bg-success-light             | green-cool-20v | #70e17  | teal-20v      | #67e4e8 |
| .bg-success                   | green-cool-40v | #00a91c | teal-40v      | #42979a |
| .bg-success-dark              | green-cool-50v | #008817 | teal-50v      | #338084 |
| .bg-success-darker            | green-cool-60v | #216e1f | teal-60v      | #206b6f |
| .bg-info-lighter              | cyan-5         | #e7f6f8 | cerulean-10   | #d4e7f2 |
| .bg-info-light                | cyan-20        | #99deea | cerulean-20   | #99cae4 |
| .bg-info                      | cyan-30v       | #00bde3 | cerulean-30v  | #51b8f0 |
| .bg-info-dark                 | cyan-40v       | #009ec1 | cerulean-40v  | #2099df |
| .bg-info-darker               | blue-cool-60   | #2e6276 | cerulean-60v  | #01679d |
| .bg-disabled-light            | gray-10        | #e6e6e6 |               |         |
| .bg-disabled                  | gray-20        | #c9c9c9 |               |         |
| .bg-disabled-dark             | gray-30        | #adadad |               |         |
| .bg-emergency                 | red-warm-60v   | #9c3d10 | cranberry-60v | #b60d43 |
| .bg-emergency-dark            | red-warm-80    | #332d29 | cranberry-80  | #700824 |

## Border Color

### Global color tokens

| Class name                   | USWDS default  |   hex   | NCIDS change  |   hex   |
|:-----------------------------|:---------------|:-------:|:--------------|:-------:|
| .border-transparent          | transparent    |         |               |         |
| .border-black                | black          |         |               |         |
| .border-white                | white          |         |               |         |

### Basic color tokens

| Class name                   | USWDS default  |   hex   | NCIDS change  |   hex   |
|:-----------------------------|:---------------|:-------:|:--------------|:-------:|
| .border-red                  | red-50v        | #e52207 |               |         |
| .border-orange               | orange-40v     | #e66f0e |               |         |
| .border-gold                 | gold-20v       | #ffbe2e |               |         |
| .border-yellow               | yellow-10v     | #fee685 |               |         |
| .border-green                | green-50v      | #538200 |               |         |
| .border-mint                 | mint-30v       | #008659 |               |         |
| .border-cyan                 | cyan-40v       | #009ec1 |               |         |
| .border-blue                 | blue-50v       | #0076d6 |               |         |
| .border-indigo               | indigo-50      | #676cc8 |               |         |
| .border-violet               | violet-50      | #8168b3 |               |         |
| .border-magenta              | magenta-50v    | #d72d79 |               |         |
| .border-teal                 |                |         | teal-50v      | #338084 |
| .border-cerulean             |                |         | cerulean-50v  | #067cbc |
| .border-cranberry            |                |         | cranberry-50v | #e41154 |
| .border-navy                 |                |         | navy-50v      | #4177c3 |
| .border-golden               |                |         | golden-50v    | #936f38 |

### Grayscale color tokens

| Class name                   | USWDS default  |   hex   | NCIDS change  |   hex   |
|:-----------------------------|:---------------|:-------:|:--------------|:-------:|
| .border-gray-5               | gray-5         | #f0f0f0 |               |         |
| .border-gray-10              | gray-10        | #e6e6e6 |               |         |
| .border-gray-30              | gray-30        | #adadad |               |         |
| .border-gray-50              | gray-50        | #757575 |               |         |
| .border-gray-70              | gray-70        | #454545 |               |         |
| .border-gray-90              | gray-90        | #1b1b1b |               |         |

### Theme color tokens

| Class name                   | USWDS default  |   hex   | NCIDS change  |   hex   |
|:-----------------------------|:---------------|:-------:|:--------------|:-------:|
| .border-base-lightest        | gray-5         | #f0f0f0 |               |         |
| .border-base-lighter         | gray-cool-10   | #dfe1e2 |               |         |
| .border-base-light           | gray-cool-30   | #a9aeb1 |               |         |
| .border-base                 | gray-cool-50   | #71767a |               |         |
| .border-base-dark            | gray-cool-60   | #565c65 |               |         |
| .border-base-darker          | gray-cool-70   | #3d4551 |               |         |
| .border-base-darkest         | gray-90        | #1b1b1b |               |         |
| .border-ink                  | gray-90        | #1b1b1b |               |         |
| .border-primary-lightest     | false          |         |               |         |
| .border-primary-lighter      | blue-10        | #d9e8f6 | cerulean-20   | #99cae4 |
| .border-primary-light        | blue-30        | #73b3e7 | cerulean-40   | #3395ca |
| .border-primary              | blue-60v       | #005ea2 | cerulean-50   | #007bbd |
| .border-primary-vivid        | blue-warm-60v  | #0050d8 | cerulean-50v  | #067cbc |
| .border-primary-dark         | blue-warm-70v  | #1a4480 | cerulean-70   | #004e7a |
| .border-primary-darker       | blue-warm-80v  | #162e51 | cerulean-80   | #003a57 |
| .border-primary-darkest      | false          |         |               |         |
| .border-secondary-lightest   | false          |         |               |         |
| .border-secondary-lighter    | red-cool-10    | #f3e1e4 | teal-10       | #beebee |
| .border-secondary-light      | red-30         | #f2938c | teal-30       | #4bbfc6 |
| .border-secondary            | red-50         | #d83933 | teal-50       | #298085 |
| .border-secondary-vivid      | red-cool-50v   | #e41d3d | teal-50v      | #338084 |
| .border-secondary-dark       | red-60v        | #b50909 | teal-70       | #1e4c4f |
| .border-secondary-darker     | red-70v        | #8b0a03 | teal-80       | #17373a |
| .border-secondary-darkest    | false          |         |               |         |
| .border-accent-warm-lightest | false          |         |               |         |
| .border-accent-warm-lighter  | orange-10      | #f2e4d4 | golden-5      | #fdf2bf |
| .border-accent-warm-light    | orange-20v     | #ffbc78 | golden-10     | #fee685 |
| .border-accent-warm          | orange-30v     | #fa9441 | golden-20     | #face00 |
| .border-accent-warm-dark     | orange-50v     | #c05600 | golden-30     | #ddaa01 |
| .border-accent-warm-darker   | orange-60      | #775540 | golden-40     | #b38c00 |
| .border-accent-warm-darkest  | false          |         |               |         |
| .border-accent-cool-lightest | false          |         |               |         |
| .border-accent-cool-lighter  | blue-cool-5v   | #e1f3f8 | navy-10       | #d7e5f4 |
| .border-accent-cool-light    | blue-cool-20v  | #97d4ea | navy-30       | #92a9c8 |
| .border-accent-cool          | cyan-30v       | #00bde3 | navy-50       | #5478ab |
| .border-accent-cool-dark     | blue-cool-40v  | #28a0cb | navy-70       | #284976 |
| .border-accent-cool-darker   | blue-cool-60v  | #07648d | navy-90       | #06162d |
| .border-accent-cool-darkest  | false          |         |               |         |

### State color tokens

| Class name                   | USWDS default  |   hex   | NCIDS change  |   hex   |
|:-----------------------------|:---------------|:-------:|:--------------|:-------:|
| .border-error-lighter        | red-warm-10    | #f4e3db | cranberry-10  | #fde2ea |
| .border-error-light          | red-warm-30v   | #f39268 | cranberry-30v | #f27da2 |
| .border-error                | red-warm-50v   | #d54309 | cranberry-50v | #e41154 |
| .border-error-dark           | red-60v        | #b50909 | cranberry-60v | #b60d43 |
| .border-error-darker         | red-70         | #6f3331 | cranberry-70  | #950b30 |
| .border-warning-lighter      | yellow-5       | #faf3d1 | golden-5      | #fdf2bf |
| .border-warning-light        | yellow-10v     | #fee685 | golden-10v    | #ffe396 |
| .border-warning              | gold-20v       | #ffbe2e | golden-20v    | #ffbe2e |
| .border-warning-dark         | gold-30v       | #e5a000 | golden-30v    | #e5a000 |
| .border-warning-darker       | gold-50v       | #936f38 | golden-50v    | #936f38 |
| .border-success-lighter      | green-cool-5   | #ecf3ec | teal-5        | #dbf2f3 |
| .border-success-light        | green-cool-20v | #70e17  | teal-20v      | #67e4e8 |
| .border-success              | green-cool-40v | #00a91c | teal-40v      | #42979a |
| .border-success-dark         | green-cool-50v | #008817 | teal-50v      | #338084 |
| .border-success-darker       | green-cool-60v | #216e1f | teal-60v      | #206b6f |
| .border-info-lighter         | cyan-5         | #e7f6f8 | cerulean-10   | #d4e7f2 |
| .border-info-light           | cyan-20        | #99deea | cerulean-20   | #99cae4 |
| .border-info                 | cyan-30v       | #00bde3 | cerulean-30v  | #51b8f0 |
| .border-info-dark            | cyan-40v       | #009ec1 | cerulean-40v  | #2099df |
| .border-info-darker          | blue-cool-60   | #2e6276 | cerulean-60v  | #01679d |
| .border-disabled-light       | gray-10        | #e6e6e6 |               |         |
| .border-disabled             | gray-20        | #c9c9c9 |               |         |
| .border-disabled-dark        | gray-30        | #adadad |               |         |
| .border-emergency            | red-warm-60v   | #9c3d10 | cranberry-60v | #b60d43 |
| .border-emergency-dark       | red-warm-80    | #332d29 | cranberry-80  | #700824 |

## Outline Color

### Global color tokens

| Class name                   | USWDS default  |   hex   | NCIDS change  |   hex   |
|:-----------------------------|:---------------|:-------:|:--------------|:-------:|
| .outline-transparent         | transparent    |         |               |         |
| .outline-black               | black          |         |               |         |
| .outline-white               | white          |         |               |         |

### Basic color tokens

| Class name                   | USWDS default  |   hex   | NCIDS change  |   hex   |
|:-----------------------------|:---------------|:-------:|:--------------|:-------:|
| .outline-red                 | red-50v        | #e52207 |               |         |
| .outline-orange              | orange-40v     | #e66f0e |               |         |
| .outline-gold                | gold-20v       | #ffbe2e |               |         |
| .outline-yellow              | yellow-10v     | #fee685 |               |         |
| .outline-green               | green-50v      | #538200 |               |         |
| .outline-mint                | mint-30v       | #008659 |               |         |
| .outline-cyan                | cyan-40v       | #009ec1 |               |         |
| .outline-blue                | blue-50v       | #0076d6 |               |         |
| .outline-indigo              | indigo-50      | #676cc8 |               |         |
| .outline-violet              | violet-50      | #8168b3 |               |         |
| .outline-magenta             | magenta-50v    | #d72d79 |               |         |
| .outline-teal                |                |         | teal-50v      | #338084 |
| .outline-cerulean            |                |         | cerulean-50v  | #067cbc |
| .outline-cranberry           |                |         | cranberry-50v | #e41154 |
| .outline-navy                |                |         | navy-50v      | #4177c3 |
| .outline-golden              |                |         | golden-50v    | #936f38 |

### Grayscale color tokens

| Class name                   | USWDS default  |   hex   | NCIDS change  |   hex   |
|:-----------------------------|:---------------|:-------:|:--------------|:-------:|
| .outline-gray-5              | gray-5         | #f0f0f0 |               |         |
| .outline-gray-10             | gray-10        | #e6e6e6 |               |         |
| .outline-gray-30             | gray-30        | #adadad |               |         |
| .outline-gray-50             | gray-50        | #757575 |               |         |
| .outline-gray-70             | gray-70        | #454545 |               |         |
| .outline-gray-90             | gray-90        | #1b1b1b |               |         |

### Theme color tokens

| Class name                    | USWDS default  |   hex   | NCIDS change  |   hex   |
|:------------------------------|:---------------|:-------:|:--------------|:-------:|
| .outline-base-lightest        | gray-5         | #f0f0f0 |               |         |
| .outline-base-lighter         | gray-cool-10   | #dfe1e2 |               |         |
| .outline-base-light           | gray-cool-30   | #a9aeb1 |               |         |
| .outline-base                 | gray-cool-50   | #71767a |               |         |
| .outline-base-dark            | gray-cool-60   | #565c65 |               |         |
| .outline-base-darker          | gray-cool-70   | #3d4551 |               |         |
| .outline-base-darkest         | gray-90        | #1b1b1b |               |         |
| .outline-ink                  | gray-90        | #1b1b1b |               |         |
| .outline-primary-lightest     | false          |         |               |         |
| .outline-primary-lighter      | blue-10        | #d9e8f6 | cerulean-20   | #99cae4 |
| .outline-primary-light        | blue-30        | #73b3e7 | cerulean-40   | #3395ca |
| .outline-primary              | blue-60v       | #005ea2 | cerulean-50   | #007bbd |
| .outline-primary-vivid        | blue-warm-60v  | #0050d8 | cerulean-50v  | #067cbc |
| .outline-primary-dark         | blue-warm-70v  | #1a4480 | cerulean-70   | #004e7a |
| .outline-primary-darker       | blue-warm-80v  | #162e51 | cerulean-80   | #003a57 |
| .outline-primary-darkest      | false          |         |               |         |
| .outline-secondary-lightest   | false          |         |               |         |
| .outline-secondary-lighter    | red-cool-10    | #f3e1e4 | teal-10       | #beebee |
| .outline-secondary-light      | red-30         | #f2938c | teal-30       | #4bbfc6 |
| .outline-secondary            | red-50         | #d83933 | teal-50       | #298085 |
| .outline-secondary-vivid      | red-cool-50v   | #e41d3d | teal-50v      | #338084 |
| .outline-secondary-dark       | red-60v        | #b50909 | teal-70       | #1e4c4f |
| .outline-secondary-darker     | red-70v        | #8b0a03 | teal-80       | #17373a |
| .outline-secondary-darkest    | false          |         |               |         |
| .outline-accent-warm-lightest | false          |         |               |         |
| .outline-accent-warm-lighter  | orange-10      | #f2e4d4 | golden-5      | #fdf2bf |
| .outline-accent-warm-light    | orange-20v     | #ffbc78 | golden-10     | #fee685 |
| .outline-accent-warm          | orange-30v     | #fa9441 | golden-20     | #face00 |
| .outline-accent-warm-dark     | orange-50v     | #c05600 | golden-30     | #ddaa01 |
| .outline-accent-warm-darker   | orange-60      | #775540 | golden-40     | #b38c00 |
| .outline-accent-warm-darkest  | false          |         |               |         |
| .outline-accent-cool-lightest | false          |         |               |         |
| .outline-accent-cool-lighter  | blue-cool-5v   | #e1f3f8 | navy-10       | #d7e5f4 |
| .outline-accent-cool-light    | blue-cool-20v  | #97d4ea | navy-30       | #92a9c8 |
| .outline-accent-cool          | cyan-30v       | #00bde3 | navy-50       | #5478ab |
| .outline-accent-cool-dark     | blue-cool-40v  | #28a0cb | navy-70       | #284976 |
| .outline-accent-cool-darker   | blue-cool-60v  | #07648d | navy-90       | #06162d |
| .outline-accent-cool-darkest  | false          |         |               |         |

### State color tokens

| Class name                    | USWDS default  |   hex   | NCIDS change  |   hex   |
|:------------------------------|:---------------|:-------:|:--------------|:-------:|
| .outline-error-lighter        | red-warm-10    | #f4e3db | cranberry-10  | #fde2ea |
| .outline-error-light          | red-warm-30v   | #f39268 | cranberry-30v | #f27da2 |
| .outline-error                | red-warm-50v   | #d54309 | cranberry-50v | #e41154 |
| .outline-error-dark           | red-60v        | #b50909 | cranberry-60v | #b60d43 |
| .outline-error-darker         | red-70         | #6f3331 | cranberry-70  | #950b30 |
| .outline-warning-lighter      | yellow-5       | #faf3d1 | golden-5      | #fdf2bf |
| .outline-warning-light        | yellow-10v     | #fee685 | golden-10v    | #ffe396 |
| .outline-warning              | gold-20v       | #ffbe2e | golden-20v    | #ffbe2e |
| .outline-warning-dark         | gold-30v       | #e5a000 | golden-30v    | #e5a000 |
| .outline-warning-darker       | gold-50v       | #936f38 | golden-50v    | #936f38 |
| .outline-success-lighter      | green-cool-5   | #ecf3ec | teal-5        | #dbf2f3 |
| .outline-success-light        | green-cool-20v | #70e17  | teal-20v      | #67e4e8 |
| .outline-success              | green-cool-40v | #00a91c | teal-40v      | #42979a |
| .outline-success-dark         | green-cool-50v | #008817 | teal-50v      | #338084 |
| .outline-success-darker       | green-cool-60v | #216e1f | teal-60v      | #206b6f |
| .outline-info-lighter         | cyan-5         | #e7f6f8 | cerulean-10   | #d4e7f2 |
| .outline-info-light           | cyan-20        | #99deea | cerulean-20   | #99cae4 |
| .outline-info                 | cyan-30v       | #00bde3 | cerulean-30v  | #51b8f0 |
| .outline-info-dark            | cyan-40v       | #009ec1 | cerulean-40v  | #2099df |
| .outline-info-darker          | blue-cool-60   | #2e6276 | cerulean-60v  | #01679d |
| .outline-disabled-light       | gray-10        | #e6e6e6 |               |         |
| .outline-disabled             | gray-20        | #c9c9c9 |               |         |
| .outline-disabled-dark        | gray-30        | #adadad |               |         |
| .outline-emergency            | red-warm-60v   | #9c3d10 | cranberry-60v | #b60d43 |
| .outline-emergency-dark       | red-warm-80    | #332d29 | cranberry-80  | #700824 |

## Box shadow

| Class name         | USWDS default                                  | NCIDS change                                   |
|:-------------------|:-----------------------------------------------|:-----------------------------------------------|
| `.box-shadow-none` | `none`                                         |                                                |
| `.box-shadow-1`    | `0 units(1px) units(0.5) 0 rgba(0, 0, 0, 0.1)` | `0 units(1px) units(0.5) 0 rgba(0, 0, 0, 0.3)` |
| `.box-shadow-2`    | `0 units(0.5) units(1) 0 rgba(0, 0, 0, 0.1)`   | `0 units(0.5) units(1) 0 rgba(0, 0, 0, 0.3)`   |
| `.box-shadow-3`    | `0 units(1) units(2) 0 rgba(0, 0, 0, 0.1)`     | `0 units(1) units(2) 0 rgba(0, 0, 0, 0.3)`     |
| `.box-shadow-4`    | `0 units(1.5) units(3) 0 rgba(0, 0, 0, 0.1)`   | `0 units(1.5) units(3) 0 rgba(0, 0, 0, 0.3)`   |
| `.box-shadow-5`    | `0 units(2) units(4) 0 rgba(0, 0, 0, 0.1)`     | `0 units(2) units(4) 0 rgba(0, 0, 0, 0.3)`     |
