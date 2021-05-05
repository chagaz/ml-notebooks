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
1. Installez Anaconda en téléchargeant [l'installeur correspondant à votre système d'exploitation](https://www.anaconda.com/products/individual#Downloads).
2. Téléchargez ce répertoire. Vous pouvez utiliser [downgit](https://downgit.github.io/#/home?url=https://github.com/chagaz/ml-notebooks/tree/master/liesse).
3. Ouvrez Anaconda et créez l'environnement Python contenant tous les modules nécessaires – cf. la section "Importing an environment" [du tutoriel](https://docs.anaconda.com/anaconda/navigator/tutorials/manage-environments/). Le fichier décrivant l'environnement est le fichier `packages_list.yml`.
Alternativement, en ligne de commande, utilisez 
```bash
   conda env create -f package_list.yml -n cours
   conda activate cours
```
4. Lancez Jupyter Notebook (depuis Anaconda ou, en ligne de commande, `jupyter notebook`)
5. Naviguez grâce à l'explorateur de fichier jusqu'au notebook `0-Donnees.ipynb`

### Utilisation avancée (git)
Pour faciliter le contrôle de version avec de notebooks jupyter, vous pouvez utiliser [`nbstripout`](https://pypi.org/project/nbstripout/), qui nettoie votre notebook (en particulier en enlevant les cellules de sortie) : installez-le avec
```bash
conda install -c conda-forge nbstripout
```
puis, avant de faire un commit,
```bash
nbstripout <nom_du_notebook>.ipynb
```
