PROJET n°2 : HADOOP BIG DATA & Power BI
==========
Présentation et objectifs du projet 
-----------------------------------------
- Utilisation de Hadoop pour effectuer un map/reduce sur une base de données afin de filtrer des données pour analyse.
Les map/reduce sont écrits en Python.
- Utilsation de Happybase pour la création d'une base de données Hbase.
- Importation de cette base de données dans PowerBI pour production de tableaux de bord intéractifs.

Ce projet est constitué de trois lots à la demande du client, une fromagerie qui propose des cadeaux à sa clientèle en échange de points et/ou chèque et/ou timbres.
Cette société possède un Data Warehouse depuis 2004 au format csv (fichier source : dataw_fro03.csv). 
Ces données concernent la gestion des commandes de cadeaux sur 20 ans sur la France entière.

Environnements et configuration technique
------------------------------------------
Pour la réalisation de ce projet, nous avons un environnement virtuel configuré et mis à disposition par Diginamic (Christophe G.). Cet environnement est composé de :
 - une machine virtuelle Linux pour faire tourner Docker et Hadoop
 - une machine virtuelle Windows (Hidora) pour le développement et Power BI
Les technologies et logiciels utilisés sont :
 - langage Python avec VS Code et les librairies associées : Pandas, Matplotlib, sys, happybase, ...
 - Hadoop pour le calcul distribué des map/reduce 
 - HBase pour le stockage de la base de données NoSQL orientée colonnes
 - PuTTY
 - Power BI avec ODBC
 - 


Lot 1 : Le client désire les statistiques suivantes
-------------------------------------------
<tr>
<td>1. Filtrer les données selon les critères suivants : 
  - Commandes passées entre 2006 et 2010 ;
  - uniquement sur les départements 53, 61 et 28.</td>
<br> 
<td>2. A partir du point 1 : Ressortir dans un tableau les 100 meilleures commandes avec la ville, la somme des quantités des articles commandés et la valeur de «timbrecde» pour chaque commande. La notion de meilleure commande désigne la somme des quantités la plus grande ainsi que le plus grand nombre de «timbrecde».</td>
<br> 
<td>3. Exporter le résultat dans un fichier Excel.</td>
</tr>


Lot 2 : Le client désire les statistiques suivantes
-------------------------------------------
<tr>
<td>1. Filtrer les données selon les critères suivants :
  - Commandes passées entre 2011 et 2016
  - uniquement les départements 22, 49 et 53.</td>
<br>
<td>2. A partir du point 1 : Ressortir de façon aléatoire 5% des 100 meilleures commandes avec la ville, la somme des quantités des articles sans «timbrecli» (le timbreclinon renseigné ou à 0) avec la moyenne des quantités de chaque commande)</td>
<br>
<td>3. Exporter le résultat dans un fichier Excel et créer un graphique (PIE) par Ville en PDF</td>
<td> Fig1: Représentation graphique des quantités commandées par ville (exemple)
<img src="GraphQtesVilles.png"     alt="dat-viz données "/></td>
</tr>


Lot 3 : Mettre en place une base NoSQL HBASE et créer des tableaux de bord intéractifs avec Power BI
-------------------------------------------
<tr>
<td>1. Pour stocker le contenu du fichier CSV et de mettre en oeuvre un moteur de recherche avec Power BI pour interroger ce Data Warehouse.</td>
<td>2. Pour répondre au Lot 1 et Lot 2 au niveau des résultats avec les graphes</td>
<td>3. Mise en place d’un Dashboard interactif</td>
</tr>
