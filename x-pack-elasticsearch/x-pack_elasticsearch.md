Installing X-Pack in Elasticsearch
----------------------------------
  
  cd to /usr/share/elasticsearch/

  Execute command & allow security
  --------------------------------

    bin/elasticsearch-plugin install x-pack

    Confirm that you want to grant X-Pack additional permissions

    Stop elasticsearch: sudo systemctl stop elasticsearch.service

    Start elasticsearch: sudo systemctl start elasticsearch.service

  Set interactive password for elasticsearch,kibana,logstash
  ----------------------------------------------------------

    bin/x-pack/setup-passwords interactive
    

    