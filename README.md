# Framework boilerplate

![My Remote Image](https://laravel.com/img/logomark.min.svg)
![My Remote Image](https://laravel.com/img/logotype.min.svg) v10

# Starter kit powered by Docker dev-box
- `PHP 8.2`
- `MySql`
- `Redis`
- `ElasticSearch`
- `Kibana`
- `Adminer`
- `Nginx`
- `MailPit`

# Repository skeleton

```
.
├── LICENSE
├── README.md
├── docker
│   ├── db    ---> database init sql script
│   ├── nginx ---> nginx server config file for new project
│   ├── php   ---> edit php versions and packages/extensions
│   └── redis ---> redis local beck up
├── docker-compose.yaml ---> edit volumes, ports, etc.
└── src                 ---> put your new projects
    ├── laravel         ---> supported framework
```

# Extensibility and Reusabillity

It's totally up to you to make replasements
- for example `MySQL` -> `PgSql` or `MongoDB` 
- for example `MailPit` -> `MailHog`
- even to make a clean up to suttesfly your needs.

# PHP version upgrade

The change is trivial and is located [here](https://github.com/sports-match-maker/docker-pnmamhes/blob/main/docker/php/Dockerfile)

`FROM php:8.1-fpm` to `FROM php:8.2-fpm` or `FROM php:7.4-fpm`
