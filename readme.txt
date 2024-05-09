*****************************************************************************
 ----------------------------- INSTALL SCRIPT ------------------------------
*****************************************************************************
 Run this script from within the public_html folder ** replace the 
 test-install with the name you want for the parent folder of your site.
 
 This script will create the parent folder for your drupal site.
 
 Run this script before you create the subdomain

mkdir test-install && cd test-install && git clone https://github.com/vincenisly/installer.git && mv installer/composer.json ./ && find ./installer -type f -and ! \( -iwholename '*.cgi' -or -iwholename '*.pl' \) -exec chmod 644 '{}' ';' && rm -r installer && composer install && composer update

****************************************************************************
 ------- If you already created your parent folder, run this script -------
****************************************************************************

git clone https://github.com/vincenisly/installer.git && mv installer/composer.json ./ && find ./installer -type f -and ! \( -iwholename '*.cgi' -or -iwholename '*.pl' \) -exec chmod 644 '{}' ';' && rm -r installer && composer install && composer update