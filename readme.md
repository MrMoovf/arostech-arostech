# Aros Tech CMS

## Welcome to the updating guide


## Welcome to the installation guide

### Please use the following commands
After you have installed your laravel application

```cd path/to/project```

``composer install ``

``composer require arostech/arostech ``

``php artisan vendor:publish --tag=migrations ``

``php artisan migrate``

``php artisan route:cache``

``php artisan view:cache``

``php artisan config:clear``

``npm run build``

### Then configure your .env-file
```
APP_NAME={{your_appname}}
APP_ENV={{either: 'local' | 'production'}}
APP_KEY={{configured_by_laravel}}
APP_DEBUG=true
APP_TIMEZONE=UTC
APP_URL={{your_app_url}}
APP_OWNER_NAME={{your_app_owner_name}}

IS_NEXT_JS_APP={{true if next.js app}}
VERCEL_FRONTEND_TOKEN={{your_vercel_token}}
VERCEL_FRONTEND_DEPLOYMENT_ID={{your_vercel_deployment_id}}
VERCEL_FRONTEND_NAME={{your_vercel_frontend_name}}

AROSTECH_USERNAME={{your_arostech_username}}
AROSTECH_PASSWORD={{your_arostech_password}}

APP_LOCALE=en
APP_FALLBACK_LOCALE=en
APP_FAKER_LOCALE=en_US

APP_MAINTENANCE_DRIVER=file
APP_MAINTENANCE_STORE=database

BCRYPT_ROUNDS=12

LOG_CHANNEL=stack
LOG_STACK=single
LOG_DEPRECATIONS_CHANNEL=null
LOG_LEVEL=debug

DB_CONNECTION=mariadb
DB_HOST={{either: '127.0.0.1' | 'your_server_ip'}}
DB_PORT={{either: '3306' | 'your_db_port'}}
DB_DATABASE={{your_db_name}}
DB_USERNAME={{your_db_username}}
DB_PASSWORD={{your_db_password}}

SESSION_DRIVER=database
SESSION_LIFETIME=120
SESSION_ENCRYPT=false
SESSION_PATH=/
SESSION_DOMAIN=null

BROADCAST_CONNECTION=log
FILESYSTEM_DISK=local
QUEUE_CONNECTION=database

CACHE_STORE=database
CACHE_PREFIX=

MEMCACHED_HOST=127.0.0.1

REDIS_CLIENT=phpredis
REDIS_HOST=127.0.0.1
REDIS_PASSWORD=null
REDIS_PORT=6379

#Change to bg@gr888.dk
MAIL_OWNERS_EMAIL={{the_website_owners_contact_email}} 
MAIL_MAILER=smtp
MAIL_HOST=secure.emailsrvr.com
MAIL_PORT=465
MAIL_USERNAME={{your_email_username}}
MAIL_PASSWORD={{your_email_password}}
MAIL_ENCRYPTION=ssl
MAIL_FROM_ADDRESS={{the_website_owners_contact_email}}
MAIL_FROM_NAME="${APP_NAME}"

AWS_ACCESS_KEY_ID=
AWS_SECRET_ACCESS_KEY=
AWS_DEFAULT_REGION=us-east-1
AWS_BUCKET=
AWS_USE_PATH_STYLE_ENDPOINT=false

VITE_APP_NAME="${APP_NAME}"

```

### The API is now installed and configured correctly
