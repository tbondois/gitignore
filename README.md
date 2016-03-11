# Smart Gitignore rules for PHP projects

This is a model of .gitignore file for your PHP project. It differs from other models you can see, in GitHub for example, because of the use of regular expressions and exceptions, making the file shorter and the rules smarter and more adaptative to any kind of projects.

French users : [my original french article](http://t.bondois.info/gitignore) for more détails.


# Method 1 : download content by PHP-CLI/SAPI

If you have local HTTP server with PHP-CLI/SAPI running, being in your project root path, type in console command :

* PHP projects (main rules) :

`php -r "readfile('https://raw.githubusercontent.com/tbondois/gitignore/master/php.gitignore');">>.gitignore`

* Additional rules for Symfony 2,3, Silex, Oro Platform, AkeneoPIM :

`php -r "readfile('https://raw.githubusercontent.com/tbondois/gitignore/master/symfony2.gitignore');">>.gitignore`

* Additional rules for Laravel / Lumen :

`php -r "readfile('https://raw.githubusercontent.com/tbondois/gitignore/master/laravel.gitignore');">>.gitignore`

* Additional rules for Magento 2 :

`php -r "readfile('https://raw.githubusercontent.com/tbondois/gitignore/master/magento2.gitignore');">>.gitignore`


* Additional rules for Magento 1 :

`php -r "readfile('https://raw.githubusercontent.com/tbondois/gitignore/master/magento1.gitignore');">>.gitignore`

or `php -r "readfile('https://raw.githubusercontent.com/github/gitignore/master/Magento.gitignore');">>.gitignore` if you want to exclude all core files from your repository.


* Additional rules for Wordpress 4 :

`php -r "readfile('https://raw.githubusercontent.com/tbondois/gitignore/master/wordpress4.gitignore');">>.gitignore`

