# Woocommerce Docker Compose

Docker compose configuration for Woocommerce development. Comes bundled with a phpMyAdmin instance for db inspect and debug.

## Requirements

- Docker 1.13.0+

## Setup

- Clone or download the repo
- `docker-compose up`
- Go to https://localhost:8090 an follow the install process.
- Install Woocommerce:
  - Go to: Plugins > Add New.
  - Search for 'WooCommerce'.
  - Select Install Now when you see it's by Automattic.
  - Select Activate Now and follow the Woocommerce wizard.

## Running

```bash
docker-compose up
```

Or in detached mode:

```bash
docker-compose up -d
```

Go to http://localhost:8090 to see the site. Admin is on http://localhost:8090/wp-admin. Credentials are what you define on installation.

Woocommerce files are in `wp-app/`

phpMyAdmin is on http://localhost:8091. Credentials: *user*: `root`, *password*: `password`

