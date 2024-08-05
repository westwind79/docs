---
title: Refactoring BO themes
weight: 63
useMermaid: true
---


# Refactoring PrestaShop BO themes

The PrestaShop back office rebranding involves two themes: `default` and `new-theme`. While `new-theme` is based on the PrestaShop UI Kit, the `default` theme is not. To achieve a cohesive redesign across both themes, we implemented a comprehensive refactoring process, including the introduction of `_root.scss` in the `default` theme on PrestaShop v9.

## Themes overview

Both themes required updates to ensure a unified look and feel for the rebranding effort.

### Necessity for refactoring

To harmonize the design, we updated the **theme specific code** for both themes. We introduced CSS variables from the UI Kit to centralize design elements and ensure consistency across the entire back office. The use of `_root.scss` provided a single source of truth for design variables, allowing us to apply uniform styles across both themes effectively.

### Default theme example tool

A quick tool has been set up for those who want to visualize most of the components available in the default theme and see what they look like now. This can be useful for those who want to use these components and see how they will look on PrestaShop v9.

To use this tool, open your terminal and go to the directory `admin-dev/themes/default`, ensure npm packages are installed, and run the following CLI command: `npm run example`. This will open a browser page listing the components available in the default theme.


{{% children /%}}
