# Empty Drupal Docksal structure

This project is an empty Docksal project for use with exisiting Drupal code and database.
It creates the default containers for a web project. There is extra configuration to automatically create the correct database import the data.

## Exisiting Code
For Drupal 7 or non Compser Drupal 8 sites copy your exisiting code into the docroot folder.

## Database
Copy and exported database in either .sql or .sql.gz file in the the db folder.

## Environment file
There are changes require for the Docksal environment to meet you specific project.
The most important is creating the corrent database.

1. Copy the `docksal.env` file to `docksal-local.env`.
2. Edit the new `docksal-local.env` file.
3. Change the MYSQL_PORT_MAPPING to a unique mapping for you system following the instructions in the file.
4. Change the `MYSQL_DATABASE`, `MYSQL_USER` and `MYSQL_PASSWORD` values to match the database settings for your Drupal site.

## Edit Drush Alias
Copy the `drush/default.aliases.drushrc.php` to `drush/aliases.drushrc.php`.
Edit the `drush/aliases.drushrc.php` and change the uri value to the uri of your new project.