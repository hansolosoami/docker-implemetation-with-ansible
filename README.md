# docker-implemetation-with-ansible  
implementing docker-CE using ansible playbook including installation of docker and running of a nginx container with accessing the file 

# You should have ansible 2.7 install in your system to run this file.
# This playbook will be run in Centos7/RHEL7

 EC2 instance is named in hosts(inventory) file.
 
 # Steps to implement the launch of a container using ansible 
 
 1. cd /root/
 
 2. git clone https://github.com/pushpendersofficial/docker-implemetation-with-ansible
 
 3. cd docker-implemetation-with-ansible
 
 4. #now edit the host file by adding you Public DNS in the file ( docker-implemetation-with-ansible/hosts )
 
 5. Now add your key of AWS EC2 (private key) on this folder by name (ansibleuser1.pem)
 
 6. Now, firstly run:-
 
  #ansible-playbook docker_install.yml
  
  7. now run :-
  
  #ansible-playbook nginx-container.yml
 
 8. now run this command in your ec2 machine to check whether its working or not.
 
 #curl 127.0.0.1:8080
 
 9. check whether the container is running or not 
 
 #docker container ls
