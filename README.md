# Kollegorna's Design System Boilerplate

This is a boilerplate for setting up design systems at Kollegorna. It provides a basic folder structure and sensible defaults for setting up reusable styles. It should be used as the basis for any new project.

## Using in an application

### Development

We suggest you keep the design system in its own folder, inside the main application's assets folder. This will let you easily tweak and add to the design system.

1. Navigate to your app's stylesheets folder
2. `$ git clone git@github.com:kollegorna/design-system-boilerplate.git design-system`
3. `$ cd design-system`
4. `$ git remote rm origin`
5. Add `@import "design-system/scss/design-system";` to your main css file


### Production

Before the project enters production mode, the design system should be moved into its own repository, and declared as a dependency on the master app. If you're using [yarn](https://yarnpkg.com/) to manage dependencies on the main repo, you can simply run `yarn add [style-guide-repository-url]`. Remember to update the `@import` declarations where needed afterwards.
