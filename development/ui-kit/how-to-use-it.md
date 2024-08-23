---
title: How to use it ?
weight: 63
---

# How to use new set of CSS variables ?

To maintain consistency across the PrestaShop back office, CSS variables have been introduced in `_root.scss`. This guide explains how to use these variables in PrestaShop.

## Using CSS variables with v9 and higher

In PrestaShop v9 and higher, use the CSS variables introduced in `_root.scss` for consistent styling in the Back Office.

### Usage Example

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

**Note:**

- `--cdk-primary-800` is a CSS variable defined in `_root.scss`. It ensures consistent color application across the back office.
- Refer to `_root.scss` for the latest <a href="https://github.com/PrestaShop/prestashop-ui-kit/blob/develop/scss/_root.scss" target="_blank">list of available variables</a>.

## Using CSS variables with older versions

For PrestaShop versions without the UI Kit v2, use fallbacks to ensure compatibility.

### Fallback Example

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

**Note:**

- Fallback values (e.g., `#1b1c1d`) ensure functionality in versions without the new UI Kit v2.

{{% children /%}}
