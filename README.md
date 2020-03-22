# Wordpress Project Starter

This repository should be used as a base for creating a new wordpress project. It's designed to be used with GIT and to be developed with a team. Only the development files are included in GIT.

* Plugins/themes managed by **Composer**.
* WordPress Core managed by **WP CLI**.

## Getting started

1. Clone this repository.
1. Run `composer install`.
1. Run `yarn run setup`.
1. Configure site from wp-config.php. See an example wp-config.php that fits this project.

## Database management

As WordPress uses the database for data storage, it's requires additional management. The database shoudn't be stored in GIT. You can either:

1. Use a local mysql database.
1. Use lando.
1. Use docker.

To export or import data from one site to another (eg. local -> pre-live), you can use WP CLI. I've found it to be the fastest and most reliable. To make it work seamlessly, define `WP_HOME` and `WP_SITEURL` in wp-config.php or use [wp-cli again](https://wordpress.org/support/article/changing-the-site-url/#wp-cli)!
