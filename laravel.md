
# download the Laravel installer using Composer:
    $ composer global require laravel/installer
# Install Laravel via Laravel Installer
    $ laravel new indianfood

# download installer
composer global require "laravel/installer=~1.1"

# setting up path
export PATH="~/.composer/vendor/bin:$PATH" 

# check laravel command
laravel 

# download installer
composer global require "laravel/installer=~1.1"

nano ~/.bashrc

#add

alias laravel='~/.composer/vendor/bin/laravel'

source ~/.bashrc

laravel

# going to html dir to create project there
cd /var/www/html/
# install project in blog dir.
laravel new blog

# Install specific laravel framework by composer:
composer create-project laravel/laravel indianfood  "5.5.*" --prefer-dist

# Copy .env.example to .env:

    $ cp -a .env.example .env

# Generate a key:

    $ php artisan key:generate

# Only then run:

    $ php artisan serve
# Run Laravel autoloader for vendor packages:
    $ composer dumpautoload
# For third party package discover run:
    $ php artisan package:discover
