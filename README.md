Ansible ELK Stack [ Financial Service Edition ]
==============================================

Application servers in Financial Services Firms are usually locked down and 
have no access to the internet. This becomes a real pain as there is only the 
default internal RPM repository available and no access to external RPM repositories
to install the ELK stack. This Ansible script allows us to deploy the ELK stack 
with pre-downloaded packages for Elasticsearch, Java, Kibana, Logstash, and 
Nginx.

Prerequisites
-------------
Ensure the following packages are packaged up in roles/files/reporting_pkg.tar.gz

Django-1.8.2.tar.gz                
freetds-0.95.14.tar.gz         
meld3-0.6.5.tar.gz  
Pillow-2.9.0.tar.gz  
Python-2.7.10.tgz     
rptlab-reportlab-5d54c7381247.tar.gz  
SQLAlchemy-1.0.6.tar.gz  
urllib3-1.10.4.tar.gz
elasticsearch-1.7.1.tar.gz         
kibana-4.1.1-linux-x64.tar.gz  
nginx-1.8.0.tar.gz  
pip-7.1.0.tar.gz     
PyYAML-3.11.tar.gz    
server-jre-8u51-linux-x64.tar.gz      
supervisor-3.1.3.tar.gz
elementtree-1.2.6-20050316.tar.gz  
logstash-1.5.3.tar.gz          
pfbfer.zip          
pyodbc-3.0.7.zip     
reporting_pkg.tar.gz  
setuptools-18.0.1.tar.gz              
unittest2-1.1.0.tar.gz

Instructions
------------
1. Modify Vagrant file or corresponding Inventory file
2. Modify playbook.yml and set the variables accordingly
3. Run 'vagrant up'


TODO
----
1. Refactor variables in playbook in vars directory
2. Integrate ETL scripts for Platform Symphony

