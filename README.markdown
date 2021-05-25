# Symfony UX Turbo Demo Application

This barebones chat application serves to demonstrate how Symfony UX Turbo can be used to make server-rendered applications more dynamic without resorting to custom JavaScript code.

Developed for my talk at the [Symfony User Group Aveiro](https://www.meetup.com/sfugaveiro/events/277418939/).

Disclaimer: The code doesn't always adhere to best practices, in favor of keeping the code as simple as possible.

## Requirements

- PHP 8.0
- Node + Yarn
- Symfony CLI

## Setup

1. Install dependencies: `composer install` & `yarn`
2. Run `make start` to start the dev server and Webpack Encore.
3. Open up `127.0.0.1:8000/rooms` to get started!

> NOTE: It has to be `127.0.0.1:8000`. Anything else (even `localhost:8000`) will result in CORS errors when attempting to connect to the Mercure Hub.
