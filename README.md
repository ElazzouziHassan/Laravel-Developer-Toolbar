# Laravel Developer Toolbar :
---

Laravel Developer Toolbar is a package that provides useful information and insights about your Laravel application during development. It displays information about the routes, views, events, queries, and more, making it easier to debug and optimize your application.

To install Laravel Developer Toolbar, you can use Composer, which is the default package manager for Laravel. Here are the steps to install it :

* Open the terminal or command prompt and navigate to your Laravel project directory.
* Run the following command to install the package:

```bash
composer require barryvdh/laravel-debugbar --dev
```

* After the installation is complete, add the following line to the `providers` array in the `config/app.php` file :
```php
Barryvdh\Debugbar\ServiceProvider::class,
```
* Next, add the following line to the `aliases` array in the same file :
```php
'Debugbar' => Barryvdh\Debugbar\Facade::class,
```
* Finally, run the following command to publish the configuration file :
```bash
php artisan vendor:publish --provider="Barryvdh\Debugbar\ServiceProvider"
```
You can now access the Laravel Developer Toolbar by opening your Laravel application in a web browser and appending `/debugbar` to the URL. For example :
```bash
http://localhost:8000/debugbar
```
That's it! You should now see the Laravel Developer Toolbar in your application's page. 

***
@by : [Wizardy](https://github.com/ElazzouziHassan "El azzouzi Hassan")
