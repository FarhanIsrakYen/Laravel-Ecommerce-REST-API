Laravel Ecommerce REST API | REST API for E-Commerce platform with admin panel integration.

| [Admin Panel Features][] | [Requirements][] | [Get Started][] | [Env setup][] | [API Documentation][] |

## Admin Panel Features

| Features    | Description                                                   |
| ----------- | ------------------------------------------------------------- |
| Users       | Create employee and manage all users.                         |
| Orders      | Manage the orders.                                            |
| Finances    | Manage the finances.                                          |
| Withdrawals | Manage the merchant's withdraw request.                       |
| Bankings    | Create and manage available banking for merchant.             |
| Categories  | Create and manage available category for merchant's products. |
| Profile     | Edit user's profile and password.                             |

## Requirements

    Laravel = ^9.x
    PHP = ^8.1.x
    kavist/rajaongkir = ^1.x
    midtrans/midtrans-php = ^2.x
    laravel/scout = ^9.x
    filament/filament = ^2.x
    beyondcode/laravel-websockets = ^1.x
    pusher/pusher-php-server = ^7.x
    flowframe/laravel-trend = ^0.1.x
    barryvdh/laravel-debugbar = ^3.x
    laravel-echo = ^1.15.x
    pusher-js = ^8.x

## Get Started

Clone repo

```
git clone https://github.com/FarhanIsrakYen/Laravel-Ecommerce-REST-API.git
```

Composer Installation

[Download Composer](https://getcomposer.org/download/)

composer update/install

```
composer install
```

Install Nodejs

[Download Node.js](https://nodejs.org/en/download/)

NPM dependencies

```
npm install
```

Run Vite

```
npm run dev
```

## Env setup

Go into .env file change Database and Email credentials. Then setup some configuration with your own credentials

```
PUSHER_APP_ID=randomstring
PUSHER_APP_KEY=randomstring
PUSHER_APP_SECRET=randomstring
PUSHER_HOST=127.0.0.1
PUSHER_PORT=6001
PUSHER_SCHEME=https|http   (any)
PUSHER_APP_CLUSTER=mt1

RAJAONGKIR_API_KEY=<Your-API-Key>

MIDTRANS_SERVER_KEY = <Your-Server-Key>
MIDTRANS_PRODUCTION = false
MIDTRANS_SANITIZED = true
MIDTRANS_3DS = true|false   (any)

<!-- If you are using algolia, change the scout_driver and setting your own algolia credentials -->
SCOUT_DRIVER=database

<!-- If you are using laravel valet and https protocol, add your valet path below -->
LARAVEL_WEBSOCKETS_SSL_LOCAL_CERT='/Users/YOUR-USERNAME/.config/valet/Certificates/VALET-SITE.TLD.crt'
LARAVEL_WEBSOCKETS_SSL_LOCAL_PK='/Users/YOUR-USERNAME/.config/valet/Certificates/VALET-SITE.TLD.key'
LARAVEL_WEBSOCKETS_SSL_PASSPHRASE=''

```

Run the migration

```
php artisan migrate
```

Or run the migration with seeder if you want seeding the related data

```
php artisan migrate --seed
```

Generate a New Application Key

```
php artisan key:generate
```

Create a symbolic link

```
php artisan storage:link
```

## API Docs
 # todo: will be added

**[⬆ back to top](#laracommerce-rest-api)**

[Admin Panel Features]: #admin-panel-features
[Requirements]: #requirements
[Get Started]: #get-started
[env setup]: #env-setup
[API Documentation]: #api-docs
