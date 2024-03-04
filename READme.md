## Local environment setup - Lando

This repository is set up with a `.lando.yml` file, which allows you to use Lando instead of pygmy for your local development environment.

1. [Install Lando](https://docs.lando.dev/basics/installation.html#system-requirements).

2. Install dependencies:

 ```bash
lando composer install
```

3. We already have a Lando file in this repository, so we just need to run the following command to get Lando up:

 ```bash
lando start
```

4. Install your Drupal site with Drush:

```bash
lando drush site:install --db-url=mysql://drupal8:drupal8@database/drupal8 -y
```
