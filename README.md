# Brightlayer UI themes for Angular applications

[![](https://img.shields.io/circleci/project/github/brightlayer-ui/angular-themes/master.svg?style=flat)](https://circleci.com/gh/brightlayer-ui/angular-themes/tree/master)
[![](https://img.shields.io/npm/v/@brightlayer-ui/angular-themes.svg?label=@brightlayer-ui/angular-themes&style=flat)](https://www.npmjs.com/package/@brightlayer-ui/angular-themes)

This package provides theming support for Eaton applications using the Brightlayer UI design system. It includes resources for developers using Angular w/ [Angular Material](https://www.npmjs.com/package/@angular/material). This package comes with two theme options: a Blue theme (standard) and a Dark theme.

For other frameworks, check out our related packages:

-   [@brightlayer-ui/react-themes](https://www.npmjs.com/package/@brightlayer-ui/react-themes)
-   [@brightlayer-ui/react-native-themes](https://www.npmjs.com/package/@brightlayer-ui/react-native-themes)

## Installation

Install with npm

```shell
npm install --save @brightlayer-ui/angular-themes
```

or yarn

```shell
yarn add @brightlayer-ui/angular-themes
```

## Usage

In order to use the Brightlayer UI themes and font (Open Sans), you will need to modify your angular.json file "styles" entries (there is one under "build" and one under "test") to include the Brightlayer UI themes and Open Sans reference:

```js
"styles": [
    "src/styles.scss",
    "./node_modules/@brightlayer-ui/angular-themes/theme.scss",
    "./node_modules/@brightlayer-ui/angular-themes/open-sans.scss"
],
```

Alternatively, you can also import the theme file in your top-level SCSS file.

```scss
// in styles.scss or your top-level scss file
import '~@brightlayer-ui/angular-themes/theme.scss'
import '~@brightlayer-ui/angular-themes/open-sans.scss'
```

You can then apply the theme to your application by adding the proper class to your application's body element:

```HTML
// Default Theme
<body class="blui-blue">

// Dark Theme
<body class="blui-blue-dark">
```

> If you do not specify a theme class, your application will use the default Material theme.

### Updating From Version 5 ~> 6

In version 6, we have migrated from the deprecated `typeface-open-sans` package to `@fontsource/open-sans` (bundled with the Brightlayer UI themes). You'll need to update your Open Sans references in angular.json:

Before:

```js
'./node_modules/typeface-open-sans';

```

After:

```js
'./node_modules/@brightlayer-ui/angular-themes/open-sans.scss';

```

## Demo

[View on Stackblitz](https://stackblitz.com/github/brightlayer-ui/angular-showcase-demo/tree/master)
