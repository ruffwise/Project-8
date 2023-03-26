# Project-8: LOAD BALANCER SOLUTION WITH APACHE

### Prerequisites

1. Two RHEL8 Web Servers
2. One MySQL DB Server (based on Ubuntu 20.04)
3. One RHEL8 NFS server

### Install and configure Apache As A Load Balancer

`sudo apt update`

`sudo apt install apache2 -y`

`sudo apt-get install libxml2-dev`

`sudo a2enmod rewrite`

`sudo a2enmod proxy`

`sudo a2enmod proxy_balancer`

`sudo a2enmod proxy_http`

`sudo a2enmod headers`

`sudo a2enmod lbmethod_bytraffic`

#Restart apache2 service

`sudo systemctl restart apache2`
![](/images/apache-status.png)

### configure load balancing

`sudo vi /etc/apache2/sites-available/000-default.conf`
![](/images/loab-balancing-config.png)

![](/images/aws.png)

### log in via load-balancer public IP

![](/images/Login-LB-IP.png)
