FROM mcr.microsoft.com/devcontainers/php:3-8.5-trixie

# Required by Laravel Pail and some signal-aware CLI workflows.
RUN docker-php-ext-install -j"$(nproc)" pcntl