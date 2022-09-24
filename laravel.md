### Q. ***What is Facades used in Laravel?***

The facade pattern is a software design pattern that is often used in object-oriented programming.

A facade is a class wrapping a complex library to provide a simpler and more readable interface to it.
Facades in Laravel

Facades provide a "static" interface to classes that are available in the application's service container. Laravel ships with many facades which provide access to almost all of Laravel's features. Laravel facades serve as "static proxies" to underlying classes in the service container, providing the benefit of a terse, expressive syntax while maintaining more testability and flexibility than traditional static methods.

How Facades Are implemented in Laravel

Every service inside the container has a unique name. In a Laravel application, to access a service directly from the container, we can use the App::make() method or the app() helper function.

In Laravel, all services have a facade class. These facade classes extend the base Facade class which is part of the Illuminate/Support package. The only thing that they need to implement is the getFacadeAccessor method, which returns the service name inside the container.



### Q. ***What is Composer?***

Composer is the package manager for the framework. It helps in adding new packages from the huge community into your laravel application.


### Q. ***What is the templating engine used in Laravel?***

The templating engine used in Laravel is Blade. The blade gives the ability to use its mustache-like syntax with the plain PHP and gets compiled into plain PHP and cached until any other change happens in the blade file. The blade file has .blade.php extension.


### Q. ***What are available databases supported by Laravel?***

The supported databases in laravel are:

    PostgreSQL
    SQL Server
    SQLite
    MySQL


### Q. ***What is an artisan?***

Artisan is the command-line tool for Laravel to help the developer build the application. 


### Q. ***What are Models?***

With Laravel, each database table can have a model representation using a model file which can be used to interact with that table using Laravel Eloquent ORM.

### Q. ***What are Events in Laravel?***

In Laravel, Events are a way to subscribe to different events that occur in the application. We can make events to represent a particular event like user logged in, user logged out, user-created post, etc. After which we can listen to these events by making Listener classes and do some tasks like, user logged in then make an entry to audit logger of application.


### Q. ***What are Requests in Laravel?***

Requests in Laravel are a way to interact with incoming HTTP requests along with sessions, cookies, and even files if submitted with the request.

### Q. ***How to do request validation in Laravel?***

Request validation in laravel can be done with the controller method or we can create a request validation class that holds the rules of validation and the error messages associated with it.



Service Container or IoC in laravel is responsible for managing class dependencies meaning not every file needs to be injected in class manually but is done by the Service Container automatically. Service Container is mainly used in injecting class in controllers like Request object is injected. We can also inject a Model based on id in route binding.

### Q. ***What is a Service Provider?***

A Service Provider is a way to bootstrap or register services, events, etc before booting the application. Laravel’s own bootstrapping happens using Service Providers as well. Additionally, registers service container bindings, event listeners, middlewares, and even routes using its service providers.

If we are creating our application, we can register our facades in provider classes. 

### Q. ***What is the register and boot method in the Service Provider class?***

The register method in the Service Provider class is used to bind classes or services to the Service Container. It should not be used to access any other functionality or classes from the application as the service you are accessing may not have loaded yet into the container.


### Q. ***What is Middleware and how to create one in Laravel?***

Middleware gives developers the ability to inspect and filter incoming HTTP requests of our application. One such middleware that ships with laravel are the authentication middleware which checks if the user is authenticated and if the user is authenticated it will go further in the application otherwise it will throw the user back to the login screen.

### Q. ***What is dependency Injection in Laravel?***

The Laravel Service Container or IoC resolves all of the dependencies in all controllers. So we can type-hint any dependency in controller methods or constructors. The dependency in methods will be resolved and injected in the method, this injection of resolved classes is called dependency Injection.

### Q. ***What are collections?***

Collections in laravel are a wrapper over an array of data in Laravel. All of the responses from Eloquent ORM when we query data from the database are collections (Array of data records).

Collections give us handy methods over them to easily work with the data like looping over data or doing some operation on it.

### Q. ***What are contracts?***

Laravel Contracts are a set of interfaces with implementation methods to complete the core tasks of Laravel.


### Q. ***What are queues in Laravel?***

While building any application we face a situation where some tasks take time to process and our page gets loading until that task is finished. One task is sending an email when a user registers, we can send the email to the user as a background task, so our main thread is responsive all the time. Queues are a way to run such tasks in the background.

### Q. ***What are accessors and mutators?***


Accessors are a way to retrieve data from eloquent after doing some operation on the retrieved fields from the database. For example, if we need to combine the first and last names of users but we have two fields in the database, but we want whenever we fetch data from eloquent queries these names need to be combined.


