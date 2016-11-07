# Doctrine-Migration-Example
I have been working on custom framework of php project where I needed database migration tool to be able to easily apply changes to production and also maintaining schema version. So I did some research and find some examples of Doctrine 2 database migration.

This is what I exactly did to run Doctrine migration tool in custom php framework.

##  Create composer.json
Download Doctrine 2 Migration package via composer


##  Create migrations.yml
Configure your migration to add migration namespace, store migration version in table and store migration classes in directory.


##  Create console.php
This file will:

- Load Doctrine package
- Define database property and set database configuration
- Add more migration commands


## Run(Example):

- `$ php console.php list migrations`
- `$ php console.php --configuration="migrations.yml" migrations:status`
- `$ php console.php --configuration="migrations.yml" migrations:generate`
