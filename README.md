Yii 2 Basic Project Template
============================

Yii 2 Shared Project Template is a skeleton [Yii 2](http://www.yiiframework.com/) application best for
rapidly creating small projects.

The template contains the basic features including user login/logout and a contact page.
It includes all commonly used configurations that would allow you to focus on adding new
features to your application.



REQUIREMENTS
------------

The minimum requirement by this project template that your Web server supports PHP 5.4.0.


### Install via Composer

If you do not have [Composer](http://getcomposer.org/), you may install it by following the instructions
at [getcomposer.org](http://getcomposer.org/doc/00-intro.md#installation-nix).

You can then install this project template using the following command:

~~~
php composer.phar global require "fxp/composer-asset-plugin:~1.1.0"
php composer.phar create-project --prefer-dist cherif/yii2-app-shared shared
~~~

Now you should be able to access the application through the following URL, assuming `shared` is the directory
directly under the Web root.

~~~
http://localhost/shared
~~~


CONFIGURATION
-------------

### Database

Edit the file `config/db.php` with real data, for example:

```php
return [
    'class' => 'yii\db\Connection',
    'dsn' => 'mysql:host=localhost;dbname=yii2basic',
    'username' => 'root',
    'password' => '1234',
    'charset' => 'utf8',
];
```

**NOTES:**
- Yii won't create the database for you, this has to be done manually before you can access it.
- Check and edit the other files in the `protected/config/` directory to customize your application as required.
- Refer to the README in the `tests` directory for information specific to shared application tests.
