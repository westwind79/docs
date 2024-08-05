---
title: Introduction
weight: 61
useMermaid: true
---

# PrestaShop BO rebranding

By the end of 2023, PrestaShop unveiled its new brand identity to reinforce its strengths and enhance credibility and trust. The PrestaShop back office was one of the final assets to be rebranded, and the release of PrestaShop 9 provided an ideal opportunity for this update.

## Anatomy of PrestaShop back office

The PrestaShop Back Office consists of [two themes][bo-themes]. Modifications have been made to both themes to achieve a complete rebranding of the Back Office:

### Theme: default
- Used for legacy controllers
- Based on **Bootstrap 3**
- Now includes `_root.scss` file from the **PrestaShop UI Kit**

### Theme: new-theme
- Used for Symfony controllers
- Based on **Bootstrap 4**
- Utilizes the **PrestaShop UI Kit**

{{% children /%}}

[bo-themes]: {{< ref "/9/development/architecture/introduction.md#bo-themes" >}}