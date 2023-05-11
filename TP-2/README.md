
### Commandes ah-hoc  
##### Création du fichier d'inventaire principal
  C'est le fichier **hosts** (hosts1 avec 1 noeud / hosts2 avec 2 noeuds)

##### Ping ansible via le module ping:
```bash
  ansible -i hosts2 all -m ping
```  
##### Création de fichier à l'aide du module copy
```bash
  ansible -i hosts2 all -m copy -a "dest=/home/vagrant/toto.txt content='bonjour christian'"
```  
##### Découverte des machines distances avec le module setup
```bash
  ansible -i hosts2 all -m setup
```