# Web-App

Laravel 12 web application starter with authentication scaffolding (Breeze), Vite, and Tailwind CSS.

## Requirements

- PHP 8.2+
- Composer 2+
- Node.js 18+ and npm
- A database (MySQL, PostgreSQL, SQLite, etc.)

## Quick Start

1. Install backend dependencies:

	composer install

2. Create environment file:

	copy .env.example .env

3. Generate app key:

	php artisan key:generate

4. Configure database in .env.

5. Run migrations:

	php artisan migrate

6. Install frontend dependencies:

	npm install

7. Start development servers:

	composer run dev

This starts:
- Laravel app server
- Queue listener
- Log tailing
- Vite dev server

## One-Command Setup

You can also run:

composer run setup

This installs dependencies, prepares .env, generates key, runs migrations, and builds frontend assets.

## Useful Commands

- Run app stack: composer run dev
- Run tests: composer run test
- Build frontend assets: npm run build
- Start Vite only: npm run dev
- Start Laravel only: php artisan serve

## Testing

Run the test suite:

php artisan test

Or with Composer:

composer run test

## Project Structure

- app/Http/Controllers: request handling controllers
- app/Models: Eloquent models
- resources/views: Blade templates
- routes/web.php: web routes
- database/migrations: schema migrations
- tests: feature and unit tests

## Troubleshooting

- If assets do not load, ensure npm run dev is running.
- If migrations fail, verify DB_* values in .env.
- If storage links are needed for uploads, run:

  php artisan storage:link

## License

This project uses the MIT license.
