# Etude de cas : Analyse huîtres perlières

### Contexte :

L’entreprise d’aquaculture **Pacific Fisher** envisage de se lancer dans la production d’huîtres perlières. Les huitres 
sont élevées en milieu naturel entre 5 et 10m de profondeur, puis au bout d’un an environ, on introduit dans l’huitre 
un petit greffon de nacre qui permettra à la perle de se développer. Après la greffe, les huitres sont remises en 
élevage pour la durée nécessaire à la croissance de la perle, de l'ordre de 18 mois. Cependant moins de  30% des 
huitres greffées forment une perle commercialisable. 

L’étude de faisabilité montre que cette nouvelle activité ne sera rentable pour Pacific Fisher que si le taux de succès 
peut être augmenté de façon significative  (succès = l’huitre produit une perle commercialisable). D’où l’idée de 
chercher à modéliser le succès en fonction des caractéristiques de l’huitre au moment de la greffe. Si on trouve un 
modèle performant, les huitres dont la probabilité de développer une perle commercialisable est faible ne seront 
tout simplement pas greffées. 

Pour cette étude, on a collecté les données suivantes sur 900 huitres greffées : 
- zone d’élevage : zone 1, 2 ou 3 
- variété : A ou B 
- profondeur d’élevage
- au moment de la greffe : taille (longueur et épaisseur) et poids de l’huitre (en cm et g) 
- 18 mois après la greffe, **présence d’une perle commercialisable : Oui / Non**
