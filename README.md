# elasticsearch_stack

Install jdk8 and jre8
---------------------
sudo su -
apt-get update && apt-get upgrade

sudo apt-get install default-jre

sudo apt-get install default-jdk

Install Postman on Ubuntu
-------------------------

wget https://dl.pstmn.io/download/latest/linux64 -O postman.tar.gz

sudo tar -xzf postman.tar.gz -C /opt

rm postman.tar.gz

sudo ln -s /opt/Postman/Postman /usr/bin/postman

Install & Chnage default editor to vim
--------------------------------------
sudo apt install vim

select-editor

Choose the vim editor

Install curl
-------------

sudo apt install curl

Install the following Elastic stack technologies & Configure them
-----------------------------------------------------------------
1. Elasticsearch
