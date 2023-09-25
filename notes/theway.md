# The Way

This page covers our naming conventions and processes. It is the central place to hold information that is vital to working on the NCI Design System.

<details>
<summary><h2>Definitions</h2></summary>
This is for any words we are going to use that are loaded, or things that allow us to discuss items using less words.

- **Variant** - a different visual display of a component, such as a big, medium and slim footer. A more technical description is that this is a BEM Block class, as well as the BEM Modifications of that BEM Block class.

***For example***, the footer `.usa-footer` has 3 variants: 
- Big (modification) `.usa-footer--big`
- Medium (block) `.usa-footer`
- Slim (modification) `.usa-footer--slim`
</details>

<details>
<summary><h2>CSS</h2></summary>

### Naming Standards

#### Block-Element-Modifier
BEM stands for Block, Element, and Modifier. It’s a CSS naming convention for writing cleaner and more readable CSS classes.

USWDS follows ***BEM***, and so do we! 

We will follow the USWDS naming conventions for CSS with some modifications as listed below.

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

<details>
<summary><h3>NCIDS-CSS Coding Rules</h3></summary>

#### Using the USWDS Utilities
The USWDS is not just a collection of components, but also the tools to create components. Many of these utilities actually perform calculations to ensure items look proportionally correct. Whenever provided, we *must* use the USWDS utility mixins, functions, and tokens. These are documented between [Design tokens](https://designsystem.digital.gov/design-tokens/) and [Utilities](https://designsystem.digital.gov/utilities/). NOTE: For Cgov-Digital-Platform we will not be using the utility classes (200k) except for the grid-* classes.

#### Rules for Overriding USWDS
This is a loose decision tree based on some recent experiences. This will dictate how much CSS you need to write and test. Our goal is to use the OOB features of USWDS as much as possible and minimize the amount of code we will have to `diff` when there are updates to USWDS. Additionally a lot of these utilities were created to make the system as usable as possible. (e.g. static css, sass with node-sass, sass with webpack, etc) Our NCIDS must work with a multitude of build tools and systems as well without breaking.

1. Will a setting from `uswds/dist/scss/settings` make the change you desire? If so, just add it to our settings override.
   * This is usually used for colors, fonts and some spacing.
2. Can you take the basic USWDS and just add a couple of css overrides to the base in order to get what we want?
   * Limit this to no more than 2 or 3. If there is a lot of nesting and mixins, then do not use this approach.
3. Can you just create some new BEM elements to go in the USA block? 
   * IDK if I have a good example yet.
4. Do you need to create a variant? Is this very different from the base, or does it behave totally differently?
   * For example our Header has mobile bits that open to the left, instead of right. The search bar is in a different place. It really is a variant.
5. Do you need to recreate the entire block?
   * This should always be a last resort

Additional things to keep in mind
1. When using `family()` what is the best type/role for this font. `sans`, `mono` and `serif` are usually NOT the best choice.
2. use `place-icon` to add icons in CSS
3. Use other utility functions that we have not figured out yet.
4. **If your CSS or JS adds English text to the dom, you need to support Spanish text as well.**

#### File Rules for Component SASS Partials
The USWDS is not granular about how it handles SASS partials for components and variants. For example, the cards package exports ALL the card types. If you want just a flag card, you get all the other CSS for the other cards. Same with headers and footers. Hopefully in future version this will change. However, we are going to approach it from the desired state so that we do not have to do a lot of reword when it is modularized.

So there are some rules to make sure that we allow site owners to import only what is needed in their own SASS files:
- **BEM Block** - each block should be defined in its own importable item. A block should never be defined in the partial of another block or variant. These rules only apply to NCIDS specific items.
  * If your argument is that the subscribe block will only ever be used by the footer block, then you should be making a BEM element.
  * Four partials will be created:
    1. Internal Core Partial - This should contain all the markup that all the variants including the block would use. The partial will be placed in `ncids-css/sass/components/<Design-system-prefix>-<type>/internal/_shared.scss`
    2. Internal Partial for the "Default" variant - This should contain all the markup that the block with no modification would use. The partial will be placed in `ncids-css/sass/components/<Design-system-prefix>-<type>/internal/_<type>.scss` 
    3. External Partial - This is the partial that others will import. This basically imports all the dependencies and the internal partial. This is placed in `ncids-css/sass/components/<Design-system-prefix>-<type>/_<type>.scss`.
    4. All Partial - This is the partial that others will import if they want all variants of said BEM block. This is placed in `ncids-css/sass/components/<Design-system-prefix>-<type>/_all.scss`. For example, `usa-footer/_all.scss` will import `.usa-footer`, `.usa-footer--slim`, `.usa-footer--big`, and `usa-footer--nci-big`. 
- **BEM Variant** - each variant should be defined as its own importable item.
  * Two partials will be created:
    1. Internal Partial - This that contains all the SASS code for the component without referencing any other files. This is placed in `ncids-css/sass/components/<Design-system-prefix>-<type>/internal/_<variant>.scss`.
       * The all styles should be contained within the variant selector. E.g.
         ```css
         .usa-someblock--my-variant {
           ... styles and nested selectors ...
         }
         ```
    2. External Partial - This is the partial that others will import. This basically imports all the dependencies and the internal partial. This is placed in `ncids-css/sass/components/<Design-system-prefix>-<type>/_<variant>.scss`.
  * In the above example, the `.usa-footer--big` variant name would be `_big.scss`.
  * NOTE: The external partial should never contain the following:
    * `@import '@nciocpl/ncids-css/scss/base/required';`
    * `@import '@nciocpl/ncids-css/scss/base/normalize';`
    * `@import '@nciocpl/ncids-css/scss/base/global';`
</details>
</details>

<details>
<summary><h2>Component/Variant Implementation Process</h2></summary>
We are iteratively working through all the components & variants of the USWDS, determining what tweaks may be needed for NCI web sites. Additionally, we have other frequently used patterns across NCI sites that we will need to build components for.
<TODO>
</details>

<details>
<summary><h2>Storybook</h2></summary>

### Writing Storybook tests for your Components.
Each test should only include the below sass. Any dependencies should be included in the component's external partial. Additionally, your external partial should NOT include any uswds partials imported in required, normalize or global.

```css
@import '@nciocpl/ncids-css/scss/base/required';
@import '@nciocpl/ncids-css/scss/base/normalize';
@import '@nciocpl/ncids-css/scss/base/global';
@import '@nciocpl/ncids-css/scss/components/<YOUR_EXTERNAL_PARTIAL>';
```
</details>

<details>
<summary><h2>Reversing a Commit</h2></summary>

The `git revert` command can be used to to remove a commit that was previously merged. When reversing a commit, BackstopJS must be ran again as subsequent commits may update reference files. 

Steps:
1. `git checkout develop` to switch to development branch
2. `git pull --rebase origin develop` to get the most up to date version of the development branch
3. `git checkout -B ticket/###-short-name` to create a new branch and switch to it
4. `git revert <hash of commit to be removed>` to remove a specific commit. 
    - Notes: 
        - This will create a new commit. Do not change the generated commit message. 
        - `lerna bootstrap -- --frozen-lockfile` should be ran if this commit updates `package.json`
5. `yarn backstop:test` to check the diff
6. `yarn backstop:approve` to approve promote the diff to the new reference images
    - Notes: 
        - `yarn backstop:reference` should not need to be ran, but we may need to keep an eye on this
7. `git add .` to track new reference files with git
8. `git commit --amend` to a append the new reference images to the previous commit
9. `git push` 
10. Create a new PR from this commit. The generated message will pass OCPL Configuration Management Standards Check. Update the description with the findings of why the offending commit warranted a reverse instead of a change request.  
</details>