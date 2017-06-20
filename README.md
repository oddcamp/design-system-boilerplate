# Kollegorna's Design System Boilerplate

This is a boilerplate for setting up design systems at Kollegorna. It provides a basic folder structure and sensible defaults for setting up reusable styles. It should be used as the basis for any new project.

## Using in an application

We suggest you keep the design system in its own folder, inside the main application's assets folder. This will let you easily tweak and add to the design system.

1. Navigate to your app's stylesheets folder
2. `$ git clone git@github.com:kollegorna/design-system-boilerplate.git design-system`
3. `$ cd design-system`
4. `$ git remote rm origin`
5. Add `@import "design-system/scss/design-system";` to your main css file

Before moving into production, the design system should be moved into its own repository, and declared as a dependency on the master repository.

## Local setup for viewing or developing

We've setup a style guide using [Middleman](https://middlemanapp.com) which should be used when previewing or developing the design system.

1. Install [Bundler](https://rubygems.org/gems/bundler) and [Node.js](http://nodejs.org).
2. `$ git clone git@github.com:kollegorna/design-system.git`
3. `$ cd design-system/styleguide`
4. `$ npm install`
5. `$ gulp install`

### Gulp commands

- `$ gulp install`
    - Runs: bundle install and bower install
- `$ gulp serve`
    - Builds Middleman and create a browser-sync server
- `$ gulp build`
    - Builds Middleman
