# Stage LIESSE 2021 - IA

Ce répertoire contient les notebooks correspondant au stage LIESSE « Intelligence Artificielle » à Mines ParisTech des 4 et 5 mai 2021 et couvre les sujets suivants : 

* Modèles linéaires : régression linéaire, régression logistique
* Réseaux de neurones : perceptrons multi-couches pour la régression et la classification 
* Méthodes des plus proches voisins

Les notebooks ont été conçu avec Python 3.8.8 et les librairies suivantes :
* matplotlib 3.3.4
* numpy 1.19.2
* pandas 1.2.2
* sklearn 0.24.1

### Protocole si vous partez de zéro
1. **Installez Anaconda** en téléchargeant [l'installeur correspondant à votre système d'exploitation](https://www.anaconda.com/products/individual#Downloads). Anaconda est une distribution de Python orientée vers la science des données et l'apprentissage automatique, dont le but est de faciliter la gestion des paquets python, y compris via une interface graphique (le Navigateur Anaconda).
2. **Téléchargez ce répertoire.** Vous pouvez simplement cliquer sur [ce lien downgit](https://downgit.github.io/#/home?url=https://github.com/chagaz/ml-notebooks/tree/master/liesse) pour le télécharger sous la forme d'une archive zip.
3. Ouvrez Anaconda et **créez l'environnement** Python contenant tous les modules nécessaires. Le fichier décrivant l'environnement est le fichier `packages_list.yml`. Vous pouvez suivre la section "Importing an environment" [du tutoriel](https://docs.anaconda.com/anaconda/navigator/tutorials/manage-environments/). 
Alternativement, en ligne de commande, utilisez 
```bash
   conda env create -f package_list.yml -n cours
   conda activate cours
```
4. **Lancez Jupyter Notebook** (depuis Anaconda ou, en ligne de commande, `jupyter notebook`). Jupyter Notebook s'ouvre dans votre navigateur web (mais ne nécessite pas de connexion Internet) et permet de créer des notebooks (ou « calepins ») interactifs, c'est-à-dire des fichiers contenant du texte (mis en forme grâce à la syntaxe Markdown), du code, et les résultats de l'exécution de ce code (sorties numériques, figures, etc.), et modifiables à la volée. Les notebooks Jupyter pour le langage Python portent l'extension `.ipynb`. Jupyter Lab offre quelques fonctionalités supplémentaires, notamment la possiblité d'ouvrir plusieurs notebooks en même temps et de copier-coller des cellules entre eux.
5. Avec l'explorateur de fichier de Jupyter qui s'est ouvert dans votre navigateur, naviguez jusqu'au premier notebook (`0-Donnees.ipynb`) et cliquez dessus pour le lancer.

### Utilisation avancée (git)
Pour faciliter le contrôle de version avec de notebooks jupyter, vous pouvez utiliser [`nbstripout`](https://pypi.org/project/nbstripout/), qui nettoie votre notebook (en particulier en enlevant les cellules de sortie) : installez-le avec
```bash
conda install -c conda-forge nbstripout
```
puis, avant de faire un commit,
```bash
nbstripout <nom_du_notebook>.ipynb
```
vous pouvez utiliser `git diff <nom_du_notebook>.ipynb` avant votre comit pour vérifier les modifications.
