SASS compiler for a custom Starterkit subtheme.
=============================================

In Drupal 10, the Classy theme has been replaced by the new Starterkit theme generator. The Starterkit theme generator is now the recommended way to creating new themes, to be done instead of setting a theme's base theme: to core theme such as classy
https://www.drupal.org/node/3305674

1. Create a new starterkit subtheme:
  - create the web/themes/custom folder
  - run from web folder tis command: php core/scripts/drupal generate-theme my_theme --path themes/custom

2. Create the sass and js folder in your custom theme
  - create the themes/custom/MY_THEME/src/sass folder. Here will be your sass files.
  - create the themes/custom/MY_THEME/src/js folder. Here will be your js files.

3. Copy these files in themes/custom/MY_THEME
  - .gitignore
  - babel.config.json
  - example.env
  - gulpfile.js
  - package.lock.json
  - package.json

4. Create the .env file
  - make a copy of the example.env named .env
  - in the .env file change the "my.site.local" into your localhost site name.

5. Change the default "my_theme" into your subtheme name in the following files:
  - package.json
  - package-lock.json

6. Install the node modules, running this command from your theme folder
  - npm install

7. Run the compiler:
  - npm start

Enjoy!

