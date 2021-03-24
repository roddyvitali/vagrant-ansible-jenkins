# IaC - Vagrant Ansible Jenkins

Install jenkins with playbook and show password like output

### Vagrant Up (master & node)

```
vagrant up
```

### Connect master to node with ssh

- Set ssh credentials for users root and vagrant in node
- Allow connect like user root at node
- Generate ssh key in master
- Copy master public key at node

### Inventory

server-jerkins 192.168.50.2

### Playbook Steps

- Install Java
- Get Jenkins Key
- Get Jenkins Repository
- Install Jenkins
- Get and show password auto generate

### Run playbook with inventory defined

```
ansible-playbook -i projects/inventory projects/playbook
```

### Go to Server

> Copy the initial password admin from the console output and go to browser and open the server 192.168.50.2 on port 8080
