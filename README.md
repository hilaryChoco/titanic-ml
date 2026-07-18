# 🚢 Titanic — Prédiction de survie

Projet de classification binaire pour prédire la survie des passagers du Titanic.
Réalisé dans le cadre d'un parcours de montée en compétences en Machine Learning.

## 📊 Résultats

| Métrique | Score |
|---|---|
| Accuracy | 80% |
| Precision (Survécu) | 76% |
| Recall (Survécu) | 74% |
| F1-score (Survécu) | 75% |

## 🔧 Stack technique

- **Python 3.11**
- **pandas** — chargement et nettoyage des données
- **matplotlib / seaborn** — visualisations
- **scikit-learn** — modélisation (Random Forest)
- **joblib** — sauvegarde du modèle

## 📁 Structure du projet
titanic-ml/
│
├── train.csv                      # Dataset d'entraînement (Kaggle)
├── titanic.ipynb                  # Notebook principal
├── random_forest_titanic.pkl      # Modèle sauvegardé
└── README.md                      # Ce fichier

## 🔄 Étapes du projet

1. **Exploration des données (EDA)** — dimensions, statistiques, visualisations
2. **Nettoyage** — valeurs manquantes, encodage des variables catégorielles
3. **Modélisation** — Random Forest (100 arbres, random_state=42)
4. **Évaluation** — accuracy, precision, recall, F1-score
5. **Analyse** — importance des features

## 💡 Points clés

- Les 3 features les plus prédictives : **Fare**, **Sex**, **Age** (~78% de l'importance totale)
- Le modèle est meilleur pour prédire les décès (F1: 0.83) que les survivants (F1: 0.75)
- Pistes d'amélioration : extraction des titres depuis `Name`, feature engineering sur `Ticket`

## 🚀 Lancer le projet

```bash
# Cloner le repo
git clone https://github.com/hilaryChoco/titanic-ml.git
cd titanic-ml

# Créer l'environnement
conda create -n ml-pratique python=3.11
conda activate ml-pratique
pip install numpy pandas scikit-learn matplotlib seaborn jupyterlab joblib

# Lancer le notebook
jupyter lab
```

## Auteur

**Hilary** — Étudiante en maîtrise IA, Université Laval  
GitHub : [@hilaryChoco](https://github.com/hilaryChoco)