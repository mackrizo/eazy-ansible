###Sécurité

### Commandes ad-hoc
##### Encrypter un fichier, utiliser "toto" comme mot de passe de chiffrement
```bash
ansible-vault encrypt files/secrets/credentials.yml
```

##### Décrypter un fichier
```bash
ansible-vault decrypt files/secrets/credentials.yml
```

##### Lancer ansible en lui passant le mot de passe de décryptage
```bash
ansible-playbook -i hosts.yml --ask-vault-pass deploy.yml
```

##### Créer un couple ssh de clé publique/privées
```bash
ssh-keygen -t rsa
```

##### Copier la clé publique sur le serveur distant
```bash
ssh-copy-id admin@10.0.0.4
```