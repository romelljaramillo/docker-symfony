# docker-symfony

This repository contains all the code explained in this [**YouTube playlist**](https://www.youtube.com/playlist?list=PLWpsZlKx38t9SEQu6_AbzBoHeQbApIcjJ)

### Scripts

\*Using **Makefile\***: https://makefiletutorial.com/

Installs composer dependencies

```shell
make prepare
```

Build the containers

```shell
make build
```

Start the containers

```shell
make run
```

Stop the containers

```shell
make stop
```

Restart the containers

```shell
make restart
```

### Steps to follow

Init the bash shell into the **Backend container**

### Install Symfony

```shell
make ssh-be
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
symfony new proyect-symfony
ln -s proyect-symfony/public public
```

### Si ya tenemos symfony en el proyecto

```shell
make ssh-be
```

Update packages

```shell
composer update
```

Install packages

```shell
composer install
```
