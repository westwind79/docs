---
title: Introducing CSS variables
weight: 64
useMermaid: true
---

# CSS variables

Towards design harmonization with the use of CSS variables across the BO

## Why use CSS variables?

CSS variables offer numerous advantages in web development, especially in large-scale projects like PrestaShop. Here’s why they are beneficial:

### 1. Avoiding naming conflicts

In complex projects with multiple themes or libraries, variable names can easily overlap. By using prefixes like `cdk-` (which stands for Core Design Kit), you ensure that your variables are unique and won't inadvertently override variables from other parts of the project or third-party libraries.

### 2. Maintaining consistency

Using a consistent naming convention, such as the `cdk` prefix, helps developers quickly identify variables that belong to the UI Kit. This ensures a cohesive design language throughout the project.

### 3. Foundation for future

Using CSS variables is a step towards creating design tokens. This approach lays the groundwork for potential future features, such as customizable back-office interface colors, and enhances flexibility for future developments.

### Summary

Using CSS variables with prefixes enhances consistency, readability, and maintenance, making it a best practice for managing styles in complex projects.

For example, `--cdk-primary-800` represents a color in the Core Design Kit. This prefix ensures that the variable is recognized as part of the Core Design Kit, preventing conflicts with other variables and maintaining design consistency. Overall, this practice helps manage styles effectively by standardizing design elements and improving code clarity across the back office.

{{% children /%}}
