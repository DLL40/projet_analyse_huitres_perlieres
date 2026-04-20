# Analyse Exploiratoire et Descriptive des Données

### 1. Dictionnaire des données : aperçu du nombre de variables, leur nom, leur type et paramètres, les ordres de grandeur 

D'après l'énoncé, nous savons que : 
- nous disposons de 900 observations 
- la variable PROFONDEUR est comprise entre 5 cm et 10 cm 
- la variable SUCCES = Oui ne concernent que 30% des huîtres

<img width="993" height="287" alt="Dictionnaire des données" src="https://github.com/user-attachments/assets/c4536ef4-a4dc-4585-b601-3766e5091bcf" />

**Objectif de l'étude :**

Nous cherchons à modéliser le succès de la greffe (présence d'une perle) en fonction des caractéristiques de l’huitre au moment de la greffe. Ce qui intéresse particulièrement l'entreprise PACIFIC FISHER, c’est d’augmenter le taux de succès en diminuant la probabilité d’échec. On cherche donc à connaître les facteurs qui contribuent au succès de la greffe. 

Variable cible : SUCCES (qualitative binaire) 
Prédicteurs : ZONE ; VARIETE ; PROFONDEUR ; LONGUEUR ; EPAISSEUR ; POIDS 
Deux modèles de discrimination pourront être mis en compétitions : 
- Régression logistique
- Arbre de discrimination
