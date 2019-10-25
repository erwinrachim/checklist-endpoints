# Test Checklists REST API

## how to install
- clone this repo
    ```bash
    git clone https://github.com/erwinrachim/checklist-endpoints.git
    cd checklist-endpoints
    ```
- create `.env` with copy `.env.example` to `.env`
- create database `checklist`
- setting your `.env`
    ```
    DB_DATABASE=checklist
    DB_USERNAME={your_db_user}
    DB_PASSWORD={your_db_password}
    ```
- run composer for install library
    ```bash
    composer install
    ```
- database migrate and seed
    ```bash
    php artisan migrate --seed
    ```
- run app
    ```bash
    php -S localhost:8000 -t public
    ```
## how to access endpoint
- you can use postman or something else
- example endpoint
```bash
    http://localhost:8000/checklists/templates
```


## how to testing
- create database `checklist_tests`
- run tests
    ```bash
    vendor/bin/phpunit
    ```
