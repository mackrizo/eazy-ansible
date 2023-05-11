### Rôles Ansible

### Commandes ad-hoc
##### Récupéreration des roles ansible
```bash
ansible-galaxy install -r roles/requirements.yml
```

##### Lancer ansible en lui passant le mot de passe de décryptage
```bash
ansible-playbook -i hosts.yml --ask-vault-pass wordpress.yml
```