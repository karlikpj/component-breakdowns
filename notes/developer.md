# Developer Notes

## Naming Conventions

### Block-Element-Modifier
BEM stands for Block, Element, and Modifier. It’s a CSS naming convention for writing cleaner and more readable CSS classes.

USWDS follows ***BEM***, and so do we! We will follow the USWDS naming conventions for CSS with some modifications as listed below.

- To differentiate NCI created items from USWDS the BEM Naming rules will be:
	- BEM ***Block*** - something descriptive and prefixed with nci. Example, *.nci-citations-list*.
	- BEM ***Element*** - this defines something that is used inside of a block and only that block.
		- NCIDS BEM ***Block*** *.nci-citations-list*: then the element name should be <block>__<element-name>. Example, *.nci-citations-list__heading*.
		- USWDS BEM ***Block*** *.usa-footer*: then the element name should be <block>__nci-<element-name>. Example, *.usa-footer__nci-special-area*
 - BEM ***Modifier*** - this is going to modify some existing block, but still use the core styles.
	- NCIDS BEM ***Block*** *.nci-citations-list*: then the modifier name should be <block>--<modifier-name>. For example, *.nci-citations--small*.
	- USWDS BEM ***Block*** *.usa-footer*: then the modifier name should be <block>--nci-<element-name>. For example, *.usa-footer--nci-superfantastic*
		- If our modifier is based on the USWDS modifier, then the name should be <block>--nci-<USWDS-modifier-name>. Example, ***usa-footer--nci-big***. This way we can tell where it came from originally.

#### What is a Block?
Blocks are independent, reusable and usually bigger components of a webpage. They can have modifiers and contain elements.

We can count bigger parts in a webpage like `<header>`, `<nav>`, `<section>`,`<form>`, `<article>`, `<footer>` as block examples.

#### Elements
Elements are children of blocks. An element can only have 1 parent Block, and can’t be used independently outside of that block. These can be items such as a `title`, `button`, `input`, `container`.

#### Modifiers
Modifiers represent different states or styles of classes. They can be used both for blocks or elements. A modifier must be used together with its Block / Element, as additional features. Examples could be `-big`, `-active`,`-mobile`