---
Title: actionAfterLoadRoutes
hidden: true
hookTitle: 
files:
    -
        url: 'https://github.com/PrestaShop/PrestaShop/blob/8.1.x/classes/Dispatcher.php#L708'
        file: classes/Dispatcher.php
locations:
    - 'front office'
    - 'back office'
type: action
hookAliases: 
array_return: false
check_exceptions: false
chain: false
origin: core
description: ''

---

{{% hookDescriptor %}}

## Call of the Hook in the origin file

This hook was added in {{< minver v="8.1.2" >}}.

```php
Hook::exec('actionAfterLoadRoutes', ['dispatcher' => $this, 'id_shop' => $id_shop]);
```

Parameter `$id_shop` has been added in version {{< minver v="8.1.5" >}}.