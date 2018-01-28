## Installation of RthinkDB Single-node/Cluster Using Ansible

## Requirements
* vagrant

## TO RUN
* **STEP-1**
```
vagrant up
```

* **STEP-2**
```
vagrant ssh controller
```

* **STEP-3**
```
cd /home/vagrant/projects/playbooks
```

* **STEP-4**
SINGLE NODE

```
ansible-playbook -i hosts/single-node.ini rthink-single-node.yml -e rethinkClusterMode=single
```

CLUSTER SETUP
```
ansible-playbook -i hosts/cluster.ini rthink-cluster.yml -e rethinkClusterMode=cluster
```

# Supported/Tested OS
* CentOS7