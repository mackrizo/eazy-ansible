### Inventaire Ansible

#### Commandes ad-hoc depuis le serveur ansible, et création du fichier sur machine distante avec passage de paramètre

##### Inventaire au format ini
```bash
ansible -i hosts.ini client -m ping
ansible -i hosts.ini prod -m ping
ansible -i hosts.ini all -m copy -a "dest=/home/admin/toto.txt content='bonjour christian {{ env }} 

```

##### Inventaire au format yml
```bash
ansible -i hosts.yml client -m ping
ansible -i hosts.yml prod -m ping
ansible -i hosts.yml all -m copy -a "dest=/home/vagrant/toto.txt content='bonjour christian {{ env }} 

```