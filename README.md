# Smart Gitignore rules for PHP projects

This is a model of .gitignore file for your PHP project. It differs from other models you can see, in GitHub for example, because of the use of regular expressions and exceptions, making the file shorter and the rules smarter and more adaptative to any kind of projects.

French users : [my original french article](http://t.bondois.info/gitignore) for more détails.


    
# Method 1 : download content by PHP-CLI/SAPI

If you have local HTTP server with PHP-CLI/SAPI running, being in your project root path, type in console command :

* PHP projects (main rules) :

`php -r "readfile('https://raw.githubusercontent.com/tbondois/gitignore/master/php.gitignore');">>.gitignore`


* Additional rules for Symfony 2, 3, Silex, Oro Platform, AkeneoPIM :

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

## Hint #1 : you can also define global gitignore file for all your project

`git config --edit  --global`

Add (and adapt with the path you want) : 

`[core]
    excludesfile = C:\\Users\\MyUser\\global.gitignore`

## Hint #2 : setup a Unix-style configuration of files for Git and your IDE 

Very useful for PHP developers (production environments are always GNU/Unix family). You can force that in

* In your IDE : you will need a [EditorConfig plugin](http://editorconfig.org/#download) plugged in your IDE for that. Then, always project root path, type in console command :

`php -r "readfile('https://raw.githubusercontent.com/tbondois/gitignore/master/unix.editorconfig');">>.editorconfig`



* In your Git config : type `git config --edit  --global` for global config or `git config --edit` for only a project config. Add/Replace this in your file :

	[core]
	    eol = lf
	    safecrlf = false
	    autocrlf = input
	    whitespace = cr-at-eol


A little offtopic, but if you can also add this in the config file to optimize your git experience :


	[http]
	    postBuffer = 524288000
	[push]
	    default = matching
	[diff]
	    mnemonicPrefix = true
	[credential]
	    # for windows : wincred. linux : store
	    helper = wincred
	[color]
	    ui = auto
	    branch = auto
	    diff = auto
	    interactive = auto
	    status = auto
	[alias]
	    a  = add .
	    st = status
	    ci = commit
	    co = checkout
	    br = branch
	    lg = log --graph --date=relative --pretty=tformat:'%Cred%h%Creset -%C(auto)%d%Creset %s %Cgreen(%an %ad)%Creset'
	    gl = log --oneline --all --graph --decorate
	    oops    = commit --amend --no-edit
	    pusha   = push -vu origin --all
	    pushd   = push -vu origin develop --tags
	    pushm   = push -vu origin master --tags
	    pulld   = pull origin develop
	    pullm   = pull origin master
	    mapd    = branch --set-upstream-to=origin/develop develop
	    mapm    = branch --set-upstream-to=origin/master master




