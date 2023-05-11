#### Découverte du yaml 

    Ecrire l'inventaire au format yaml

##### Ping ansible via le module ping:
```bash
  ansible -i hosts.yml all -m ping
```  
##### Création de fichier à l'aide du module copy
```bash
  ansible -i hosts.yml all -m copy -a "dest=/home/vagrant/toto.txt content='bonjour christian'"
```  

    Vérifiez que le fichier est écrit sur les deux noeuds.
```
