# What is this?

CakePHP environment on Nginx + PHP-FPM + MySQL on Docker.

# Installation and Setting

## 1. Make directory which installing CakePHP

```
$ mkdir app
```

## 2. Install CakePHP

```
$ docker-compose run --rm composer create-project --prefer-dist cakephp/app .
```

## 3. Create MySQL environment file and edit it

```
$ cp docker/mysql/.env.sample docker/mysql/.env
$ vim docker/mysql/.env
```

# Startup

```
$ docker-compose up -d nginx
```

# Installation of additional package

## 1. Edit `composer.json`

```
$ vim app/composer.json
```

## 2. Install additional package

```
$ docker-compose run --rm composer install
```
