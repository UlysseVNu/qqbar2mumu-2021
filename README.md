
:warning: | WIP - ne pas utiliser avant la première scéance | :bangbang:
:---: | :---: | :---:

# Projet expérimental - Production de quarkonia

> Ce dépot git héberge les fichiers nécessaires pour démarrer le projet "Production de quarkonia" du Master 2 RPS de l'Université de Nantes. Il est principalement à destination des étudiants qui réalisent ce projet. Le "vous" ci-dessous s'adresse donc à ces étudiants.

Pour ce projet le language de programmation choisi est Python. Nous recommandons de l'utiliser par le biais de ["Notebooks Jupyter"](https://jupyter.org) qui permettent de mélanger le code, la documentation et les résultats de l'exécution du code.  

Jupyter est un outil commun dans le domaine de la science des données. Il y a bien des façons d'utiliser Jupyter et de nombreux tutoriels sont disponibles en ligne pour aller plus loin, mais vous trouverez ci-dessous deux méthodes pour démarrer : une méthode locale et une méthode "cloud".

## Installation locale (recommandée)

Si possible, essayez d'installer Jupyter sur votre ordinateur (portable), car cela offre plus de souplesse (et potentiellement de performance).

Même si ce n'est pas la seule façon d'installation Jupyter et les dépendences nécessaires à ce projet (ou tout autre projet à base de Python), nous conseillons le recours à [conda](https://docs.conda.io), en particulier via sa version [miniforge](https://github.com/conda-forge/miniforge/#download).

### Installation de miniforge (conda)

Récupérer le [script d'installation](https://github.com/conda-forge/miniforge/#download) correspondant à votre plateforme et exécutez-le. Par exemple sous Linux : 

```shell
bash Miniforge3-Linux-x86_64.sh
```

Suivez les instructions (en résumé : ENTER - SPACE - yes - ENTER - yes). 

A l'issue de cette étape la commande `conda` est maintenant disponible (vous devrez peut-être vous déconnecter et reconnecter pour la voir).

```shell
conda help
```

### Installation des paquets de base avec conda

Ce dépot contient un fichier [`environment.yml`](environment.yml) qui décrit les dépendences utilisées par le notebook d'exemple (`muon-eta-distribution.ipynb`) que vous utiliserez pour vous mettre dans le bain.

Avec conda (et plus généralement avec Python) il est très fortement recommandé de travailler dans un "environnement" (qui décrit un ensemble de modules Python et leurs versions respectives). Pour ce faire il faut installer l'environnement (une seule fois) :

```shell
conda env create
```

puis l'activer pour l'utiliser (à chaque connection/déconnection).

```shell
conda activate qqbar2mumu
```

Une fois l'environment activé, vous pouvez lancer Jupyter lab


```shell
jupyter lab
```

Ce qui lance une application web dans votre navigateur : 

![fenêtre initiale jupyter lab](./jupyter-lab-first-screen.png)

Double-cliquez sur `muon-eta-distribution.ipynb` dans le panneau de gauche et vous êtes prêts à démarrer !

## Installation cloud 

Si vous ne trouvez vraiment aucun ordinateur sur lequel installer le projet, vous pouvez essayer de travailler directement en ligne. Il existe [plusieurs services](https://www.dataschool.io/cloud-services-for-jupyter-notebook/) en ligne qui offrent la possibilité d'exécuter des notebooks Jupyter. 

A titre d'exemple, le badge suivant devrait vous permettre d'ouvrir le notebook d'example dans un de ces sites, Binder : 



