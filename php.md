# list all of the available PHP 7.0-related packages for review:
    $ apt-cache pkgnames | grep php7.0

# Install PHP 7 and related packages in Ubuntu:
    $ sudo apt-get install -y php7.0 libapache2-mod-php7.0 php7.0-cli php7.0-common php7.0-mbstring php7.0-gd php7.0-intl php7.0-xml php7.0-mysql php7.0-mcrypt php7.0-zip

# Switch between PHP versions for apache web server:
        $ sudo a2dismod php7.0
        $ sudo a2enmod php5.6
        $ sudo systemctl restart apache2
        $ sudo service apache2 restart

# After switching from one version to another, you can find your PHP configuration file, by running the command below.
        $ which php
        $ which php5.6
        $ which php7.3
        $ sudo update-alternatives --set php /usr/bin/php5.6
        $ php -i | grep "Loaded Configuration File"

# PHP built in webserver:
        $ php -S localhost:8000
        
$ To serve public folder of a framework/webapp:        
        $ php -S 0.0.0.0:8080 -t public
