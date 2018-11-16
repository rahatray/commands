# Search for a composer package
    $ composer search indianfood

# Install a specific version of a package via composer:
    $ composer require indianfood/indianfood:v3.0.4-beta.5
    
# these conflict with your requirements or minimum-stabilitym arose, add these two lines at the end of "composer.json" file, before the closing brace, don't forget to add a "," before putting these:
  "minimum-stability": "dev",
  "prefer-stable": true

# To clear the composer cache just run the following:
    $ composer clearcache

# Add own github repository in "composer.json":
    "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/rahatray/indianfood"
        }
    ]

# Run the folloing composer command to install the package:
    $ composer require your-github-username/indianfood --dev

# Safe replacement for `composer global require` especially for solving composer dependency problems
    $ composer global require consolidation/cgr
