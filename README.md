# Journal

## Installation & Configuration

### Laravel
1. Open Project jurnal
- Setup Installation
    1. Open terminal with path the project
    2. Run `composer install`
    3. Run `npm install`
    4. Run `npm run dev`

- Setup Environtment
    1. Duplicate `.env.example`
    2. Rename to `.env`
    3. Run `php artisan key:generate`
    4. Setup `.env`
        ```env
        DB_CONNECTION=mysql
        DB_HOST=127.0.0.1
        DB_PORT=3306
        DB_DATABASE=yourdatabase
        DB_USERNAME=yourusername
        DB_PASSWORD=yourpassword
        
        ```
        > Don't forget to create database in MySQL

- Setup Project
    1. Open terminal with path the project
    2. Run `php artisan migrate:fresh`
    3. Run `php artisan db:seed --class=RoleTableSeeder`
    4. Run `php artisan db:seed --class=AdminSeeder`
    5. Run `php artisan db:seed --class=StatusSeeder`
    6. Run `php artisan db:seed --class=HeadlineSeeder`
    7. Run `php artisan serve`
    8. Open the url
