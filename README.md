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
  - clustering: travail de clustering des députés en fonction de leur historique de vote et des indices crées 
  - cluster_votants : création de la dataframe historique de vote des députés
  - scrapping_age : récupération de l'âge de chaque député.e sur sa page wikipédia


Articles : 
- https://laviedesidees.fr/Qui-sont-les-deputes-francais-de.html : Quelle est la population des députés français depuis les débuts de la Cinquième République ? Au travers d’une analyse statistique de la composition des 13 législatures, A. François et E. Grossman dressent un portrait du député français et suivent l’évolution des pensionnaires de l’Assemblée Nationale. Il apparaît que la structure socioprofessionnelle en est particulièrement stable.
- https://laviedesidees.fr/Les-enracines-du-Palais-Bourbon.html : Les professionnels de la politique ont mauvaise presse. Trois sociologues ont enquêté sur l’évolution du profil de nos députés, et leurs conclusions invitent à s’interroger : les résultats des élections de juin 2017 marquent-ils vraiment une ouverture du monde politique ?
- https://laviedesidees.fr/Les-cols-blancs-de-l-Assemblee-nationale.html : Qu’est-ce que les vêtements et tissus de l’Assemblée nationale disent du fonctionnement d’une institution politique ? En s’attachant aux coulisses de ce petit monde, Delphine Gardey réincarne la production des lois et des discours, et ouvre l’analyse des matières du pouvoir.
- http://www.slate.fr/story/147171/deputes-diversite : La nouvelle Assemblée comptera notamment une petite quinzaine d'élus issus de l'immigration dite «arabo-musulmane», à l'issue d'une campagne où, selon une récente étude, leur présence parmi les candidats reflétait leur poids général dans la population française.
