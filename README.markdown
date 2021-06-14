# Symfony UX Turbo Demo Application

This barebones chat application serves to demonstrate how Symfony UX Turbo can be used to make server-rendered applications more dynamic without resorting to custom JavaScript code.

Developed for my talk at the [Symfony User Group Aveiro](https://www.meetup.com/sfugaveiro/events/277418939/).

Disclaimer: The code doesn't always adhere to best practices, in favor of keeping the code as simple as possible.

## Requirements

- PHP 8.0 (with SQLite drivers)
- Node + Yarn
- Symfony CLI (with TLS support for the local web server)

## Setup

1. Install dependencies: `composer install` & `yarn`
2. Create the database with the matching schema: `bin/console doctrine:schema:update --force`
3. Run `make start` to start the dev server and Webpack Encore.
4. Open up `https://127.0.0.1:8000/rooms` to get started!

> NOTE: It has to be `https://127.0.0.1:8000`. Anything else (even `localhost:8000`) will result in CORS errors when attempting to connect to the Mercure Hub.

## Notes

Turbo Frames are given red borders while Turbo Streams are given blue borders to better identify them.
