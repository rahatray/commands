# Search for a composer package
    $ composer search indianfood

# Install a specific version of a package via composer:
    $ composer require indianfood/indianfood:v3.0.4-beta.5
    
# these conflict with your requirements or minimum-stabilitym arose, add these two lines at the end of "composer.json" file, before the closing brace:
    ,
  "minimum-stability": "dev",
  "prefer-stable": true

# To clear the composer cache just run the following:
    $ composer clearcache
