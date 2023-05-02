# Brightlayer UI themes for Angular applications

[![](https://img.shields.io/circleci/project/github/etn-ccis/blui-angular-themes/master.svg?style=flat)](https://circleci.com/gh/etn-ccis/blui-angular-themes/tree/master)
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
use '@brightlayer-ui/angular-themes/theme.scss'
use '@brightlayer-ui/angular-themes/open-sans.scss'
```

You can then apply the theme to your application by adding the proper class to your application's body element:

```HTML
// Default Theme
<body class="blui-blue">

// Dark Theme
<body class="blui-blue-dark">
```

> If you do not specify a theme class, your application will use the default Material theme.

## Customization

If you need to customize the styles (for OEM purposes for example). You can import the styles and define the customization in your top level scss file.

```scss
// in styles.scss or your top-level scss file
use '@brightlayer-ui/angular-themes/theme_bases';
use '@brightlayer-ui/angular-themes/open-sans.scss';

@include theme-bases.coreTypography();

body {
    $blui-blue-primary: mat.define-palette($primary);
    $blui-blue-accent: mat.define-palette($accent);
    $blui-blue-warn: mat.define-palette($warn);

    @include theme-bases.light-theme($blui-blue-primary, $blui-blue-accent, $blui-blue-warn);
}
```

Where the variables `$primary`, `$accent` and `$warn` must be a [palette](https://v15.material.angular.io/guide/theming#palettes). The values in the palette can be CSS custom properties or css colors.

# Custom Classes and Attributes

Brightlayer UI provides some custom classes and attributes that can be used to further align it with Material Design specifications.

### `blui-inline`

`blui-inline` is an attribute that can be placed on a `mat-button` that applies custom icon-sizing and placement.

#### Usage

```
<button blui-inline mat-flat-button color="primary">
    <mat-icon>download</mat-icon>
    <span>Download</span>
</button>
```

### `blui-input`

`blui-input` is an attribute that can be applied to a `mat-form-field` to standardize the height to be `56px`.

#### Usage

```ts
<mat-form-field blui-input appearance="standard">
    <input matInput placeholder="Placeholder" />
    <mat-label>Legacy</mat-label>
    <mat-hint>Hint</mat-hint>
    <mat-hint align="end">0/10</mat-hint>
    <mat-icon matSuffix>info</mat-icon>
    <mat-icon matPrefix>info</mat-icon>
</mat-form-field>
```

### `blui` Typography

Our [Brightlayer UI Typography guidelines](https://brightlayer-ui.github.io/style/typography) align with Material Design's recommended naming convention and size specifications.  
We have included a custom set of `blui-[name]` classes to match our documentation, eliminating the need to cross-reference Angular Material's default typography naming convention to find a specific correct font.

#### Usage

```
<div class="blui-headline-1">Headline 1</div>
<div class="blui-headline-2">Headline 2</div>
...
<div class="blui-overline">Overline</div>
```

#### Migration

If you are using an older version of the themes package and wish to update, check out our [migration guide](https://github.com/etn-ccis/blui-angular-themes/blob/master/MIGRATION.md);

## Demo

[Interactive Demo](https://blui-angular-showcase.web.app/)
