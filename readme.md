# WordPress.org Pattern Directory

## Prerequisites
- Docker
- Node/NPM
- Yarn
- Composer

## Setup
1. `yarn`
2. `yarn run create`
3. Visit site at `localhost:8888`

## Stopping Environment
run `yarn run wp-env stop`

## Removing Environment
run `yarn run wp-env destroy`

## Development

While working on the theme & plugin, you might need to rebuild the CSS or JavaScript.

To build both projects, you can run:

	yarn workspaces run build

To build one at a time, run

	yarn workspace wporg-pattern-directory build

If you want to watch for changes, run `start`. This can only be run in one project at a time:

	yarn workspace wporg-pattern-directory start

### Linting

This project has eslint, stylelint, and phpcs set up for linting the code. This ensures all developers are working from the same style. To check your code before pushing it to the repo, run

	yarn workspace wporg-pattern-directory lint:css
	composer run lint

These checks will also be run automatically on each PR.