<<<<<<< HEAD
# Ansible Kafka



## How to get it

Add to your playbooks requirements.yml:




 Inventory example:

[kafka]
kafka-3 ansible_ssh_host=10.xxxx
kafka-2 ansible_ssh_host=10.xxxx
kafka-1 ansible_ssh_host=10.xxxx

[zookeeper]
kafka-3 ansible_ssh_host=10.xxxx
kafka-2 ansible_ssh_host=10.xxxx
kafka-1 ansible_ssh_host=10.xxxx


[all:vars]
ansible_user=ubuntu
kafka_zookeeper_hosts=[ 'kafka-1','kafka-2','kafka-3'  ]
kafka_hosts=[ 'kafka-1','kafka-2','kafka-3' ]
zookeeper_hosts=kafka-1:2181,kafka-2:2181,kafka-3:2181


[xenials]  # Ubuntu 16.04 hosts without python2
kafka-3 ansible_ssh_host=10.xxxx
kafka-2 ansible_ssh_host=10.xxxx
kafka-1 ansible_ssh_host=10.xxxx


[xenials:vars] 
ansible_user=ubuntu
#ansible_python_interpreter=/usr/bin/python3
=======
# Ansible Kafka ROLE
>>>>>>> add a \ in consumer and change mode
# ansible_kafka
