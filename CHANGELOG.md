# Changelog

## v9.0.0 (TBD)

### Changed

-   Updated to Angular 15 for building the library. The lib will use the legacy Material components (not the MDC Web).

## v8.1.0 (April 13, 2023)

### Fixed

-   Fixed `<blui-drawer-header>` `color` prop issue ([#152](https://github.com/etn-ccis/blui-angular-themes/issues/152)).
-   Fixed `<mat-select>` wrong label and underline color ([#67](https://github.com/etn-ccis/blui-angular-themes/issues/67)).
-   Fixed dropdown arrow not vertically aligned issue in `<mat-select>` ([#78](https://github.com/etn-ccis/blui-angular-themes/issues/78)).
-   Fixed chip mixin to use correct accent color issue ([#72](https://github.com/etn-ccis/blui-angular-themes/issues/72)).
-   Fixed `<blui-inline>` does not work with inline svg icons issue ([#133](https://github.com/etn-ccis/blui-angular-themes/issues/133)).
-   Fixed Dark theme `<blui-drawer-header>` text and icon color issue ([#79](https://github.com/etn-ccis/blui-angular-themes/issues/79)).
-   Fixed an issue where the browser default password reveal button collides with any matSuffix input icon provided ([#168](https://github.com/etn-ccis/blui-angular-themes/issues/168)).

### Added

-   Support for CSS Custom properties customization.

## v8.0.0 (November 21, 2022)

### Changed

-   Updated to Angular 14 for building the library.

## v7.0.1 (June 20, 2022)

### Fixed

-   Fixed incorrect autocomplete colors for input fields in dark theme ([#76](https://github.com/etn-ccis/blui-angular-themes/issues/76)).
-   Fixed default `mat-button` height not being 36px. ([#103](https://github.com/etn-ccis/blui-angular-themes/issues/103))
-   Fixed `mat-expansion-panel-header` border color not similar to divider color ([#107](https://github.com/etn-ccis/blui-angular-themes/issues/107))
-   Fixed `<blui-info-list-item>` disabled state when within a `<mat-nav-list>` ([#114](https://github.com/etn-ccis/blui-angular-themes/issues/114))
-   Fixed stepper input styles ([#90](https://github.com/etn-ccis/blui-angular-themes/issues/90))
-   Fixed `mat-button-toggle` border styles ([#109](https://github.com/etn-ccis/blui-angular-themes/issues/109))

## v7.0.0 (March 14, 2022)

### Added

-   Added support for Angular v13.
-   Added `blui` typography rules. ([#49](https://github.com/etn-ccis/blui-angular-themes/issues/49))

### Changed

-   Changed Angular Material default typography ruleset to match specifications on our [documentation site](https://brightlayer-ui.github.io/style/typography).

## v6.4.1 (March 1, 2022)

### Fixed

-   Fixed bug where `blui-inline` didn't align buttons with prefix and postfix icons. ([#94](https://github.com/etn-ccis/blui-angular-themes/issues/94))

## v6.4.0 (February 11, 2022)

### Added

-   Added `blui-inline` attribute styles to `mat-button`. ([#31](https://github.com/etn-ccis/blui-angular-themes/issues/31))
-   Added `blui-input` attribute styles to `mat-form-field`.
-   Added new `outline` and `filled` variant for `<mat-toggle-button>`.([#19](https://github.com/etn-ccis/blui-angular-themes/issues/19))

### Fixed

-   Fixed non-center aligned chevron in `<mat-expansion-panel-header>`. ([#50](https://github.com/etn-ccis/blui-angular-themes/issues/50))
-   Fixed disabled slider color in `<mat-slider>`. ([#27](https://github.com/etn-ccis/blui-angular-themes/issues/27))
-   Fixed text color of active option in `<mat-select>` for light and dark mode. ([#18](https://github.com/etn-ccis/blui-angular-themes/issues/18))
-   Fixed dark-mode text and icon color in `<mat-toolbar>`. ([#18](https://github.com/etn-ccis/blui-angular-themes/issues/59))

### Changed

-   Updated `mat-form-field` styles ([#48](https://github.com/etn-ccis/blui-angular-themes/issues/48)).
-   Updated table styles to match design specifications ([#36](https://github.com/etn-ccis/blui-angular-themes/issues/36), ([#37](https://github.com/etn-ccis/blui-angular-themes/issues/37)), [#38](https://github.com/etn-ccis/blui-angular-themes/issues/38)).
-   Changed default font-size of `.mat-tooltip` text to `12px`.([#10](https://github.com/etn-ccis/blui-angular-themes/issues/10))

## v6.3.0 (November 3, 2021)

### Changed

-   Changed package namespace from `@pxblue` to `@brightlayer-ui`.

## Package Migration Notice

Previous versions listed after this indicator refer to our deprecated `@pxblue` packages.

---

## v6.3.0 (September 28, 2021)

### Added

-   Added theme support for `UserMenuHeaderComponent`.
-   Red text highlight color for invalid form fields.
-   Applied Open Sans font family to HTML `<input>` elements.

### Fixed

-   Fixed light theme active item icon color for `<pxb-drawer>`.

### Changed

-   Changed `<mat-button-toggle-group>` default height to 36px.

## v6.2.1 (August 30, 2021)

### Fixed

-   Fixed bug in `<mat-chip>` styles where non-selected chips appeared as selected.

## v6.2.0 (August 25, 2021)

### Added

-   Added new `stroked` variant for `<mat-chip>` and adjusted default chip theme.

### Changed

-   Default `<mat-chip>` icon size to be 18x18 pixels.

## v6.1.1 (June 30, 2021)

### Fixed

-   Fixed a few color issues in the `<pxb-drawer-header>` ([#184](https://github.com/pxblue/themes/issues/184)) and `<pxb-drawer-nav-item>` ([#186](https://github.com/pxblue/themes/issues/186)).

### Changed

-   Changed `mat-button` styles for disabled `primary`, `accent`, and `warn` variants.

## v6.1.0 (May 28, 2021)

### Added

-   Added support for `<pxb-user-menu>` bottomsheet overlay.

## v6.0.3 (April 8, 2021)

### Fixed

-   Fixed disabled icon & text color for `<pxb-info-list-item>` and `<mat-menu-item>`.
-   Fixed dark-mode active item text color for `<pxb-drawer>` rail variant.

## v6.0.2 (April 5, 2021)

### Fixed

-   Fixed default `<pxb-drawer-header>` and `<pxb-dropdown-toolbar>` background color.

## v6.0.1 (March 31, 2021)

### Added

-   Added `<pxb-score-card>` badge background theme.

### Fixed

-   Fixed missing navigation rail active-item font-color bug.
-   Fixed missing navigation rail hover highlight.

### Changed

-   Adjusted `<mat-form-field>` blue-theme colors.
-   Updated deprecated `typeface-open-sans` dependency to `@fontsource/open-sans`.
-   Changed several dark mode defaults.
-   Updated `<pxb-empty-state>` default colors.
-   Updated CSS rule-specificity for some default styles. If you have been using custom style overrides, check to make sure that your rules are specific enough to take precedence over the defaults.

## v5.2.0 (December 10, 2020)

### Added

-   Add theme for `<pxb-mobile-stepper>`.

### Changed

-   Update `filled` input field light-themed background color.
-   Update `<pxb-drawer>` theme.

## v5.1.2 (September 30, 2020)

### Added

-   Add style rules for `<mat-stepper>`.

### Changed

-   Rename class used to highlight `<pxb-drawer>` selection.

### Removed

-   Remove `<mat-button>` uppercase default behavior.

## v5.1.1 (August 14, 2020)

### Fixed

-   Fix an issue with with setting a color for `<pxb-info-list-item>` text.

## v5.1.0 (July 22, 2020)

### Added

-   Add UserMenu theme.

## v5.0.0 (June 30, 2020)

### Changed

-   Update theme definitions to use the [@pxblue/colors](https://www.npmjs.com/package/@pxblue/colors) version 3.0.0.
<!-- - Update color schemes to address accessibility concerns. -->
-   Update default typography styles for consistency.

## v4.0.0 (February 24, 2020)

### Changed

Themes have been broken out into their own packages. This package was originally part of @pxblue/themes. If you are switching to this package, you'll need to update some import statements (refer to the usage instructions in the README).

-   Includes minor color adjustments for outlined buttons in blue theme and cards in dark theme.
