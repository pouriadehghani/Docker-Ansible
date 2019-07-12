# Docker-Ansible
Define your servers in inventory file
```
cat <<EOF >> inventory 
server1
server2
server3
EOF
```
Run ansible playbook  like following :
```
ansible-playbook -i inventory all.yaml
```




Also you can define your docker-compose version in vars/allvars  the default value is 1.24.0

```
docker_compose_version: xxx
```
The default value of docker-compose path is : 
```
docker_compose_path: /usr/local/bin/docker-compose
```