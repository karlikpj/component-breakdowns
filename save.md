
## Font Weight Tokens

Font weights control the heaviness or lightness of how a font displays. The NCIDS supports 3 different weights.

<FontWeightTable>
	<FontWeightRow
		token="light"
		weight="300"
		variable="theme-font-weight-light"
	/>
	<FontWeightRow
		token="normal"
		weight="400"
		variable="theme-font-weight-normal"
	/>
	<FontWeightRow token="bold" weight="600" variable="theme-font-weight-bold" />
</FontWeightTable>

### Font Weight Utilities

To set the weight of the font.

Set the font weight using the u-text mixin or the font-weight function.

```css
/* Utility Example */
.my-class {
	@include u-text('bold');
}
/* Mixin Example */
.my-class {
	font-weight: font-weight('bold');
}
```

## Line Height Tokens

The line height tokens are used to control the amount of space between lines in a block of text. The output listed below is the "target" size and may vary based on the normalized font.

<LineHeightTable />

### Line Height Utilities

To set the line height for the font.

Set the line height using the u-line-height mixin or the line-height function.

```css
/* Utility Example */
.my-class {
	@include u-line-height('heading', 2);
}
/* Mixin Example */
.my-class {
	line-height: line-height('heading', 2);
}
```

Set the family, size, and line height together using the typeset mixin.

```css
.my-class {
	@include typeset('heading', 'lg', 2);
}
```
