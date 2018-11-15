
# Github Commands:
        $ git clone  git@github.com:mygitname/theproject.git --branch 2.1.1
        
        git clone git@gitlab.com:rahat/indianfood.git
        git remote add origin git@gitlab.com:rahat/indianfood.git
        git push github

        git commit -m "Commit message"

# Git Workflow of Development branch:
        git branch dev
        git add *
        git commit -m "My initial commit message"
        git push -u origin dev

# Merging all the changes on the development branch into the master:
        git checkout master 
        git merge dev
        git push -u origin master

# View all the differences between branches:
        git diff master..dev
# List files that are different between branches:
        git diff --name-status master..dev

# I always do this if I forget to add a file or do a change.
## Remember to specify --soft instead of --hard, otherwise you lose that commit entirely.
        git reset --soft HEAD~1
        git commit -m 'New and corrected commit message'
        git push -f

# This will tell git you want to start ignoring the changes to the file
        git update -index --assume-unchanged path/to/file
## When you want to start keeping track again
        git update-index --no-assume-unchanged path/to/file

Ubuntu Server Commands:
        sudo chmod 766 -R /var/www/html
        Defaults: drwxr-xr-x  3 root root 4096 অক্টো  22 19:55 html
        
# Composer write permission error solving:
        sudo chown -R $USER $HOME/.composer

# Create Specific version of a package from composer
        composer create-project laravel/laravel=4.1.27 your-project-name --prefer-dist