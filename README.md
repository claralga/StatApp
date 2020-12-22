## Projet de statistiques appliquées - CREST, ENSAE, Institut Polytechnique de Paris
### Sujet : Machine Learning à l'Assemblée Nationale

Romane Gajdos, Clémentine Abed-Meraim, Poppée Mongruel, Clara Le Gallic-Ach
 
Encadré par Jules Depersin et Nicolas Schreuder

*De novembre 2020 à juin 2021*
 



Ce dossier comporte plusieurs fichiers : 
  - importation_données : importation des données en format .json depuis l'open data de l'Assemblée Nationale
  - database_scrutins : fichier csv comprenant les données par scrutin
  - database_votants : fichier csv comprenant les données par votant
  - database_creation : code pour fusionner les deux bases de données ci-dessus
  - database_votes : base de données finale sur le vote des députés à l'Assemblée nationale
  - statistiques_scrutins : statistiques descriptives des scrutins (nombre de votants par scrutin, de pour/contre, d'abstention...)
  - statistiques_votants : statistiques descriptives sur les votants et leur groupe d'appartenance 
  - statistiques_demandeurs : travail sur les demandeurs de la loi, notamment nettoyage de ces données et one hot encoding 
