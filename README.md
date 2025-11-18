# Docker Stack 

Docker Development environment

Features
 - **Portainer** - Visual docker manager , Docker GUI 
 - **Traefik** - Reverse proxy with load balancing
 - It has most of useful services @see components bellow
 - container data are persisted into local `/data` folder inside each component folder 
  
Components
 - **portainer**
     - http://portainer.loc/ 
     - credentials made when first run
 - **traefik** - proxy - for nice URL access
     - http://traefik.loc/
 - **redis** - key value storage
    - http://redis.loc/
 - **rabbitmq** - qeue system with admin
     - http://rabbitmq.loc/
     - credentials:  admin : rabbitmq
 - **Kibana** - GUI for ElasticSearch 
    - http://kibana.loc/
 - **Cerebro** - GUI for ElasticSearch cluster
     - http://cerebro.loc/
 - **whoami** - container for testing proxy - response is container_name
    - http://whoami.loc/  
 - Feel free to add others
     
## Start

Starting docker stack 
```
cd docker-stack
docker-compose up -d
```

starting component
```
cd docker-stack/{component}
docker-compose up -d
```

###  How to redirect all  `*.loc` domains to localhost

[dnsmasq with homebrew guide](https://medium.com/@kharysharpe/automatic-local-domains-setting-up-dnsmasq-for-macos-high-sierra-using-homebrew-caf767157e43)  
or  [dnsmasq-dev-osx guide](https://passingcuriosity.com/2013/dnsmasq-dev-osx/)


@author: daniel.kouba@mallgroup.com
