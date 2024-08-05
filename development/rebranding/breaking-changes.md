---
title: Breaking changes
weight: 64
useMermaid: true
---

# Breaking changes in PrestaShop BO rebranding

The rebranding of the PrestaShop back office introduces a few breaking changes. These updates are essential for aligning the BO with the new design standards and ensuring a consistent user experience. Here’s what you need to know:

## Notable breaking changes

- **New Fonts**: The adoption of `IBM Plex Sans` and `Material Symbols` is part of the rebranding effort. These fonts are included in the `default` theme and also the `new-theme` through the UI Kit.

- **Removal of `postcss.config.js`**: This file, which used the deprecated `postcss-cssnext` package, has been removed, and this package is no longer needed.

- **Removal of SCSS files**: The file `admin-dev/themes/default/scss/modules/_colors.scss` and the directory `admin-dev/themes/default/scss/modules/colors/` are no longer used in the back office and have been removed. Update your stylesheets to avoid relying on these outdated resources.

These changes are important for modernizing the back office and aligning it with PrestaShop's new brand design. Be sure to update your development workflows to accommodate these updates and maintain compatibility with the latest PrestaShop version.

{{% children /%}}
