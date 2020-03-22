# WordPress Project Starter

This repository should be used as a base for creating a new wordpress project. It's designed to be used with GIT and to be developed with a team. Only the development files are included in GIT.

* **Composer** for plugins and theme management.
* **PHP CodeSniffer** for code that follows WordPress standards.
* **WP CLI** for WordPress Core management.

This starter project should be built upon to fit your project! For exmaple: gulp for assets and styles, CI/CD configuration.

## Getting started
See [prerequisites](#prerequisites) below.

1. Clone this repository.
1. Run `composer install`.
1. Run `yarn run setup`.
1. Configure site from wp-config.php. See an example wp-config.php that fits this project.

## Database management

As WordPress uses the database for data storage, it's requires additional management. The database shoudn't be stored in GIT. You can either:

1. Use a local mysql database.
1. Use lando.
1. Use docker.

To export or import data from one site to another (eg. local -> pre-live), you can use WP CLI. I've found it to be the most reliable. To make it work seamlessly, define `WP_HOME` and `WP_SITEURL` globals or use [wp-cli again](https://wordpress.org/support/article/changing-the-site-url/#wp-cli)!

## Prerequisites

1. [WP CLI](https://wp-cli.org/)
1. [Composer](https://getcomposer.org/)
1. [Yarn](https://yarnpkg.com/)
