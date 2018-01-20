# fmg-setup-env

This post leads you through the steps to create a program that uses the BigQuery API. In this case, the program is an installed application.
It shows you how to:
- Get the json secrets file for an installed application.
- Add the BigQuery Client Library API to your application 
- In the code:
    - get the user’s permission to use the BigQuery API
    - store the credentials if you don’t want to get permission every time the program runs
    - get the Bigquery service
    - issue the query request to the Bigquery service
    - process the results
    
> Configuration
- 4 VMs on google compute Engine (3 VM for Hadoop Cluster and 1 VM for data backup and micro services)
- OS: CentOS 7
- RAM: 15 Go
- CPU: 4
- Boot disk: 200Go
- Attached disk: 2000G

> Cluster model

![MetaStore remote database](https://github.com/gamboabdoulraoufou/hdp-1-host-config/blob/master/img/archi_v2.png)

  
> Log as root on all VM and change root password `_All nodes_`  
```sh 
# log as root
sudo su - root

# change root password
passwd # set password
``` 
