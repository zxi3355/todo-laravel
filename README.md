## Clone and start the application

_Please make sure you have docker desktop installed and running before proceeding._

```
git clone git@github.com:zxi3355/todo-laravel.git
cd todo-laravel
./vendor/bin/sail up
```

## Seed the application

Open another terminal window and run the following command. This will create 5 todos in the mysql database

```
./vendor/bin/sail artisan migrate --seed
```

## Use postman to talk the public to do API

Import the postman collection from file todo_api.postman_collection.json in the root folder. It contains CRUD operations together will some basic request validation.
