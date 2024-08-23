---
title: BO rebranding
weight: 72
---

# PrestaShop back office rebranding

By the end of 2023, PrestaShop introduced a new brand identity to reinforce its strengths and enhance credibility and trust. The PrestaShop back office was one of the final components to undergo rebranding, with the release of PrestaShop 9 providing an ideal opportunity for this update.

## Anatomy of PrestaShop back office

The PrestaShop back office consists of [two themes][bo-themes]. Both themes have been modified to achieve a complete rebranding:

### Theme: default
- Used for legacy controllers
- Based on **Bootstrap 3**
- Now includes `_root.scss` file from the **PrestaShop UI Kit** to expose CSS variables from the UI Kit


### Theme: new-theme
- Used for Symfony controllers
- Based on **Bootstrap 4**
- Utilizes the **PrestaShop UI Kit**

{{% children /%}}

[bo-themes]: {{< ref "/9/development/architecture/introduction.md#bo-themes" >}}
