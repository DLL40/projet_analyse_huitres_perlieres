## MODELISATION

Dans cette partie, nous avons deux modèles à mettre en compétition selon deux techniques de modélisation (Régression logistique + Arbre de discrimination) : 

Modèle 1 : SUCCES =  PROFONDEUR + LONGUEUR + EPAISSEUR  
Modèle 2 : SUCCES =  ZONE + LONGUEUR + EPAISSEUR 

Pour cela, nous utiliserons le logiciel SAS ENTERPRISE MINER

Après avoir montrer la procédure d'importation de notre base de données sur le logiciel (voir ci-dessous), nous comparerons nos deux retenus afin de déterminer le modèle le plus pertinent nous permettant de prédire les facteurs favorisant l’obtention d’une perle commercialisable au bout de 18 mois d’élevage. Les deux modèles vont être mis en compétition en utilisant deux techniques de modélisation qui sont la régression logistique et l’arbre de décision.  

#### ▶️ Procédure d’importation SAS ENTERPRISE MINER

Après avoir cliquer sur "Ouvrir un projet...", nous lui avons attribué un nom (par exemple : "Exo_Huitres") ainsi qu'un répertoire (ici, "T:\Datamining\Cas_Huitres")

<img width="898" height="405" alt="ProcImportSAS_1" src="https://github.com/user-attachments/assets/c8d73abe-1ebc-4ed5-9b49-1271cc6d8db3" />

<br>

Plutôt que d’utiliser les bibliothèques par défaut (Work, Sasuser), nous décidons de créer une bibliothèque SAS associée à un répertoire de notre espace de travail personnel, dans laquelle seront stockés nos fichiers SAS.

Nouveau => Bibliothèque

<img width="435" height="410" alt="ProcImportSAS_2" src="https://github.com/user-attachments/assets/21ba330f-c50e-4f19-837f-04dbbb0c9452" />

<br>

Créer une bibliothèque => Suivant

<img width="725" height="415" alt="ProcImportSAS_3" src="https://github.com/user-attachments/assets/ba1bc3fd-dbac-4922-8387-2abfa64e2da5" />

<br>

Nous nommons la bibliothèque "DM" en lui donnant le chemin d’accès correspondant au nom du répertoire crée précédemment : "T:\Datamining\Cas_Huitres"

Une fois la bibliothèque créée, il faut importer le fichier csv en cliquant sur l’éditeur de programmes puis, insérer le code comme ci-dessous et enfin appuyer sur "Run" pour exécuter :

<img width="1128" height="367" alt="ProcImportSAS_4" src="https://github.com/user-attachments/assets/47e0c756-55cc-48c0-a023-a0897f21e138" />

<br>









 


 


