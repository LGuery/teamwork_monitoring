# Weekly Reports

* [8 Janvier](#date-8th-January-2021)
* [15 Janvier](#date-15th-January-2021)
* [21 Janvier](#date-21st-January-2021)
* [29 Janvier](#date-29th-January-2021)
* [4 février](#4-février)
* [9 février](#9-février)
* [18 février](#18-février)
* [3 mars](#3-mars)
* [10 mars](#10-mars)
-------------------------------------------------------------------
## Date: 8th January 2021
#### Who helped you this week? 
Loreleï (rmarkdown, github), Daniel (admin etc.)
#### What did you achieve?
* Lu et classifié des articles (cf "bibliographie.md")
* Travaillé sur tutoriel SOM de Rakotomalala envoyé par Daniel en utilisant des données d'un cours de l'ETH (cf. fichier Rmarkdown dans le repository SOMtest) --> réussi à créer cartes SOM et à mieux comprendre leur fonctionnement et les données nécéssaires.
* Intro github de Loreleï pour commit, push etc.
* commencé une liste de concepts statistiques utiles à revoir
#### What did you struggle with?
* Dans le tuto SOM, pas réussi la partie clusterisation, message d'erreur sur dim(x)
* pas clair s'il faut transformer (scale, center, zero-variance) les données avant de les utiliser pour la SOM
* influence de la corrélation entre les variables pas claire
#### What would you like to work on next week?
* terminer le tuto SOM et comprendre bien les étapes
* lire plus d'articles qui illustrent l'utilisation des SOM en écologie et bien comprendre les étapes avant la modélisation --> commencer mind map suggérée par Daniel avaec le workflow SOM
* revoir les concepts statistiques qui sont sur la liste
#### Where do you need help from Daniel, Lorelei or others?
* éventuellement sur la partie clusterisation, à confirmer quand j'aurai pris un peu plus de temps pour comprendre le problème
#### Any other topics
* prendre contact avec mon encadrant ETH pour lui dire ,comment ça se passe etc. --> lui proposer de rejoindre le "weeklyreports" github si OK pour vous et lui ? 
#### Weekly meeting 
* symposium mardi, mercredi et jeudi à la station
## Date: 15th January 2021
#### What did you achieve?
* Lu et classifié des articles (cf "bibliographie.md")
* Travaillé sur tutoriel SOM de Rakotomalala envoyé par Daniel en utilisant des données d'un cours de l'ETH (cf. fichier Rmarkdown dans le repository SOMtest)
* Revu qques concepts statistiques mis sur la liste, p.ex Ward's distance, bootstrapping etc.
* Assisté au symposium AOTTP avec Daniel, Loreleï et Sosthène
* SOM workflow commencé avec doc en plus "données utiles", "r packages et fonctions" et "méthodes utiles" pour retrouver les infos facilement
#### What did you struggle with?
* Choix des paramètres SOM (hexagonal VS rectangulaire) toujours pas clair, influences corrélation entre variables
#### What would you like to work on next week?
* Tester des fonctions pour digitaliser cartes, tester fonctions pour transformer raster en tableau pour voir si fonctionne en input SOM
* continuer biblio
* ? à clarifier au meeting lundi
#### Where do you need help from Daniel, Lorelei or others?
* A clarifier lundi
#### Any other topics
#### Weekly meeting 
* lundi 18
## Date: 21st January 2021
#### What did you achieve?
* Lu encore qques articles
* Fini et compilé doc sur différentes librairies SOM
* Rdv skype avec Jake, et tuna dream team pour prise de contact et discuter un peu des prochaines étapes
* Rdv skype avec Jake et Bernat pour parler du paper Oikos --> pas mal de travail qd même, deadline 18 février. Il y a bcp de questions de formulation/présentation des concepts dont ils se chargeront plutôt eux.
* readings pour mon cours Env. Regulation (certains très intéressants d'ailleurs, que je peux vous envoyer si ça vous intéresse)
* nettoyé un peu documents pour pouvoir les montrer demain (vendredi) au skype
* premier regard sur dataset ICCAT envoyé par Daniel
#### What did you struggle with?
* petite bouffée de stress en recevant mail oikos + mail sur sur le cours environmental regulation...
* Quel système de coordonnées géographiques est utilisé par l'ICCAT
#### What would you like to work on next week?
* sur les données ICCAT et voir dans quel format elles doivent être pour input SOM (je suggère d'utiliser la librairie kohonen comme Mendoza-Carranza et al.)
* env. regulation lundi et mercredi 10-12 et 14-16 avec bcp de readings à préparer, je vais essayer de faire le max ce week-end
* vendredi 28 rdv paper oikos pour faire le point
#### Where do you need help from Daniel, Lorelei or others?
* A clarifier demain
#### Any other topics
#### Weekly meeting 
* demain vendredi 22 et lundi 25
## Date: 29th January 2021
#### What did you achieve?
* cours Env. Regulation lundi et mercredi + readings--> idée policy brief (basée sur email Daniel): dynamic ocean management for trop. atlantic tuna fisheries
* SOM avec données ICCAT pour années 1991-1997 (~19000 samples), clustering ok, à approfopndir + lecture DOM
* paper oikos, meeting 
#### What did you struggle with?
* comment projeter les années (comme Mendoza) sur la carte SOM dans R (vu examples librairie d3.js), et plus tard autres variables
* petits problèmes de motivation cette semaine
#### What would you like to work on next week?
* régler cette histoire de visualisation des SOMs , essayer avec qqes données environnementales pour voir ce que ça donne 
* essayer ensuite de voir les clusters --> par année? par localisation ? par saison?
* écrire l'abstract pour la conférence (deadline 5.2)
#### Where do you need help from Daniel, Lorelei or others?
* écriture abstract conférence ?
* éventuellement sur ces histoires de visualisation, la plupart des gens font les SOM sur matlab du coup pas facile de trouver des tipps sur interrnet
#### Any other topics
#### Weekly meeting 
* mercredi à la station ?
## 4 février
#### Who helped you this week?
* meeting hier avec tt le monde, discussions très constructives sur les SOM et ce sur quoi il faut se concentrer mnt (cf. meetings reports)
#### What did you achieve?
* paper oikos
* compilé document html avec SOM 91-97, 98-19, pour le montrer au meeting du 3.
* pas perdu à l'ascenseur ni au barbu
#### What did you struggle with?
* visualisation des résultats SOM
* sélection nb de clusters
#### What would you like to work on next week?
* régler cette histoire de visualisation des SOMs, essayer package SOMbrero ?
* tester méthode Ilan pour sélection nb clusters
* tester autres distances pour clusters
* relire Mendoza et Andrienko pour voir comment ils gèrent les dimensions spatio-temporelles
* tester réduction dimension 1 par 1, p.ex. année type, comme ça variation temporelle juste sur les mois.
* envoyer l'abstract pour la conférence
* se concentrer sur années 91-97 pour tous ces tests
* identifier outliers dans données et checker si normal
* essayer de faire tourner SOM sans log10() et standardize()
* essayer de visualiser clusters dans espace géographique (régler problème crs au passage, car la violence policière c'est pas cool)
#### Where do you need help from Daniel, Lorelei, Ilan or others?
* peut-être pour projections géographiques (Ilan?)
* peut-être pour création années types (Daniel?)
#### Any other topics
#### Weekly meeting 
* mercredi prochain 11.03 à la station ?
## 9 février
#### What did you achieve?
* envoyé l'abstract
* pas mal travaillé sur le paper oikos, il fallait que je termine des trucs, sinon ça nous empêchait d'avancer
* testé autres distances pour la clusterisation et Ward.D2 est bel et bien la plus adaptée
* add.cluster.boundaries
* trouvé une 2ème méthode bien pour sélection nb de clusters
* SOM année type et saison type (février-juin) pour réduire la dimension temporelle (dcf docs html)
* visu clusters dans espace géographiques (problèmes points sur terre à discuter, d'après moi il s'agit en fait d'erreurs dans le dataset)
* reregardé le package sombrero, mais les fonctions pour plotter ne prennent pas des objets kohonen en input, et puis après j'ai eu la flemme de relire tout le package manual...
#### What did you struggle with?
* vraiment pas très productive, surtout hier et aujourd'hui...
#### What would you like to work on next week?
* régler cette histoire de visualisation des SOMs, essayer package SOMbrero ? --> commencé
* tester méthode Ilan pour séection nb clusters --> demander à Ilan !
* identifier outliers (géographiques et quantitatifs) dans données et checker si normal !
* essayer de faire tourner SOM sans log10() et standardize()
#### Where do you need help from Daniel, Lorelei, Ilan or others?
* à discuter demain
#### Any other topics
#### Weekly meeting 
* demain mercredi à la station
## 18 février
* semaine de télétravail à Genève, ça fait du bien de changer un peu de décor et de voir des amis !!
#### What did you achieve?
* envoyé ajd ENFIN le paper oikos
* tests CPUE et filtrage données ICCAT
* Année type 98-09
* avancé policy brief (pour cours env regulation, deadline 1 mars)
#### What did you struggle with?
* filtrage données ICCAT
#### What would you like to work on next week?
* finir policy brief
* savoir quel format de données je veux utiliser pour quoi
* commencer à chercher données sur requins et autres, voir comment les extraire (ou les demander aux auteurs qui sont de Marbec??)
#### Where do you need help from Daniel, Lorelei, Ilan or others?
* à discuter demain
* ne pas oublier de parler des données environnementales --> pk veut-on les utiliser et lesquelles ? Clavareau et al. disent que déjà plusieurs auteurs montrent qu'il y a peu de corrélations entre distribution thons et données classiques (SST, O2 etc)
#### Any other topics
#### Weekly meeting 
* demain vendredi skype
## 3 mars
#### What did you achieve?
* terminé et envoyé policy brief sur dynamic ocean management
* écrit et finalisé rapport activité janvier-février:
* refait tourner toutes les SOMs pour le rapport avec ratio largeur/longueur défini par eigenwerte de la input matrix et rlen = 10'000 à chaque fois
* clustering cutreeHybrid() pour tou.te.s
* refait tourner saisons avec trimestres classiques à la place des saisons de Gipsy
* refait année type 99/03 à la place de 98/09
* refait comparaison méthodes clustering
#### What did you struggle with?
* savoir à quel point le rapport devait être formel et déjà dans l'analyse des résultats... j'espère que c'était plus ou moins ce que vous vouliez
* malgré tous mes efforts d'organisation, toujours casse-tête de retrouver exactement d'où venait quel info pour la policy brief et le rapport
#### What would you like to work on next week?
* comme discuté ajd: analyse données task 2 pour voir si moratoires respectés ou non, à quel degré, etc., faire tableau récapitulatif --> demander son code à Ilan !
* regarder données ICCAT T2_SZ et T2_CZ avec tailles et/ou poids ? utilisable pour notre analyse ?
* Si données ECD regarder ça aussi et réfléchir à transfert aux données ICCAT task 2
#### Where do you need help from Daniel, Lorelei, Ilan or others?
* données ECD
* code Ilan
#### Any other topics
#### Weekly meeting
* ce matin
## 10 mars
#### What did you achieve?
* data check sur zones moratoires
* commencé powerpoint pour jeudi marbec
* checké données ICCAT de taille --> elles n'ont pas l'air très prometteuses
* préparé entretien de stage pour parc national des calanques (qui était mardi matin), comme ça me stressait je n'arrivais pas à travailler sur autre chose...
#### What did you struggle with?
* html sur github, tableaux n'apparaissent pas chez les autres --> check package DT et regarder formation CESAB sur github
* ggplot(): je n'arrive pas à ajouter les limites géographiques du moratoires s'il y a un facet_wrap() (mais ça marche pour une carte simple avec geom_segment()) ...
* Et puis je trainais un truc la semaine dernière qui m'épuisait, mais maintenant ça va mieux !
#### What would you like to work on next week?
* données ECD de taille ? commencer analyses hotspots juvéniles
#### Where do you need help from Daniel, Lorelei, Ilan or others?
#### Any other topics
#### Weekly meeting
* tout à l'heure (jeudi 11 matin)
