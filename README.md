# laravel-chat

## Getting Started

Clone the project repository

After cloning,run:

```bash
composer install
```

Duplicate `.env.example` and rename it `.env`

Then run:

```bash
php artisan key:generate
```

### Prerequisites

#### Setup Pusher

If you don't have one already, create a free Pusher account at [https://pusher.com/signup](https://pusher.com/signup) then login to your dashboard and create an app.

Set the `BROADCAST_DRIVER` in your `.env` file to **pusher**:

```txt
BROADCAST_DRIVER=pusher
```

Then fill in your Pusher app credentials in your `.env` file:

```txt
PUSHER_APP_ID=xxxxxx
PUSHER_APP_KEY=xxxxxxxxxxxxxxxxxxxx
PUSHER_APP_SECRET=xxxxxxxxxxxxxxxxxxxx
PUSHER_APP_CLUSTER=
```

#### Database Migrations

Be sure to fill in your database details in your `.env` file before running the migrations:

```bash
php artisan migrate
```

And finally, start the application:

```bash
php artisan serve
```

and visit [http://localhost:8000/](http://localhost:8000/) to see the application in action.

## Built With

* [Pusher](https://pusher.com/) - APIs to enable devs building realtime features
* [Laravel](https://laravel.com) - The PHP Framework For Web Artisans
* [Vue.js](https://vuejs.org) - The Progressive JavaScript Framework

## Demo
http://laravel-chat-apps.herokuapp.com/register
