# Instructions pour projet : Développez un programme logiciel en Python
**Instruction** :
Ce projet a pour but de développer une application hors ligne de gestion de tournois d'échecs en utilisant Python et le modèle MVC. En assurant que l'application permette de sauvegarder et revoir les résultats, de suivre les principes de la programmation orientée objet, en respectant la PEP 8 pour la propreté du code, et en utilisant le format JSON pour les fichiers de données. 

## Configuration de l'Environnement

Pour exécuter le script, suivez les étapes ci-dessous pour configurer l'environnement.

### Prérequis

- Un éditeur : VisualStudio code, Spider, pycharm ...
- Python 3.x
- pip (LE gestionnaire de paquets pour Python)

### Création et Activation de l'Environnement Virtuel

1. **Créer un environnement virtuel** :

Ouvrez un terminal et naviguez jusqu'au dossier de votre projet. Exécutez la commande suivante pour créer un environnement virtuel :

   ```bash
   python -m venv env
```

2. **Activer l'environnement virtuel** :

Utilisez la commande appropriée selon votre système d'exploitation.

**Sur Windows** :

   ```bash
   env\Scripts\activate
```
**Sur MacOS/Linux** :

   ```bash
   source env/bin/activate
```


3. **Installation des Dépendances** :

Avec l'environnement virtuel activé, installez les dépendances requises :

   ```bash
   pip install -r requirements.txt
```
Assurez-vous que le fichier requirements.txt est présent dans le dossier du projet !

4. **Lancement du Script** :

Après l'installation des bibliothèques, lancez le script avec :

   ```bash
   python main.py
```

Vous pouvez maintenant naviguer dans tous les menus et sous menus de l'application !


## Générer un rapport avec flake8

Il faut changer l'option de longueur de ligne maximale et la fixée à 119 et exclure les répertoires/fichiers également non voulu.

Donc après avoir installer les dépendances requises :

Appliquer tout cela à l'aide de la commande :

   ```bash
   flake8 --format=html --htmldir=flake8-report --max-line-length 119 --exclude=.git,env,__pycache__,.gitignore
```

Assurez-vous de bien être dans le dossier du projet !


## Autre solution pour flake8

Dans le dossier du projet, créé un fichier nommé :

   ```bash
   setup.cfg
```

Puis dans ce fichier, copier les attributs voulu, vous pouvez modifier "exclude" au besoin :


   ```bash
[flake8]
format = html
htmldir = flake8-report
max-line-length = 119
exclude = .git,env,__pycache__,.gitignore
```


Ensuite dans le terminal, générer le rapport avec :
   ```bash
flake8 --format=html --htmldir=flake8-report
```
