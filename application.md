# Analyse Exploiratoire et Descriptive des Données

### 1. Dictionnaire des données : aperçu du nombre de variables, leur nom, leur type et paramètres, les ordres de grandeur 

D'après l'énoncé, nous savons que : 
- Nous disposons de **900 observations**
- La variable PROFONDEUR est comprise **entre 5 cm et 10 cm** 
- La variable SUCCES prenant la modalité "Oui" ne concernent que **30% des huîtres**

<img width="993" height="287" alt="Dictionnaire des données" src="https://github.com/user-attachments/assets/c4536ef4-a4dc-4585-b601-3766e5091bcf" />

<br>

### Objectif de l'étude :

Nous cherchons à modéliser le succès de la greffe (présence d'une perle) en fonction des caractéristiques de l’huitre au moment de la greffe. Ce qui intéresse particulièrement l'entreprise PACIFIC FISHER, c’est d’augmenter le taux de succès en diminuant la probabilité d’échec. Nous devons donc déterminer les facteurs qui contribuent au succès de la greffe. 

- Variable cible : SUCCES (qualitative binaire) 
- Prédicteurs : ZONE ; VARIETE ; PROFONDEUR ; LONGUEUR ; EPAISSEUR ; POIDS 
- Deux modèles de discrimination pourront être mis en compétition : **Régression logistique** et **Arbre de discrimination**
  
### 2. Statistiques univariées : repérer les valeurs manquantes, aberrantes, voire extrêmes

▶️Pour chaque variable qualitative : 
- statistiques descriptives
- diagramme à barres ou camembert (si modalités > 2)  

D'après notre tableau précédent, nous disposons ici de trois variables qualitatives :
- SUCCES
- ZONE
- VARIETE

Ainsi, sur SPSS :

<img width="542" height="140" alt="SPSS_11" src="https://github.com/user-attachments/assets/ac7a790f-51c8-4be1-8c31-2460a267d3f7" />

<br>

<img width="543" height="261" alt="SPSS_22" src="https://github.com/user-attachments/assets/c7dc45ec-1486-47ab-b927-10211a1bfe24" />

<br>

Pour les différentes variables qualitatives nous obtenons les graphiques suivants :

a) SUCCES

<img width="452" height="363" alt="graph_1" src="https://github.com/user-attachments/assets/581f91f4-56f2-4921-99a5-3cc58e6af651" />

<br>

- Plus de la moitié des huîtres (65,6%) n’ont pas produit de perle 18 mois après la greffe 
- Pas de valeurs manquantes, ni atypiques

b) ZONE

<img width="452" height="362" alt="graph_2" src="https://github.com/user-attachments/assets/fddbab73-5874-43bf-bdb2-0cf709218265" />

<br>

- Plus d’une huître greffée sur deux a été élevée dans la première zone.  
- Pas de valeurs manquantes, ni atypiques

c) VARIETE

<img width="436" height="351" alt="graph_3" src="https://github.com/user-attachments/assets/b615ba24-1823-4f45-9dee-17a241164290" />

<br>

- Près de trois huîtres greffées sur cinq sont de variété A 
- Pas de valeurs manquantes, ni atypiques

▶️Pour chaque variable quantitative : 
- statistiques descriptives
- histogramme ou boîtes à moustache

Nous avons ici quatre variables quantitatives :
- PROFONDEUR
- LONGUEUR
- EPAISSEUR
- POIDS

Sur SPSS, nous procédons aux différentes analyses :

<img width="521" height="173" alt="SPSS_1" src="https://github.com/user-attachments/assets/7f1719e3-c9e5-42f9-a10f-9a20db696c29" />

<br>

<img width="421" height="270" alt="SPSS_2" src="https://github.com/user-attachments/assets/c1fd3a36-8e98-415f-8612-6cb5eb1bc9e4" />

<br>

<img width="611" height="402" alt="SPSS_3" src="https://github.com/user-attachments/assets/a1aaee37-31ad-41c9-91e9-2f190d243e9e" />

<br>

Pour les variables quantitatives, nous obtenons les résultats suivants :

a) PROFONDEUR

<img width="536" height="501" alt="graph_4" src="https://github.com/user-attachments/assets/c31ce7d6-9fba-48c4-b279-60a97b80a24a" />

<br>

<img width="440" height="351" alt="graph_5" src="https://github.com/user-attachments/assets/2a28ed8d-c4f2-41ed-901f-33884871fcad" />

<br>

<img width="442" height="352" alt="graph_6" src="https://github.com/user-attachments/assets/d54bb594-db91-44f3-ae2a-b5dc33c5a6b2" />

<br>

- Conformément aux informations du cas, les données sont bien comprises entre 5 cm et 10 cm 
- Pas de valeurs manquantes, ni atypiques 
- Il s'agit d'une variable quantitative discrète 
- La très grande majorité des huîtres (près de 76%) sont élevées entre 6 et 8 cm de profondeur 

b) LONGUEUR

<img width="435" height="95" alt="graph_7" src="https://github.com/user-attachments/assets/348e06c8-87e1-4345-8add-1207c81fed43" />

<br>

<img width="371" height="326" alt="graph_8" src="https://github.com/user-attachments/assets/209251e7-2a43-4b4f-bce6-01a3407b29c2" />

<br>

- Données comprises entre 7,6 cm et 105 cm
- Pas de valeurs manquantes, mais 2 valeurs atypiques : les huîtres n°392 (105 cm) et n°069 (91 cm)
- Ces valeurs peuvent être dues à un dysfonctionnement de l’appareil de mesure ou à une erreur de saisie => **nous considérons ces valeurs comme manquantes**

<img width="487" height="392" alt="graph_9" src="https://github.com/user-attachments/assets/c4851ac9-771c-4151-9d5a-b9a1f5eb723a" />

<br>

<img width="657" height="137" alt="graph_10" src="https://github.com/user-attachments/assets/123fd6f6-9882-4b76-969e-526aaf4cd93e" />

<br>

- Données comprises entre 7,6 cm et 14,6 cm
- La distribution est étalée vers la gauche => asymétrie à gauche (coefficient d’asymétrie = 1,052)
- 50% des observations ont une longueur comprise entre 7,6 cm et 9,2 cm
- Nous pourrions procéder à une transformation logarithmique pour aplatir la distribution
  
c) EPAISSEUR

<img width="427" height="340" alt="graph_11" src="https://github.com/user-attachments/assets/869400e2-2947-434f-931b-2fb3b90b4969" />

<br>

- Données comprises entre 1,3 cm et 3,9 cm
- Pas de valeurs manquantes, ni atypiques
- Les huîtres ont une épaisseur moyenne de 2,7 cm

d) POIDS

<img width="502" height="115" alt="graph_12" src="https://github.com/user-attachments/assets/a396a4c2-72ee-4525-9798-22ec6318164f" />

<br>

<img width="438" height="353" alt="graph_13" src="https://github.com/user-attachments/assets/b6ee5247-39d0-45ba-9d91-8d135419fcd7" />

<br>

- Données comprises entre 71 g et 156 g
- 20 valeurs manquantes, pas de valeurs atypiques
- La distribution est étalée vers la gauche ; asymétrie à gauche (coefficient d’asymétrie = 0,687)
- 50% des observations ont un poids compris entre 71 g et 99 g

### Conclusion Statistiques Univariées 

▶️Variables qualitatives : 
- Les huîtres ne produisant pas de perle représentent **66% des huîtres greffées**
- Les huîtres, dans leur majorité : ont été **élevées dans la zone 1 (53%)** et sont de **variété A (61%)**
- Absence de valeurs manquantes et atypiques 
 
▶️Variables quantitatives : 
- La majorité des huîtres ont été élevées **entre 6 cm et 8 cm de profondeur (~76%)**
- Les huîtres ont une **épaisseur moyenne de 2,7 cm** au moment de la greffe 
- 2 valeurs aberrantes pour LONGUEUR, qui ont été **considérées comme manquantes** => après suppression de ces données, les huîtres ont une **longueur moyenne de 9,7 cm (médiane = 9,2)**  
- 20 valeurs manquantes pour POIDS
- Les huîtres ont un **poids moyen de 102 g** au moment de la greffe (médiane = 99)

### 3.  Statistiques bivariées : repérer des relations fortes entre deux variables, trouver des solutions pour les valeurs manquantes

Ci-dessous, un tableau résumant le nombre d'analyses bivariées à effectuer ainsi que la nature de ces croisements

<img width="966" height="267" alt="tableau_corr_1" src="https://github.com/user-attachments/assets/aa38de43-c152-438f-8552-b8e61a1db030" />

<br>

<table>
  <tr style="border: none;">
    <td style="border: none; vertical-align: middle;">
      <img width="92" height="27" alt="legend_qlql" src="https://github.com/user-attachments/assets/0ec13723-8890-4100-976d-a1e90f0ef19a">
    </td>
    <td style="border: none; vertical-align: middle;"> : Croisement de deux variables qualitatives
    </td>
  <tr style="border: none;">
    <td style="border: none; vertical-align: middle;">
      <img width="92" height="27" alt="legend_qlqt" src="https://github.com/user-attachments/assets/5e83c9d3-7849-42af-9065-a6faa6157d2e">
    </td>
    <td style="border: none; vertical-align: middle;"> : Croisement d’une variable qualitative (2 ou 3 modalités) et quantitative
    </td>
  <tr style="border: none;">
    <td style="border: none; vertical-align: middle;">
      <img width="92" height="27" alt="legend_qtqt" src="https://github.com/user-attachments/assets/213aacc9-00c7-42b8-a8d7-44e538a4bd40">
    </td>
    <td style="border: none; vertical-align: middle;"> : Croisement de deux variables quantitatives
    </td>
  </tr>
</table>

En théorie, nous devrions effectuer 21 analyses bivariées. Cependant, nous allons voir qu'il sera possible de reduire ce nombre d’analyses en supprimant notamment les variables susceptibles d'être redondantes en informations.

Par exemple, il apparait tout à fait pertinent de penser que la longueur ou l’épaisseur de l’huître ont possiblement une relation avec le poids de l’huître. De plus, pour rappel, le poids de l’huître possède 20 valeurs manquantes. 

a) Croisements de deux variables quantitatives : corrélations (matrice de dispersion)

- LONGUEUR*POIDS
- LONGUEUR*EPAISSEUR
- POIDS*EPAISSEUR  
- PROFONDEUR*POIDS  
- PROFONDEUR*LONGUEUR

Etape 1 : analyse visuelle avec la matrice de dispersion

Sur SPSS, pour obtenir la matrice de dispersion, nous suivons les étapes ci-dessous

<img width="598" height="456" alt="Biv_1" src="https://github.com/user-attachments/assets/f4472e96-4eaf-4c3b-a642-3c9466f92a3b" />

<br>

<img width="571" height="243" alt="Biv_2" src="https://github.com/user-attachments/assets/10c655a2-c07e-4fb8-8604-2c76d4496ba9" />

<br>

En cliquant sur "Dispersion de type matrice" nous pouvons insérer toutes les variables quantitatives

Nous obtenons alors la matrice de dispersion suivantes :

<img width="497" height="396" alt="QTQT_1" src="https://github.com/user-attachments/assets/c4d80bc0-6dfc-4f33-b1ce-efc93bd06f04" />

<br>

Ainsi, graphiquement, nous constatons : 
- pas ou peu de relation entre la profondeur d’élevage et les autres prédicteurs
- une relation linéaire positive entre le poids de l’huître et sa longueur => plus une huître est lourde et plus elle est longue  
- pas ou peu de relation entre LONGUEUR et les autres prédicteurs 
- pas ou peu de relation entre EPAISSEUR et les autres prédicteurs

Etape 2 : test de la significativité de la relation

Nous pouvons quantifier l’intensité des relations par le coefficient de corrélation de Bravais-Pearson :

<img width="553" height="296" alt="Biv_3" src="https://github.com/user-attachments/assets/3d25cc4d-fb9d-4a55-a836-95e31c021e1a" />

<br>

<img width="541" height="320" alt="QTQT_2" src="https://github.com/user-attachments/assets/5bf16d6f-ded9-4ff2-a82a-d06155ffe72b" />

<br>

- Confirmation de la **forte relation entre LONGUEUR et POIDS** (r = 0,87, corrélation significative p<0,01). 
- Nous constatons l'existence d'une **faible relation négative entre l’épaisseur et la longueur d’une huître** => plus une huître est fine et plus elle est grande (r = -0,30, corrélation significative p<0,01). 
- La variable POIDS possède 20 valeurs manquantes alors qu’elle nous apporte une information quasi similaire à 
LONGUEUR. **Nous allons donc supprimer la variable POIDS de notre modèle**. Ainsi, nous n’effectuerons plus
d’analyse bivariée sur cette variable. 

b) Croisements de deux variables qualitatives : Test du Khi-deux d’indépendance et Coefficients d’association (Phi et V de Cramer)

Toujours sur SPSS, en suivant la procédure ci-dessous : 

 <img width="553" height="296" alt="Biv_4" src="https://github.com/user-attachments/assets/2850e297-a3de-48e6-9b51-99a97af2417b" />

<br>

<img width="690" height="360" alt="Biv_5" src="https://github.com/user-attachments/assets/c46997b5-f61a-44b7-b370-b4afdc8864d3" />

<br>

En cliquant sur "Statistiques" et en cochant Khi-deux et Phi et V de Cramer, nous obtenons respectivement le test et la force de l’association
- Le coefficient Phi est pertinent pour les tableaux 2x2 seulement
- Le coefficient V de Cramer est pertinent pour les tableaux plus grands que 2x2

> [!NOTE]
Si coefficient ~0,10 alors faible association ; si coefficient ~0,30 alors association moyenne ; si coefficient >0,50 alors forte association

<img width="515" height="208" alt="Biv_6" src="https://github.com/user-attachments/assets/2864926d-e1b2-4e9f-a56d-57a9dd23a122" />

<br>

ZONE*VARIETE : Analyse d'une possible relation entre la zone d’élevage et la variété de l’huître

<img width="362" height="290" alt="QLQL_ZV_1" src="https://github.com/user-attachments/assets/b748d3b8-4b6b-457e-97d1-365ce75cd876" />

<br>

Graphiquement, nous ne constatons pas de relation entre la zone d’élevage et la variété de l’huître (Il y a autant 
d’huîtres de variété A et B dans les différentes zones) => Les deux variables sont à priori indépendantes.

Cette analyse est confirmée par le test de la relation entre ces deux variables (non significatif) :

<img width="356" height="121" alt="QLQL_ZV_2" src="https://github.com/user-attachments/assets/fab54cf2-7047-46c3-8677-5d8f051a1cf6" />

<br>

c) Croisements variables qualitatives (à 2 modalités) et quantitatives : Analyse graphique (boxplot) et/ou test
t pour échantillons indépendants

Procédure SPSS : 

<img width="740" height="216" alt="Biv_7" src="https://github.com/user-attachments/assets/e6302775-da3b-40e2-bfc7-85f3f04c5f7d" />

<br>

Nous insérons la variable quantitative dans "variable à tester" et la variable qualitative dans "variable de regroupement" en définissant les différents groupes correspondant aux différentes modalités

<img width="586" height="352" alt="Biv_8" src="https://github.com/user-attachments/assets/10f9655a-b653-4f97-97de-214090a26c64" />

<br>

Si la relation est significative, il faut calculer la force de l’association (pas donné par SPSS) càd calculer l’indice Eta-carré (η2 ): 
           
η2 =  t² / t² + (N1 + N2 -2)

avec N1 et N2, la taille de chaque groupe. 
 
> [!NOTE]
Si coefficient ~0,01 alors faible association ; si coefficient ~0,06 alors association moyenne ; si coefficient ~0,14 
et plus, alors forte association

VARIETE*LONGUEUR

<img width="462" height="372" alt="QLQT_VL_1" src="https://github.com/user-attachments/assets/8b88b97a-a03e-4e66-b3b0-6b2290810e60" />

<br>

Graphiquement, il existe une relation entre la variété de l’huître et sa longueur : les huîtres de variété A semblent 
moins longues que les huîtres de variété B. 
- La variété A correspondrait à des huîtres de longueur majoritairement comprises entre 8 cm et 12 cm 
- La variété B correspondrait à des huîtres de longueur majoritairement comprises entre 8 cm et 15 cm

<img width="478" height="465" alt="QLQT_VL_2" src="https://github.com/user-attachments/assets/c7d1cd89-22c3-4ef8-be62-7ceaf9049f6f" />

<br>

Les huîtres de variété B sont en moyenne plus longues de 1,3 cm. 
Nous devons déterminer quelles sont les probabilités d'observer une différence d'au moins 1,3 cm entre les deux 
groupes indépendants d’huîtres (variété A et B) si ces deux groupes proviennent de la même population (H0)

<img width="472" height="131" alt="QLQT_VL_3" src="https://github.com/user-attachments/assets/0278a5ba-dba8-4ed4-ba43-acb6d78a9f5b" />

<br>

<img width="768" height="153" alt="QLQT_VL_4" src="https://github.com/user-attachments/assets/816d3fb7-3d42-4753-a0f4-9cfd0c824146" />

<br>

Le test d'homogénéité des variances est significatif : nous rejetons l'hypothèse nulle. Les variances sont 
significativement différentes. Nous devons donc lire la deuxième ligne. 
 
Le test t est significatif : on rejette H0, les deux groupes proviennent probablement de deux populations différentes. 

Nous pouvons ainsi calculer l’intensité de la relation entre ces deux variables : 

Eta-carré = (−11.302)² / (−11.302)2+(549+349−2) = 0,125 

↪️Relation significative d’intensité moyenne à forte => Il est donc possible d'estimer la longueur de l’huître des observations N°392 et N°069 en fonction de leur variété

Comme ces deux observations appartiennent à la variété B, nous imputons à ces deux observations, pour la variable LONGUEUR, la médiane du groupe B, c'est à dire 10 cm. En effet, en raison de la présence d'une asymétrie sur la distribution de LONGUEUR, nous ne pouvons leur attribuer la valeur de la moyenne de la variable LONGUEUR car celle-ci est biaisée.

Quelle variable garder dans notre modèle ? La longueur de l’huître ou la variété ? 

À priori, nous devrions garder la longueur car la variété de l’huître semble être déterminer par sa longueur. Cependant, la variété de l’huître est peut être une variable plus riche en informations en nous renseignant sur d'autres critères que la simple longueur de l’huître. 

Pour décider, nous décidons de regarder la variable qui explique le plus la présence d’une perle 18 mois après la 
greffe, c'est à dire, la variable dont l'intensité de la relation avec la variable SUCCES est la plus prononcée

SUCCES*VARIETE

<img width="362" height="287" alt="QLQL_SV_1" src="https://github.com/user-attachments/assets/e4c84626-5184-466e-9796-c048b072a2c3" />

<br>

<img width="362" height="117" alt="QLQL_SV_2" src="https://github.com/user-attachments/assets/276af040-0ee6-40d2-b0c9-8f426527c706" />

<br>

Les huîtres de variété A ont plus de chances que celles de variété B de produire une perle 18 mois après la greffe. 
La relation est significative mais l’association est plutôt faible (~0,14)

SUCCES*LONGUEUR

<img width="312" height="251" alt="QLQT_SL_1" src="https://github.com/user-attachments/assets/584a1909-32de-4f1a-8cff-ae40f66f2709" />

<br>

<img width="766" height="257" alt="QLQT_SL_2" src="https://github.com/user-attachments/assets/d02d7aed-0529-45d5-b18f-44976a934b18" />

<br>

Le test d'homogénéité des variances est significatif : nous rejetons l'hypothèse nulle. Les variances sont 
significativement différentes. Nous devons donc lire la deuxième ligne. 

Le test t est significatif : les deux groupes proviennent probablement de deux populations différentes. 

Nous calculons donc l’intensité de la relation entre ces deux variables : 

Eta-carré = (−9.487)² / (−9.487)²+(590+310−2) = 0,09 

↪️L’association entre ces deux variables est significative, et est moyenne à forte => Plus l’huître est longue et moins elle est susceptible de produire une perle. 

Par conséquent, nous choisissons de garder dans notre modèle la variable qui a la plus forte relation avec la variable cible : il s’agit de la longueur de l’huître.

d) Croisements variables qualitatives (à 3 modalités) et quantitatives : Analyse graphique (boxplot) et/ou 
ANOVA à 1 facteur

> [!NOTE]
Pour l’ANOVA à 1 facteur, la variable qualitative doit être recodée en numérique

Procédure SPSS pour recoder une variable

<img width="562" height="215" alt="Biv_9" src="https://github.com/user-attachments/assets/6c52292e-3c2a-4a1e-b34b-8754284d3f14" />

<br>

<img width="746" height="403" alt="Biv_10" src="https://github.com/user-attachments/assets/2608168c-9d25-44e9-a4a8-fc0c26ff8cc4" />

<br>

Dans "Variable de destination", nous pouvons nommer la nouvelle variable puis cliquer sur "Changer"

Enfin, en cliquant sur "Anciennes et nouvelles valeurs" nous pouvons recoder les différentes modalités afin de finaliser la transformation de la variable qualitative en variable numérique

<img width="693" height="333" alt="Biv_11" src="https://github.com/user-attachments/assets/819870f1-5854-4991-8898-a6184ce67dd1" />

<br>

La variable qualitative (à 3 modalités) à présent recodée en variable quantitative, nous sommes désormais prêts à lancer l'analyse : 

<img width="646" height="266" alt="Biv_12" src="https://github.com/user-attachments/assets/3a276cd4-e9cd-4c9c-a1b0-908b243efa16" />

<br>
 
Nous insérons la variable quantitative dans "Variables dépendantes" et la variable qualitative dans "Facteur"

<img width="598" height="322" alt="Biv_13" src="https://github.com/user-attachments/assets/4242acc3-4466-4a53-8579-b58547cf4e1e" />

<br>

Si le test ANOVA est significatif, nous calculons la force de l’association :

$$r = \sqrt{\frac{\text{Somme des carrés intergroupes}}{\text{Somme totale des carrés}}}$$

> [!NOTE]
Si coefficient ~0,10 alors faible association ; si coefficient ~0,30 alors association moyenne ; si coefficient >0,50 
alors forte association

