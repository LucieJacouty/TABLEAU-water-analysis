# Etude de l'accès à l'eau potable dans le monde avec Tableau  

Projet Openclassrooms - Formation Data Analyst    


Objectif : Réaliser plusieurs dashboards présentant une vue globale de l'accès à l'eau potable dans le monde   

Projet pour le compte d'une ONG comprenant 3 domaines d'expertise.
Demande de financement effectuée : si accordée permettra d'investir dans un des domaines d'expertise dans un pays  
But : déterminer le pays à cibler  

Contenu :
- Data : données préparées utilisées sous Tableau
- Notebook préparation : notebook jupyter qui a permis de préparer les données
- Water Analysis Tableau : export Tableau Desktop regroupant toutes les visualisations

### Synthétisation des besoins clients : 

Besoin de 3 dashboards : niveau mondial, régional et national 
Choix d'un principe de cascade -> du plus large au plus précis. Zoom grâce aux filtres intéractifs  

### Vérification et Préparation des données avec Python : 
 
Vérification des valeurs nulles (notamment "accès à l'eau de qualité") 
Vérification de la synchronisation des noms des pays 
Pivot table population et calcul taux urbain 
Création des indices pour l'efficacité gouvernementale (index final champs calculé sous Tableau)  


## Vues Export Tableau  

### Vue mondiale : 

Vue statique, présente principaux indicateurs aggrégés niveau mondial :
- Taux de moralité moyen
- Nombre de morts dû à l'eau insalubre 
- Evolution de l'accès à l'eau basique (rural, urbain, total) 
- Evolution de la population urbaine (à relier à l'évolution de l'accès à l'eau)  
- Carte Mondiale représentant les taux de mortalité selon les pays  

### Vue Régionale/Continentale :

Même indicateurs que précédemment 
Ajoute la possibilité d'interaction : 
- Filtres : sélection région(s), taux de mortalité, stabilité politique
- Sélection sur la carte 

Intéraction renforcée avec la vue nationale 

### Vue nationale : 

3 visualisations représentant les 3 domaines d'expertise de l'ONG  
Tous les filtres/sélections appliquées sur la vue régionale se retrouvent sur la vue nationale 

But : faire une première sélection avec les filtres sur la vue régionale ; puis analyser les pays les plus en difficultés dans chaque domaine d'expertise avec la vue nationale