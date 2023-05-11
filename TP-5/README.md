### Utilisation d'un playbook

### Commandes ad-hoc
#####  Installation de ansible-lint
```bash
sudo pip install ansible-lint
```

#####  Check de l'indentation du playbook
```bash
ansible-lint deploy.yml
```

#####  Lancement du playbook
```bash
ansible-playbook -i hosts.yml -vvv deploy.yml
```