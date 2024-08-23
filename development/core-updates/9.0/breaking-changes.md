---
title: BO breaking changes
weight: 73
---

# Breaking changes in PrestaShop BO

The rebranding of the PrestaShop back office introduces several breaking changes. These updates are necessary to align the back office with new design standards and ensure a consistent user experience.

## Notable breaking changes

- **New Fonts**: The adoption of `IBM Plex Sans` and `Material Symbols` is part of the rebranding effort. These fonts are included in both the `default` theme and also the `new-theme` through the UI Kit.

- **Removal of `postcss.config.js`**: The `postcss.config.js` file, which used the deprecated `postcss-cssnext` package, has been removed. This package is no longer needed.

- **Removal of SCSS Files**: The file `admin-dev/themes/default/scss/modules/_colors.scss` and the directory `admin-dev/themes/default/scss/modules/colors/` have been removed. These are no longer used in the back office. Update your stylesheets to avoid relying on these outdated resources.

These changes are essential for modernizing the back office and aligning it with PrestaShop’s new brand design. Update your development workflows to accommodate these changes and maintain compatibility with the latest PrestaShop version.

{{% children /%}}
