# elastic_stack

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

Install & Change default editor to vim
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
   
   	wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch | sudo apt-key add -
   
   	sudo apt-get install apt-transport-https

   	echo "deb https://artifacts.elastic.co/packages/6.x/apt stable main" | sudo tee -a /etc/apt/sources.list.d/elastic-6.x.list
   
   	sudo apt-get update && sudo apt-get install elasticsearch

   	sudo /bin/systemctl daemon-reload

   	sudo /bin/systemctl enable elasticsearch.service

   	sudo systemctl start elasticsearch.service

   	sudo systemctl stop elasticsearch.service

   Test if the elasticsearch service is up or not:
   -----------------------------------------------

   	curl -XGET 'localhost:9200/?pretty'

   Basic elasticsearch configuration:
   ----------------------------------

   	$ES_HOME : /usr/share/elasticsearch

   	elasticsearch/elasticsearch-plugin : /usr/share/elasticsearch/bin

   	elasticsearch.yml : /etc/elasticsearch

   	conf : /etc/default/elasticsearch

   	data : /var/lib/elasticsearch   path.data

   	logs : /var/log/elasticsearch   path.logs

   	plugins : /usr/share/elasticsearch/plugins  path.repo






   
