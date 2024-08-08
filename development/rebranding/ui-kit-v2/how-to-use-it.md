---
title: How to use it ?
weight: 65
useMermaid: true
---

# How to use new set of CSS variables ?

To maintain consistency across the PrestaShop back office, the introduction of new CSS variables in `_root.scss` plays a important role. This guide will show you how to effectively utilize these variables in both PrestaShop v9 and older versions.

- <a href="https://github.com/PrestaShop/prestashop-ui-kit/blob/1c255d96d79c69e2d3e0dd1712f76379941c06bb/scss/_root.scss#L122" target="_blank">See exposed CSS variables</a>
- [More information about PrestaShop UI Kit][ps-ui-kit]

## Using CSS variables with v9 and higher

When developing new features or updating existing ones in the Back Office for PrestaShop v9 and higher, you can leverage the new CSS variables introduced in `_root.scss`. These variables ensure a consistent styling approach across the back office interface.

### How to Use CSS Variables

Here’s how you can apply these variables in your CSS or SCSS:

```scss
/* CSS: Apply dark background on a block */
.my-block {
  background-color: var(--cdk-primary-800);
}

/* SCSS: Apply dark background on a block */
.my-block {
  background-color: var(--#{$cdk}primary-800);
}
```

#### Explanation:

`--cdk-primary-800` is a CSS variable defined in `_root.scss`. It ensures that the color applied to `.my-block` remains consistent with the new design. These variables refer to specific color values that stay uniform across the back office, helping maintain design consistency.

**Tip:** Always refer to `_root.scss` for the most up-to-date <a href="https://github.com/PrestaShop/prestashop-ui-kit/blob/1c255d96d79c69e2d3e0dd1712f76379941c06bb/scss/_root.scss#L122" target="_blank">list of available variables</a>. This ensures you use the correct variables for your styling needs and that your design aligns with the latest updates.

## Using CSS variables with older versions

For PrestaShop versions that do not include the new UI Kit v2, you should provide fallbacks to ensure compatibility. Here’s how you can include a fallback for older versions:

### How to use CSS variables with fallback

```scss
/* CSS: Apply dark background on a block with fallback */
.my-block {
  background-color: var(--cdk-primary-800, #1b1c1d);
}

/* SCSS: Apply dark background on a block with fallback */
.my-block {
  background-color: var(--#{$cdk}primary-800, #1b1c1d);
}
```

#### Explanation:

Using fallbacks ensures that your styles remain functional in PrestaShop versions that do not include the new UI Kit v2. The fallback value (e.g., `#1b1c1d` in this case) serves as a default if the CSS variable is not recognized or available.

{{% children /%}}

[ps-ui-kit]: {{< ref "/9/development/uikit.md" >}}
