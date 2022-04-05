## Clone and start the application

_Please make sure you have docker desktop installed and running before proceeding._

```
git clone git@github.com:zxi3355/todo-laravel.git
cd todo-laravel
./vendor/bin/sail up
```

## Run database migration and seed the application

Open another terminal window and run the following command inside the todo-laravel folder. This will create the database tables and add 5 todos to the todos table in the mysql database

```
./vendor/bin/sail artisan migrate --seed
```

## Use postman to talk to the public todo API

Import the postman collection from file todo_api.postman_collection.json in the root folder. It contains CRUD operations together with some basic request validations. For the time being, the title is a required field that should be less than or equal to 50 characters.
