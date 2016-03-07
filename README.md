
# Gitignore collection files

See [my original blog article in french](http://t.bondois.info) for more détails

## Usage

# Method 1 : download content

Being in your project root path, type in console command :

PHP projects (main rules) :

php -r "readfile('https://raw.githubusercontent.com/tbondois/gitignore/master/php.gitignore');" >> .gitignore

Additional rules for Symfony / Silex :

php -r "readfile('https://raw.githubusercontent.com/tbondois/gitignore/master/symfony2.gitignore');" >> .gitignore

Additional rules for Laravel / Lumen :

php -r "readfile('https://raw.githubusercontent.com/tbondois/gitignore/master/laravel.gitignore');" >> .gitignore

Additional rules for Magento 1 :

php -r "readfile('https://raw.githubusercontent.com/tbondois/gitignore/master/magento1.gitignore');" >> .gitignore

Additional rules for Magento 2 :

php -r "readfile('https://raw.githubusercontent.com/tbondois/gitignore/master/magento2.gitignore');" >> .gitignore

Additional rules for Wordpress 4 :

php -r "readfile('https://raw.githubusercontent.com/tbondois/gitignore/master/wordpress4.gitignore');" >> .gitignore
