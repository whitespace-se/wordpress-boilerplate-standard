# Wordpress Standard Boilerplate

Boilerplate for a standard setup of Wordpress

## How to install

1. Create project with Composer
   ```bash
   composer create-project whitespace-se/wordpress-boilerplate-standard <folder>
   ```
2. Update package name, author and description in _composer.json_ and
   _package.json_.
3. Duplicate all example files in /config and update them to match your setup.
4. Create your empty database.
5. Run `valet link`.
6. Run `valet open` and then the Wordpress install wizard.

### Install and activate ACF Pro

1. Create a .env file and add your ACF Pro key.
2. Install ACF Pro:
   ```bash
   composer require "advanced-custom-fields/advanced-custom-fields-pro":"*"
   ```
3. Activate the ACF Pro plugin:
   ```bash
   wp plugin activate advanced-custom-fields-pro
   ```

### Final steps

1. Set `phpVersion` inside _.prettierrc.yml_ to the lowest version of PHP
   required by your environments.

## Format code using Prettier

1. Run `yarn install` to install Prettier.
2. Run `yarn format` to format all applicable files.
3. Install a sutiable Prettier plugin for you aditor to format files
   automatically on save.
4. Also install the Editorconfig for your editor to format files not supported
   by Prettier.
