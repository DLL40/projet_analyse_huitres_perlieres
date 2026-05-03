## MODELISATION

Dans cette partie, nous avons deux modèles à mettre en compétition selon deux techniques de modélisation (Régression logistique + Arbre de discrimination) : 

Modèle 1 : SUCCES =  PROFONDEUR + LONGUEUR + EPAISSEUR  
Modèle 2 : SUCCES =  ZONE + LONGUEUR + EPAISSEUR 

Pour cela, nous utiliserons le logiciel SAS ENTERPRISE MINER

Après avoir montrer la procédure d'importation de notre base de données sur le logiciel (voir ci-dessous), nous comparerons nos deux retenus afin de déterminer le modèle le plus pertinent nous permettant de prédire les facteurs favorisant l’obtention d’une perle commercialisable au bout de 18 mois d’élevage. Les deux modèles vont être mis en compétition en utilisant deux techniques de modélisation qui sont la régression logistique et l’arbre de décision.  

#### ▶️ Procédure d’importation SAS ENTERPRISE MINER

Après avoir cliquer sur "Ouvrir un projet...", nous lui avons attribué un nom (par exemple : "Exo_Huitres") ainsi qu'un répertoire (ici, "T:\Datamining\Cas_Huitres")

Plutôt que d’utiliser les bibliothèques par défaut (Work, Sasuser), nous décidons de créer une bibliothèque SAS associée à un répertoire de notre espace de travail personnel, dans laquelle seront stockés nos fichiers SAS. 

Nous nommons la bibliothèque "DM" en lui donnant le chemin d’accès suivant : "T:\Datamining\Cas_Huitres"
Il s'agit du nom du répertoire crée précédemment



 


 


