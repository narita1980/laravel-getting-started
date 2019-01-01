# laravel-getting-started

A barebones [Laravel 5.7](https://laravel.com/) app.

This application supports the [Getting Started with Laravel on Heroku](https://devcenter.heroku.com/articles/getting-started-with-laravel) article - check it out.

## Running Locally

Make sure you have [Composer](https://getcomposer.org/) and the [Heroku CLI](https://cli.heroku.com/) installed.

```sh
$ git clone https://github.com/narita1980/laravel-getting-started.git # or clone your own fork
$ cd laravel-getting-started
$ composer install
$ mv .env.example .env
$ php artisan key:generate
$ php artisan serve
```

Your app should now be running on [127.0.0.1:8000](http://127.0.0.1:8000).

## Deploying to Heroku

```
$ heroku create
$ git push heroku master
$ heroku config:set APP_KEY=$(php artisan --no-ansi key:generate --show)
$ heroku open
```

## Documentation

For more information about using Laravel on Heroku, see these Dev Center articles:

- [Getting Started with Laravel on Heroku](https://devcenter.heroku.com/articles/getting-started-with-laravel)
- [Scaling a Laravel Application with Memcache](https://devcenter.heroku.com/articles/laravel-memcache)
- [PHP Application Logging](https://devcenter.heroku.com/articles/php-logging#laravel)
- [MemCachier](https://devcenter.heroku.com/articles/memcachier#laravel)
- [Heroku Postgres](https://devcenter.heroku.com/articles/heroku-postgresql#connecting-with-laravel)
- [Stream](https://devcenter.heroku.com/articles/stream#demo-django-rails-and-laravel)
- [Moesif API Insights](https://devcenter.heroku.com/articles/moesif#using-with-php-laravel)
