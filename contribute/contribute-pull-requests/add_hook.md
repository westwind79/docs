---
title: Adding a new hook
weight: 3
---

# How to add a new Hook
Adding a new hook is a process that can be done in only three steps.

## 1) Add a call to Hook::exec()

As visible in [this PR](https://github.com/PrestaShop/PrestaShop/pull/34431/files), the first step is to add a `Hook::exec()` in the code where you want to execute it. This will execute the code from the modules hooked into your `Hook`.

## 2) Modify the hook.xml file

The second step is correctly adding the `Hook` during installation. You need to add it to the `hook.xml` file, as seen in this [PR](https://github.com/PrestaShop/PrestaShop/pull/34431/files). This will ensure that the `Hook` is added to the database, which enables users to sort modules hooked into it. It won't be possible without the hook in the database.

## 3) Add the new hook in the Autoupgrade fixture

The last step is to make this new hook available for users upgrading from older versions of PrestaShop. You need to add it to the current version of the SQL script of the Autoupgrade module, as can be seen in this [PR](https://github.com/PrestaShop/autoupgrade/pull/672/files).

If you are unsure which file to put the code inside the [autoupgrade module](https://github.com/PrestaShop/autoupgrade), feel free to ping `@PrestaShop/Committers`.

You can also use a [helper](https://github.com/PrestaShop/autoupgrade/pull/577/files) available to add a new hook during the upgrade process for a given version.