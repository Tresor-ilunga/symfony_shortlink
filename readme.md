# Short Link

Application de réduction de liens ddévelopper par  [Tresor Ilunga]

## 👾 Environnement de développement

### 🏁 Pré-requis

* [Symfony CLI](https://symfony.com/download)
* [Docker](https://www.docker.com/)
* [Docker-compose](https://docs.docker.com/compose/install/)
* [PHP 8.1](https://www.php.net/downloads)
* [Composer](https://getcomposer.org/)

### 🔥 Installer le projet en local

Pour les phases de développement, nous utilisons un environnement mixte : Symfony CLI + PHP 8.1 + Docker + Docker-compose

```bash
composer install
docker-compose up -d
symfony serve -d
symfony d:m:m
```

### ✅ Lancer les tests en local

```bash
APP_ENV=test symfony console d:d:c
APP_ENV=test symfony console d:m:m
APP_ENV=test symfony php vendor/bin/phpunit --testdox
```