#!/bin/sh

#============================================================
#WORDPRESS KURULUMU

cd ~
wget --no-check-certificate https://wordpress.org/latest.tar.gz
tar xzvf latest.tar.gz
sudo apt-get update
cd ~/wordpress
cp wp-config-sample.php wp-config.php
cd ..
cp wordpress /var/www/html/wp
