# TP1 — Analyse d’un algorithme en fonctionnement

## Étudiant
Maeva Taite

## Matière
Les fondamentaux de l’IA

## Objectif
Observer un pipeline ML complet sur le dataset Iris, comparer un Decision Tree et un Random Forest, analyser les métriques, détecter l’overfitting et utiliser SHAP pour l’explicabilité.

## Structure du rendu
- `tp1_iris.ipynb` : notebook principal
- `images/` : graphiques générés
- `requirements.txt` : dépendances Python

## Réponses aux questions

### Étape 1 — Analyse des données
- Le dataset contient 150 échantillons.
- Il y a 50 échantillons par classe.
- Le dataset est équilibré.
- Il n’y a pas de valeurs manquantes.
- Les variables les plus discriminantes semblent être `petal_length` et `petal_width`.

### Étape 2 — Modèles
Commencer par une baseline simple permet d’avoir un point de comparaison avant d’utiliser un modèle plus complexe. Cela permet de vérifier si la complexité supplémentaire apporte une amélioration réelle.

### Étape 3 — Métriques
À compléter avec tes résultats obtenus dans le notebook :
- Accuracy Decision Tree :
- F1-score Decision Tree :
- Accuracy Random Forest :
- F1-score Random Forest :

Analyse :
- Le Random Forest devrait généralement être plus performant et plus stable.
- Les espèces les plus difficiles à distinguer sont souvent `versicolor` et `virginica`.

Différence accuracy / F1-score :
- L’accuracy mesure la proportion totale de bonnes prédictions.
- Le F1-score équilibre précision et rappel, et est plus utile en cas de classes déséquilibrées.

### Étape 4 — Overfitting
À compléter avec tes résultats :
- L’overfitting apparaît à partir d’une certaine profondeur lorsque le score d’entraînement reste très élevé mais que le score de test baisse ou stagne.
- Le meilleur compromis performance / coût est souvent atteint avec un nombre moyen d’arbres.

La validation croisée permet d’obtenir une estimation plus robuste qu’un simple split train/test.

### Étape 5 — SHAP
À compléter avec tes résultats :
- Variable la plus importante selon SHAP :
- Cohérence avec l’intuition :

Différence sklearn / SHAP :
- L’importance sklearn (MDI) mesure la contribution moyenne des variables dans les arbres.
- SHAP explique l’impact réel des variables sur les prédictions.

L’explicabilité est cruciale dans les domaines réglementés pour justifier les décisions prises par le modèle.

## Debrief — 3 insights

### Insight 1 — Performance
Observation :  
Explication :  
Implication pratique :  

### Insight 2 — Overfitting / Généralisation
Observation :  
Explication :  
Implication pratique :  

### Insight 3 — Explicabilité
Observation :  
Explication :  
Implication pratique :  