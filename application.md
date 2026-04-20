# Analyse Exploiratoire et Descriptive des Données

### 1. Dictionnaire des données : aperçu du nombre de variables, leur nom, leur type et paramètres, les ordres de grandeur 

D'après l'énoncé, nous savons que : 
- nous disposons de 900 observations 
- la variable PROFONDEUR est comprise entre 5 cm et 10 cm 
- la variable SUCCES = Oui ne concernent que 30% des huîtres

<img width="993" height="287" alt="Dictionnaire des données" src="https://github.com/user-attachments/assets/c4536ef4-a4dc-4585-b601-3766e5091bcf" />

**Objectif de l'étude :**

Nous cherchons à modéliser le succès de la greffe (présence d'une perle) en fonction des caractéristiques de l’huitre au moment de la greffe. Ce qui intéresse particulièrement l'entreprise PACIFIC FISHER, c’est d’augmenter le taux de succès en diminuant la probabilité d’échec. Nous devons donc déterminer les facteurs qui contribuent au succès de la greffe. 

- Variable cible : SUCCES (qualitative binaire) 
- Prédicteurs : ZONE ; VARIETE ; PROFONDEUR ; LONGUEUR ; EPAISSEUR ; POIDS 
- Deux modèles de discrimination pourront être mis en compétitions : 
      - Régression logistique
      - Arbre de discrimination
  
### 2. Statistiques univariées : repérer les valeurs manquantes, aberrantes, voire extrêmes

Pour chaque variable qualitative : 
- statistiques descriptives
- diagramme à barres ou camembert (si modalités > 2)  

D'après notre tableau précédent, nous disposons ici de trois variables qualitatives :
- SUCCES
- ZONE
- VARIETE

Ainsi, sur SPSS :

<img width="542" height="140" alt="SPSS_11" src="https://github.com/user-attachments/assets/ac7a790f-51c8-4be1-8c31-2460a267d3f7" />
<b/>

<img width="543" height="261" alt="SPSS_22" src="https://github.com/user-attachments/assets/c7dc45ec-1486-47ab-b927-10211a1bfe24" />

Pour les différentes variables nous obtenons les graphiques suivants :

a) SUCCES

<img width="452" height="363" alt="graph_1" src="https://github.com/user-attachments/assets/581f91f4-56f2-4921-99a5-3cc58e6af651" />

- Plus de la moitié des huîtres (65,6%) n’ont pas produit de perle 18 mois après la greffe 
- Pas de valeurs manquantes / atypiques

b) ZONE

<img width="452" height="362" alt="graph_2" src="https://github.com/user-attachments/assets/fddbab73-5874-43bf-bdb2-0cf709218265" />

- Plus d’une huître greffée sur deux a été élevée dans la première zone.  
- Pas de valeurs manquantes / atypiques

c) VARIETE

<img width="436" height="351" alt="graph_3" src="https://github.com/user-attachments/assets/b615ba24-1823-4f45-9dee-17a241164290" />

- Près de trois huîtres greffées sur cinq sont de variété A 
- Pas de valeurs manquantes / atypiques

Pour chaque variable quantitative : 
- statistiques descriptives
- histogramme ou boîtes à moustache

Variables quantitatives 
- PROFONDEUR
- LONGUEUR
- EPAISSEUR
- POIDS

Sur SPSS, 

<img width="521" height="173" alt="SPSS_1" src="https://github.com/user-attachments/assets/7f1719e3-c9e5-42f9-a10f-9a20db696c29" />

<img width="421" height="270" alt="SPSS_2" src="https://github.com/user-attachments/assets/c1fd3a36-8e98-415f-8612-6cb5eb1bc9e4" />

<img width="611" height="402" alt="SPSS_3" src="https://github.com/user-attachments/assets/a1aaee37-31ad-41c9-91e9-2f190d243e9e" />

Pour les différentes variables nous obtenons les graphiques suivants :

a) PROFONDEUR

<img width="536" height="501" alt="graph_4" src="https://github.com/user-attachments/assets/c31ce7d6-9fba-48c4-b279-60a97b80a24a" />

<img width="440" height="351" alt="graph_5" src="https://github.com/user-attachments/assets/2a28ed8d-c4f2-41ed-901f-33884871fcad" />

<img width="442" height="352" alt="graph_6" src="https://github.com/user-attachments/assets/d54bb594-db91-44f3-ae2a-b5dc33c5a6b2" />

- Données sont bien comprises entre 5 et 10 cm (information du cas) 
- Pas de valeurs manquantes, atypiques 
- Variable quantitative discrète 
- La très grande majorité des huîtres sont élevées entre 6 et 8 cm de profondeur (env. 76%)

b) LONGUEUR

<img width="435" height="95" alt="graph_7" src="https://github.com/user-attachments/assets/348e06c8-87e1-4345-8add-1207c81fed43" />

<img width="371" height="326" alt="graph_8" src="https://github.com/user-attachments/assets/209251e7-2a43-4b4f-bce6-01a3407b29c2" />

- Données comprises entre 7,6 et 105 cm
- Pas de valeurs manquantes, mais 2 valeurs atypiques : H392 (105 cm) et H069 (91 cm)
- Ces valeurs peuvent être dues à un dysfonctionnement de l’appareil de mesure ou à une erreur de saisie => nous considérons ces valeurs comme manquantes

<img width="487" height="392" alt="graph_9" src="https://github.com/user-attachments/assets/c4851ac9-771c-4151-9d5a-b9a1f5eb723a" />

<img width="657" height="137" alt="graph_10" src="https://github.com/user-attachments/assets/123fd6f6-9882-4b76-969e-526aaf4cd93e" />

- Données comprises entre 7,6 et 14,6 cm
- Queue de distribution étalée vers la gauche ; asymétrie à gauche (coefficient d’asymétrie = 1,052)
- 50% des observations ont une longueur comprise entre 7,6 et 9,2 cm
- On pourrait faire une transformation logarithmique pour aplatir la distribution
  
c) EPAISSEUR

<img width="427" height="340" alt="graph_11" src="https://github.com/user-attachments/assets/869400e2-2947-434f-931b-2fb3b90b4969" />

- Données comprises entre 1,3 et 3,9 cm
- Pas de valeurs manquantes, ni atypiques
- L’huître mesure en moyenne 2,7 cm d’épaisseur. 

d) POIDS

<img width="502" height="115" alt="graph_12" src="https://github.com/user-attachments/assets/a396a4c2-72ee-4525-9798-22ec6318164f" />

<img width="438" height="353" alt="graph_13" src="https://github.com/user-attachments/assets/b6ee5247-39d0-45ba-9d91-8d135419fcd7" />

- Données comprises entre 71 et 156 grammes
- 20 valeurs manquantes, pas de valeurs atypiques
- Queue de distribution étalée vers la gauche ; asymétrie à gauche (coefficient d’asymétrie = 0,687)
- 50% des observations ont un poids compris entre 71 et 99 grammes

Conclusion Statistiques Univariées 
Variables qualitatives : 
Les huîtres qui ne produisent pas de perle représentent 66% des huîtres greffées 
Les huîtres, dans leur majorité : - ont été élevées dans la première zone (53%),  - sont de variété A (61%), 
pas de valeurs manquantes, ni aberrantes 
 
Variables quantitatives : - La majorité des huîtres ont été élevées entre 6 et 8 cm de profondeur (~76%) - Les huîtres ont une épaisseur moyenne de 2,7 cm au moment de la greffe. 
 - 2 valeurs aberrantes pour LONGUEUR, qui ont été considérées comme manquantes - Après suppression de ces données, les huîtres ont une longueur moyenne de 9,7 cm 
(médiane = 9,2).  
 - 20 valeurs manquantes pour POIDS - Les huîtres ont un poids moyen de 102g au moment de la greffe (médiane = 99).
