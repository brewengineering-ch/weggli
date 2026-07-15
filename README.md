# weggli

## Local development

After cloning the repository, install the PHP and frontend dependencies:

```bash
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
npm install && npm run build
```

Start the local development environment:

```bash
composer run dev
```

This command starts the Laravel development server, queue worker, log tailing, and Vite.

## Updating dependencies

Rerun dependencies only when they change:

- Run `composer install` when `composer.lock` changes.
- Run `npm install` when `package.json` or `package-lock.json` changes.

## Notes

- In this devcontainer setup, `composer run dev` binds Laravel to `0.0.0.0:8000` so the app is reachable through VS Code port forwarding.
- During normal day-to-day development, you typically only need to rerun `composer run dev`.
