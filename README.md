# Analyse de séries temporelles (timeseries)

Ce dépôt contient des jeux de données et un notebook Jupyter pour une première exploration et analyse de séries temporelles démographiques (naissances, mariages, âge moyen d'accouchement) en France.

## Contenu du dépôt

- `age moyen accouchement 1901.csv` : données sur l'âge moyen à l'accouchement (1901).
- `naissance_france.csv` : données de naissances en France.
- `Nombre total de mariages .csv` : nombre total de mariages (format CSV).
- `time_serie_analyse.ipynb` : notebook Jupyter contenant l'analyse exploratoire et les visualisations.

## Objectif

Fournir un point de départ pour l'analyse de séries temporelles démographiques. Le notebook couvre :

- nettoyage et préparation des données
- visualisations temporelles (trend, saisonnalité)
- exemples simples de décomposition et de modélisation

## Prérequis

- Python 3.8+ (testé avec 3.9/3.10)
- Jupyter / JupyterLab
- Bibliothèques Python usuelles : pandas, numpy, matplotlib, seaborn

Je recommande de créer un environnement virtuel :

```bash
python -m venv .venv
source .venv/bin/activate   # zsh / bash
pip install --upgrade pip
pip install jupyter pandas numpy matplotlib seaborn
```

Ou créer un `requirements.txt` si tu préfères :

```text
jupyter
pandas
numpy
matplotlib
seaborn
# ajoute d'autres dépendances si nécessaire
```

## Lancer le notebook

Dans le dossier du projet :

```bash
source .venv/bin/activate   # si tu utilises un environnement
jupyter lab                 # ou "jupyter notebook"
```

Ouvre ensuite `time_serie_analyse.ipynb` dans l'interface Jupyter.

## Bonnes pratiques / suggestions

- Ajouter un fichier `.gitignore` pour exclure les environnements virtuels, fichiers de checkpoint Jupyter, etc. Exemple minimal :

```
.venv/
.ipynb_checkpoints/
__pycache__/
*.pyc
```

- Si certains CSV sont volumineux et doivent rester privés, envisage de ne pas les committer et de les stocker ailleurs (ex : stockage cloud) et d'ajouter des scripts d'import.

## Licence

Ajoute ici la licence que tu souhaites (MIT, CC-BY, etc.) ou supprime cette section si non nécessaire.

## Contact

Si tu veux que j'améliore le notebook (tests, modélisation ARIMA/Prophet, README plus détaillé), dis-moi ce que tu veux explorer en priorité.
