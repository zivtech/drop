# drop
Just a drop of Drupal.

Drop is a very lightweight set of files to get started with building a Drupal 8 website.

The basic idea of drop is to start with a well maintained base install, such as [Drops 8](https://github.com/pantheon-systems/drops-8) or [Composer Drupal Project](https://github.com/drupal-composer/drupal-project), and add additional modules and libraries to the composer.json. Later we may also look at exporting some base config options that can be imported to any new site build.

## Get Started With a Base
First grab [Drops 8](https://github.com/pantheon-systems/drops-8) for Pantheon hosted sites, or spin up a new site on Pantheon and pull down the repository. Sites to be hosted elsewhere should use the Drupal Composer [Drupal Project](https://github.com/drupal-composer/drupal-project).

**Note:** After cloning one of those base projects, make sure to remove the .git dir and `git init` a new repository for the project.

## Add Contrib Modules
Next, add modules to the composer.json file using the following syntax, where `project_name` is the machine name of the Drupal project.

    composer require drupal/project_name drupal/project_name drupal/project_name

## Add Third Party Libraries
Add any third party libraries needed to the composer.json, so that they are managed by composer.

## Add Drupal Core and Contrib Patches
Add any suggested Drupal core and contrib patches to the composer.json file as well, so that compoer manages applying patches to core and contrib projects.
