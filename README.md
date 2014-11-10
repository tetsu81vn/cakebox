Cakebox
=======

One Box, All Cakes.

# Notes

- filemode caching will log everything (including errors() to /var/log/app ==> not recommended, better use Redis or Memcached

# TODO

### General

- new: replace bash with php-cli
- bug: use setfacl for cakephp2 and foc2 (and foc3) /tmp permissions
- bug: add ruby file-detector to Cakebox.yaml.examples
- foc: install suggested Search plugin???
- new: warn if no Cakebox.yaml is found? (load default settings first?)
- new: long args so we can shorten cakebox-command (e.g. cakebox-app URL, everything else as argument)
- new: enable Vagrantfile.rb environment variables
- new: check -e Cakebox.yaml in Vagrantfile
- bug: foc3 template broken ==> looks in wrong dir for bootstrap.php (https://github.com/FriendsOfCake/app-template/issues/58)
- bug: cakephp3 test-database configuration uses prod-settings ==> depends on decent bash argument parsing
- bug: add vagrant to /var/log/nginx


## cakebox site

- ssl support (generate cert)

### cakebox database

- add option -o --overwrite        Otherwise leave untouched

### cakebox database

- change default username/password
- add option d, --drop database    Drop database, otherwise skip if exist

### YAML

- configure global git user (email, password, options)
-



### Maybe
- add bash colouring scheme?
- remote (Git hosted?) Cakebox.yaml

# DOCS
- describe vagrant_private_key.pkk
- uses https://github.com/ulrichsg/getopt-php
