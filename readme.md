# Shared Github Actions

## Deploy to WP Engine

## PHPCS

## Playwright Tests

---

# Changelog

## v1.8.0 - [April 10, 2026]

- Added: `phpcs` includes a custom path for running composer installs from places _other_ than the root (/public) folder
- Updated: `phpcs` uses default branches

## v1.7.2 - [April 9, 2026]

- Fixed: Updated composer install path to theme dir for proper deployment to WP Engine

## v1.7.1 - [April 8, 2026]

- Fixed: Passed additional flags to default "deploy" to WP Engine sites (per [action readme](https://github.com/wpengine/github-action-wpe-site-deploy/tree/main/?tab=readme-ov-file))

## v1.7.0 - [April 6, 2026]

- Added: `with_autoload` flag now supported on theme deploys to WP Engine
- Added: `node_version` flag now supported on node actions
- Added: `php_version` input now supported

## v1.6.0 - [March 31, 2026]

- Updated: Node uses `lts/*`

## v1.5.0 - [March 11, 2026]

- Added: Better logic to try to use built assets instead of re-building assets every time
- Added: PHPUnit tests workflow
- Added: deploy-release (for plugins) now supports autoloading.
- Updated: Actions use latest versions (`@main` or `@master`)

## v1.4.1 - [Feb 11, 2026]

- Reset `deploy` to use `ubuntu-latest` for cheaper actions (un-does 1.1.2 change)

## v1.4.0 - [Dec 11, 2025]

- Added: New optional flag for `phpcs` arg to pass PHP value (default "latest")
- Fixed: potential bug in phpcs yml file (removed trailing `'`).

## v1.3.0 - [Oct 20, 2025]

- Added: New, optional "Flags" argument to pass rsync flags to [`wpe-site-deploy` action](https://github.com/wpengine/github-action-wpe-site-deploy)
- Tweak: Focus `wpe deploy` action to the theme folder **only**

## v1.2.0 - [Aug 27, 2025]

- Added: New "lint-if-changed" shared action to lint style/js files!
- Updated: "Checkout" action bumped to v5
- Updated: PHPCS code checks only run if `composer.json` file exists and PHP files were changed
- Updated: Swapped `composer_json_check` from Github Env to step OUTPUTS for uniformity with `check-php-files`

## v1.1.3 - [Aug 08, 2025]

- Add check if composer.json file exists to PHPCS

## v1.1.2 - [Aug 08, 2025]

- Add a cache-busting mechanism for npm deps.
- Force `npm ci` to run on macos-latest for highest compatibility with current dev systems.

## v1.1.1

- Update Deploy to Github Release to trim whitespace from the Version variable.

## v1.1.0

- Add "Deploy to Github Release" for plugins
- Add caching for npm dependencies!

## v1.0.0

- Init actions!
