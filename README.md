# Adonis Ticketing

> Basic ticketing app built with Adonisjs.

## Setup

Run the command below to install dependencies

```bash
$ npm install
```

### Environment variables

Duplicate `.env.example` and rename it `.env`

### Migrations

To setup your database. Create a `adonis.sqlite` file in the database folder.

To setup e-mail functionality you can create a [Mailtrap](https://mailtrap.io/) account. From the Mailtrap settings you can copy the port, username and password.

Enter the following in `.env` file

```
HOST=127.0.0.1
PORT=99
NODE_ENV=development
APP_NAME=Adomail
APP_URL=http://${HOST}:${PORT}
CACHE_VIEWS=false
APP_KEY=
DB_CONNECTION=sqlite
DB_DATABASE=adonis
HASH_DRIVER=bcrypt
MAIL_HOST=smtp.mailtrap.io
MAIL_PORT=2525
MAIL_USERNAME=
MAIL_PASSWORD=
```

Run this command to generate a key for the app.

```bash
$ adonis key:generate
```

Run the following command to run migration.

```bash
$ adonis migration:run
```

Seed the database:

```bash
$ adonis seed
```

Finally, start the application:

```bash
$ adonis serve --dev
```

### To-Do

- [x] Fix unable to comment bug
- [ ] Fix invalid login exceptions
- [ ] Fix ticket link sent via e-mail
- [ ] Fix navbar extending over viewport
- [x] Fix variables appearing in admin actions column

&#9888; This project is not finished. It is work in progress **(WIP)!** &#9888;
