# ELKStack
* sudo apt-get update
* install docker via sudo apt install docker.io
* install docker-compose via sudo apt install docker-compose
* set {DATA_DIR}, Linux: sudo nano /etc/environment en voeg toe DATA_DIR="/elastisdata" , Windows: setx DATA_DIR "C:\elastisdata" /M
* exit (om omgevingsvariabele te activeren, test met printenv DATA_DIR) 
* sudo mkdir -p ${DATA_DIR}/elasticsearch
* sudo chmod g+rwx ${DATA_DIR}/elasticsearch
* sudo chgrp 0 ${DATA_DIR}/elasticsearch
* sudo mkdir -p ${DATA_DIR}/logstash
* start met docker-compose up -d