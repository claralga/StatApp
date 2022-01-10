## Projet de statistiques appliquées - CREST, ENSAE, Institut Polytechnique de Paris
### Sujet : Machine Learning à l'Assemblée Nationale

Romane Gajdos, Clémentine Abed-Meraim, Poppée Mongruel, Clara Le Gallic-Ach 
Encadré par Jules Depersin et Nicolas Schreuder
*De novembre 2020 à juin 2021*
 
 
Notre projet repose sur les données suivantes : **https://data.assemblee-nationale.fr/**



Ce projet comporte plusieurs dossiers : 
  - **Rapport : Le pdf de notre rapport rédigé comportant tous les graphiques finalisés**
  - Data : Les fichiers csv de nos données
  - Data Process : Les scripts de certaines de nos manipulations de données
  - Premières Statistiques : Les scripts des statistiques descriptives générales des données
  - Random Forest : Les scripts concernant la random forest
 
 Ci-dessous le détail de certains fichiers : 
  - importation_données : importation des données en format .json depuis l'open data de l'Assemblée Nationale
  - database_scrutins : fichier csv comprenant les données par scrutin
  - database_votants : fichier csv comprenant les données par votant
  - database_creation : code pour fusionner les deux bases de données ci-dessus
  - database_votes : base de données finale sur le vote des députés à l'Assemblée nationale
  - statistiques_votants : statistiques descriptives sur les votants et leur groupe d'appartenance 
  - statistiques_demandeurs : travail sur les demandeurs de la loi, notamment nettoyage de ces données et one hot encoding 
  - clustering: travail de clustering des députés en fonction de leur historique de vote et des indices crées 
  - cluster_votants : création de la dataframe historique de vote des députés
  - scrapping_age : récupération de l'âge de chaque député.e sur sa page wikipédia
  - profil votants : clustering sur l'évolution de l'accord de chaque député avec son parti (piste abandonnée, notebook à supprimer à terme)
  - abstention_final : notebook reprenant le travail sur l'abstention avec les bonnes données + une frise chronologique du taux d'abstention
  - agreement_index : plot des indices de cohésion de chaque parti en fonction du temps (à relier avec statistiques_votants)

Open Data : 
- https://www.hatvp.fr/wordpress/wp-content/uploads/2016/12/Open-data-integrite-publique.pdf 
- https://www.gouvernement.fr/action/l-ouverture-des-donnees-publiques


Articles : 
- https://www.ladepeche.fr/2021/01/23/comment-votent-vos-deputes-a-lassemblee-nationale-9328626.php : À un an et demi de la fin de leur mandat – les prochaines élections législatives sont programmées en juin 2021 –, le site internet datan.fr a épluché et analysé le comportement des parlementaires français, avec l’historique de tous les votes des députés… Soit plus de 3 000 scrutins ! Positions importantes, derniers votes, participation, loyauté envers son groupe politique, quels sont les enseignements à en tirer pour nos élus aveyronnais ?
- https://laviedesidees.fr/Qui-sont-les-deputes-francais-de.html : Quelle est la population des députés français depuis les débuts de la Cinquième République ? Au travers d’une analyse statistique de la composition des 13 législatures, A. François et E. Grossman dressent un portrait du député français et suivent l’évolution des pensionnaires de l’Assemblée Nationale. Il apparaît que la structure socioprofessionnelle en est particulièrement stable.
- https://laviedesidees.fr/Les-enracines-du-Palais-Bourbon.html : Les professionnels de la politique ont mauvaise presse. Trois sociologues ont enquêté sur l’évolution du profil de nos députés, et leurs conclusions invitent à s’interroger : les résultats des élections de juin 2017 marquent-ils vraiment une ouverture du monde politique ?
- https://laviedesidees.fr/Les-cols-blancs-de-l-Assemblee-nationale.html : Qu’est-ce que les vêtements et tissus de l’Assemblée nationale disent du fonctionnement d’une institution politique ? En s’attachant aux coulisses de ce petit monde, Delphine Gardey réincarne la production des lois et des discours, et ouvre l’analyse des matières du pouvoir.
- http://www.slate.fr/story/147171/deputes-diversite : La nouvelle Assemblée comptera notamment une petite quinzaine d'élus issus de l'immigration dite «arabo-musulmane», à l'issue d'une campagne où, selon une récente étude, leur présence parmi les candidats reflétait leur poids général dans la population française.
- https://tnova.fr/notes/l-agonie-de-la-democratie-parlementaire : Un premier bilan de la réforme constitutionnelle vue sous l'angle du travail parlementaire La révision constitutionnelle du 23 juillet 2008 a modifié en profondeur la procédure parlementaire. Un an après son entrée en vigueur, et malgré les références à "l'hyper-parlement", l'usage systématique par la majorité gouvernementale de procédures permettant d'enrayer le travail parlementaire signale une dérive dangereuse pour la démocratie. Selon Jean-Jacques Urvoas, Député du Finistère et maître de conférences en droit public, c'est désormais aux élus de l'opposition de montrer l'exemple.
- https://journals.openedition.org/sociologie/3284#xd_co_f=YzRkMTgyMzAtMWE0Mi00YTRkLWIyN2ItMTY3OGIyYTVlOWEw~ : Partant du constat qu’être un professionnel de la politique est mal vu dans la société française, ils en déconstruisent les origines, les causes et les conséquences, pour soutenir deux thèses fortes : la professionnalisation de la vie politique française s’est essentiellement accrue par l’augmentation du temps passé en politique par les élus, en même temps qu’elle a entrainé une individualisation de la carrière politique. En 138 pages et quatre chapitres, la démonstration est efficace : après s’être intéressés à la façon dont les députés de l’Assemblée nationale rejettent à tout prix l’identification de leur activité politique à un métier (chapitre 1), les auteurs proposent une plongée au cœur des « pratiques d’Assemblée » (Nay, 2003) en montrant ce qu’est au quotidien le métier de député (chapitre 2). Ce sont ensuite les transformations des modes d’entrée en politique et des profils sociologiques des députés qui sont analysées (chapitre 3), ainsi que l’individualisation du capital politique qui en découle (chapitre 4). Malgré la densité des matériaux recueillis, et parfois la complexité de leur traitement, les auteurs ont fait de cet ouvrage un écrit pédagogique et accessible aux non-spécialistes, en répondant en chercheurs critiques à la question suivante : la professionnalisation est-elle un problème ?
- https://www.cairn.info/revue-politique-europeenne-2014-1.htm : Opposés dans la diversité. Les usages de l’opposition à l’Europe en France
- https://www.revuepolitique.fr/la-nouvelle-sociologie-de-lassemblee-nationale-renouvellement-ou-cercle-ferme/ : La nouvelle sociologie de l’Assemblée nationale : renouvellement ou « cercle fermé » ?
- https://www.leparisien.fr/paris-75/la-loyaute-est-necessaire-comment-votent-les-deputes-de-paris-20-01-2021-8420279.php : A un an de la fin de leur mandat, le Parisien fait le point sur l’activité des députés de l’Oise et de l’Ile-de-France. Zoom sur les 16 élus parisiens, très respectueux des consignes de vote de leurs partis.
