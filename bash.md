# Permanently edit PATH
    $ sudo nano ~/.bash_profile

# then add, save and restart the terminal:
    export PATH=~/.composer/vendor/bin:$PATH

# If restarting Terminal doesn't work then issue the following command:
    $ source ~/.bash_profile

# N.B: Alternate way is to edit the ".bashrc" similarly.
# To check PATH:
    $ echo $PATH