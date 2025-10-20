# Shared Github Actions

## Deploy to WP Engine

## PHPCS

## Playwright Tests

---

# Changelog

## v1.3.0 - [Oct 20, 2025]

-   Added: New, optional "Flags" argument to pass rsync flags to [`wpe-site-deploy` action](https://github.com/wpengine/github-action-wpe-site-deploy)

## v1.2.0 - [Aug 27, 2025]

-   Added: New "lint-if-changed" shared action to lint style/js files!
-   Updated: "Checkout" action bumped to v5
-   Updated: PHPCS code checks only run if `composer.json` file exists and PHP files were changed
-   Updated: Swapped `composer_json_check` from Github Env to step OUTPUTS for uniformity with `check-php-files`

## v1.1.3 - [Aug 08, 2025]

-   Add check if composer.json file exists to PHPCS

## v1.1.2 - [Aug 08, 2025]

-   Add a cache-busting mechanism for npm deps.
-   Force `npm ci` to run on macos-latest for highest compatibility with current dev systems.

## v1.1.1

-   Update Deploy to Github Release to trim whitespace from the Version variable.

## v1.1.0

-   Add "Deploy to Github Release" for plugins
-   Add caching for npm dependencies!

## v1.0.0

-   Init actions!
