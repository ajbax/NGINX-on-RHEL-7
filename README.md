# NGINX-on-RHEL-7
Deploy NGINX Reverse Proxy on RHEL 7
## FROM YOUR RHEL Server - enable Red Hat Software Collections (RHSCL)

## The command below enable RHSCL ##
sudo yum-config-manager --enable rhel-server-rhscl-7-rmps

## Next step is to install NGINX - use the command below:
sudo yum install rh-nginx18

## Start using RHEL Software Collection:
sudo scl enable rh-nginx18 bash

## Start NGINX service
sudo systemctl start rh-nginx18-nginx

## Configure NGINX to start at boot
sudo systemctl enable rh-nginx18-nginx

