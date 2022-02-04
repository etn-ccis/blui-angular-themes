# Changelog

## v6.4.0 (Not yet published)

### Added

-   Added `blui-inline` attribute styles to `mat-button`. ([#31](https://github.com/brightlayer-ui/angular-themes/issues/31))
-   Added new `outline` and `filled` variant for `<mat-toggle-button>`.([#19](https://github.com/brightlayer-ui/angular-themes/issues/19))

### Fixed

-   Fixed non-center aligned chevron in `<mat-expansion-panel-header>`. ([#50](https://github.com/brightlayer-ui/angular-themes/issues/50))
-   Fixed disabled slider color in `<mat-slider>`. ([#27](https://github.com/brightlayer-ui/angular-themes/issues/27))
-   Fixed text color of active option in `<mat-select>` for light and dark mode. ([#18](https://github.com/brightlayer-ui/angular-themes/issues/18))
-   Fixed dark-mode text and icon color in `<mat-toolbar>`. ([#18](https://github.com/brightlayer-ui/angular-themes/issues/59))

### Changed

-   Updated `mat-form-field` styles ([#48](https://github.com/brightlayer-ui/angular-themes/issues/48)).
-   Updated table styles to match design specifications ([#38](https://github.com/brightlayer-ui/angular-themes/issues/38), [#36](https://github.com/brightlayer-ui/angular-themes/issues/36)).
-   Changed default font-size of `.mat-tooltip` text to `12px`.([#10](https://github.com/brightlayer-ui/angular-themes/issues/10))
-   Changed default height of `.mat-row` to `52px`.([#37](https://github.com/brightlayer-ui/angular-themes/issues/37))
-   Changed `mat-table` header styles. ([#36](https://github.com/brightlayer-ui/angular-themes/issues/36))

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
