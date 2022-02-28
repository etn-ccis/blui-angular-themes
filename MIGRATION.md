# Migration Guide

This document covers integration differences between major versions of our themes.

## Updating From Version 6 ~> 7

In version 7, we have updated our `@angular/material` dependency from v12 to v13 which has changed the way our themes are imported in project's styles.

Before:

```scss
import '~@brightlayer-ui/angular-themes/theme.scss'
import '~@brightlayer-ui/angular-themes/open-sans.scss'
```

After:

```scss
use '@brightlayer-ui/angular-themes/theme.scss'
use '@brightlayer-ui/angular-themes/open-sans.scss'
```

## Updating From Version 5 ~> 6

In version 6, we have migrated from the deprecated `typeface-open-sans` package to `@fontsource/open-sans` (bundled with the Brightlayer UI themes). You'll need to update your Open Sans references in angular.json:

Before:

```js
'./node_modules/typeface-open-sans';
```

After:

```js
'./node_modules/@brightlayer-ui/angular-themes/open-sans.scss';
```
