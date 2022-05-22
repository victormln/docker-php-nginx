# Introduction

Template repository to have PHP 8.1 + nginx available through a local URL: https://web-server.test

## Installation

1. From composer

```shell
$ composer require victormln/docker-php-nginx your-project
```

OR with git:

```shell
$ git clone https://github.com/victormln/docker-php-nginx.git your-project
```

2. Install repository

```shell
$ cd your-project
$ make install # It will ask you for your sudo password in order to add to your /etc/hosts the domain
```

3. Start web server:

```shell
$ make start
```

Test website: `https://web-server.test` (you will see all `phpinfo()`)