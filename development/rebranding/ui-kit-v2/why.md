---
title: Why a new version ?
weight: 63
useMermaid: true
---

# PrestaShop UI Kit v2

The PrestaShop UI Kit has been fully rebranded and is available starting from **v2.0.1**. This update introduces a new file named `_root.scss`, which defines CSS variables for both the `default` and `new-theme` in PrestaShop BO from **v9.0.0**.

The `_root.scss` file serves as a single source of truth for CSS variables, ensuring consistency in the Back Office design. All UI Kit components have been updated to work with this new set of variables, and Bootstrap has been recompiled to maintain component functionality.

<a href="https://github.com/PrestaShop/prestashop-ui-kit/blob/1c255d96d79c69e2d3e0dd1712f76379941c06bb/scss/_root.scss#L122" target="_blank">See exposed CSS variables</a>

## Why rebrand the UI Kit?

The rebranding of the PrestaShop back office necessitated a comprehensive update to the UI Kit. Here’s why:

- **Introduction of CSS variables:** We created a new version of the UI Kit (v2) that includes a newly defined set of CSS variables. These variables, now exposed within the BO, align the UI Kit with the new PrestaShop brand design.

- **Consistent design implementation:** The UI Kit components were updated to utilize this new set of CSS variables. This ensures that the new design is applied consistently across the back office interface.

These updates not only provide a modern and cohesive look for the back office but also help ensure design consistency across the whole user interface

{{% children /%}}
