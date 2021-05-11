# Meetings
* [25 janvier](#25-janvier)
* [3 février](#3-février)
* [10 février](#10-février)
* [19 février](#19-février)
* [24 février](#24-février)
* [3 mars](#3-mars)
* [25 mars](#25-mars)
* [12 avril](#12-avril)
* [4 mai](#4-mai)
* [11 mai](#11-mai)
# 25 janvier
* discuté du système de coordonnées géographiques ICCAT (cadrans par rapport au 0°/0°), mais en fait les coordonnées classiques sont aussi dispos dans le dataset
* comparer carte SOM à carte géographique classique des captures juvéniles (zB Gipsy) pour validation
* dans un premier temps uniquement SOM non-supervisée avec données environnementales associées à chaque input vector (SST, O2, etc.) --> à discuter avec Ilan pour savoir lesquelles choisir. Pour l'instant premiers tests SOM uniquement avec données ICCAT.
* nous utiliserons les données ICCAT brutes (approche plutôt fisheries science, pression exercée sur le carré/mois) et aussi les CPUEs (approche + écologique, détection habitats) et comparerons les résultats. (p.ex. en cas de report de l'effort de pêche suite à un moratoire)
* on ne filtrera pas des éventuelles données problématiques car pas nécessaire à cette résolution (carré/mois)
* on n'utilisera pas les données ECD car on perdrait toutes les données des pays africains --> par contre éventuellement pour estimer la proportion de juvéniles dans les prises (car les classes de taille sont présentes dans le dataset ECD mais pas ICCAT)
* PVD pas tjrs échantillonage au port, armateurs coréens jouent pas le jeu --> éventuellement sujet pour policy brief ?
* vérifier dans dataset ICCAT si pas de données 5x5
* prochain point lundi 1er février
# 3 février
* refaire tourner SOM avec données ni log-transformées ni standardisées pour voir différence
* identifier les noeuds outliers et checker les données associées --> si erreur dans données ICCAT supprimer
* essayer clustering avec autre distance (pas Ward.D2), regarder si une distance en particulier est adaptée aux données log10()
* clustering: chercher méthodes autre que "elbow" pour choisir le nb de clusters. P.ex. méthodes avec dendogramme --> Ilan va m'envoyer un exemple qu'il avait utilisé. Tester 3 et 7 clusters pour les années 2000.
* faire tourner les SOM avec une année type pour voir variation spatiale et temporelle (mois) --> pour créer cette année type, prendre médiane pour chaque carré sur qques années plus ou moins identiques (p.ex. 1991-1995)
* faire tourner les SOM sur carré type pour voir variation entre années et aussi mois --> ?
* d'une manière générale pour ces histoires spatio-temporelles: regarder comment Andrienko 2010 et Mendoza 2018 ont géré leurs dimensions
* essayer SOM avec données aggrégées par saison
* analyse exploratoire: regarder l'évolution des captures dans une zone au cours d'une année type
* ne pas utiliser les proportions de chaque espèces dans les vecteurs en temps que nouvel input -->  il ne sera pas possible de discerner les vecteurs à forte abondance des vecteurs à faible abondance et on perdra de vue l'objectif d'identification des hotspots
* autre test diminution dimension: anomalie par carré pour voir lesquels s'écartent de la variation moyenne
* {} pour résoudre problème plots Rmd
* trouver comment visualiser les clusters et les noeuds dans l'espace géographique (comme Andrienko)
* trouver quel CRS est utilisé par l'ICCAT --> si pas donné, mail à Carlos (d'abord essayer la méthode d'Ilan df -> sf)
* faire graphique log10() pour évolution totale des prises et comparer aux time series par clusters.
# 10 février
* tester set.seed() pour voir si donne mm cartes
* verra-t-on apparaître les zones moratoires dans les clusters saisonniers des années 2000 ?
* data processing: filtrer les données en se basant sur méthode de Loreleï; regarder histogramme pour voir quelles cellules sont les moins visitées etc. Enlever les données problématiques (p.ex. celles situées sur terre)
* regarder les méthodes de pruning de dendogramme utilisées en génétique/phylogénie
* comparer les 4 saisons (SaisonType90)
* faire aussi tourner les SOM avec données corrigées par effort (captures/Eff2) (hypothèse de départ = pêcheurs pêchent là où il y a le + de poissons)
* demander à Daniel projet Esther avec timeline introduction nouvelles technologies (p.ex. 2010 échosondeur)
# 19 février
* écrire rapport activité, pour garder une trace de ce que j'ai testé et quels choix (méthodes et data) on a faits --> pour mercredi prochain
* essayer de fixer l'échelle de couleurs dans les heatmaps pour meilleure comparaison entre espèces
* Essayer d'identifier dans les clusters les abondances par espèces (p.ex. cluster 1 forte abondance BET en début d'année etc)
* filtrage données: regarder variance dans CPUE par strates d'efforts de pêche --> p.ex. si pour un jour de pêche la variance de CPUe est très grande (peut être dû à l chance), éventuellement retirer données eff2<1 jour etc. (article Daniel tag shedding océan indien)
* par contre, nouvelle méthode clustering (dynamicTreeCut) semble exclure d'elle-même les outliers. --> à creuser, à ce moment-là il ne serait pas forcément nécessaire de le faire en aval (https://academic.oup.com/bioinformatics/article/24/5/719/200751)
* définitions saisons: regarder par périodes (pour création années types), et comparer abondance relative VS captures VS CPUE --> Loreleï va m'envoyer le script de Gipsy qui avait fait ça pour le bigeye 
# 24 février
* discussions basées sur le premier rapport que j'ai écrit et que je dois retravailler: intro, ajouter toutes les cartes géographiques des clusters (en annexe, avec sommaire pour trouver facilement)
* vérifier que les zones moratoires des années 2000 apparaissent bien dans les données brutes de l'ICCAT (cartes géographiques)
* faire une timeline de l'introduction des nouvelles technologies et des zones moratoires depuis les années 90 (attention aux erreurs dans les tableaux, regarder carnet) -> but = définir des périodes pour les années types plus ou moins homogènes (afin de voir l'effet des mesures sur les clusters spatio-temporels)
* demander données Fr+Es pour estimer des proportions de juvéniles par zones géographiques (1x1 ou 5x5)
* échosondeurs: Es 2009, Fr 2010
* 2006: plus d'accords de pêche avec le Sénégal
* Mauritanie: 2012
# 3 mars
* topo data flow de l'ICCAT (brutes --> T3 --> ECD --> ICCAT)
* discussion sur quelles données on va utiliser pour les proportions de juvéniles:
* checker données ICCAT T2_SZ et T2_CZ, peut-être que ça va suffire 
* échantillonages pas vraiment aléatoires et couvre pas du tout toute la zone
* problème T3: lisse trop les proportions, pas génial pour nous
* autre considération: variation de la proportion des gos au fil des années, peut-on appliquer la même sur une période type, ou toutes les périodes?
* a faire: tableau résumé des captures à l'intérieur des zones moratoires pendant les moratoires
# 25 mars
* doc ICCAT résumé respect (ou non) des zones moratoires depuis leur introduction 
  * faire histogrammes par périodes et pays (inside VS outside), cartes moratoires
  * premier draft pour envoyer à Mauricio 
* corrections ppt pour conférence CEMEB
* discussion données espèces accessoires: 
  * Papier de Manocci pas référence espèces à protéger
  * A faire: recherche biblio, liste totale et shortlist des espèces accessoires avec statut IUCN et autres infos si nécessaire
  * aussi chercher sources de données potentielles, p.ex. cartes de distribution
* discussion sur cartes années et saison types sur périodes moratoires:
  * comparer clusters de période en période
  * refaire tourner avec CPUE pour voir si clusters tjrs différents (91-98 VS 99-03)
  * quand moatoires respectés pas clair si effets du moratoire ou de changements environnementaux sur les clusters
  * si pas respectés mieux pour nous (merci le Ghana)
* présentation générale des outputs: 
  * associer boxplots par clusters (colorés avec même couleurs) aux cartes en plus des timeseries
  * timeseries par espèces: ne pas utiliser des couleurs, plutôt linetype, sinon perturbant car couleur=cluster
* discussion juvéniles et T3
  * appliquer proportions T3+ aux données d'entrée SOM (juvénile BET, juvénile YFT, SKJ, espèces accessoires)
  * comme ça aussi au lieu de zones d'interdiction, zones de recommendations à la pêche
 # 12 avril
 [Meeting 12 avril.docx](https://github.com/LGuery/teamwork_monitoring/files/6303591/Meeting.12.avril.docx)
 # 4 mai
 * tester data flow et méthodes sur jeu de données iris
 * simuler datasets thons avec et sans hotspots, d'une ou plusieurs espèces, pour voir si la méthode les détecte
 * reprendre script et visualiser données après chaque étape (+ schéma data flow pour clarification) + stats descriptives (prop. par espèces etc)
 * prendre somme, pas médiane, et log1p pas log10
 * CPUE brutes 5x5 marlins pêcheries japonaises à chercher dans stock assessment
 * OBJECTIF 18 juin: tous résultats, plus d'analyses à faire tourner, squelette papier
 * multiplier indice abondance requins pour que ça ressemble à du tonnage
  # 11 mai
 * refaire tourner script (DataFlow_SOM_May) avec données FAD (pas en incluant FSC, cependant ça nous a permis de tester la méthode sur un cluster connu, gros bancs libres YFT, et de voir sur quelles données et avec quel clustering ça marchait le mieux ! erreur pas si énervante finalement)
 * ajouter à ce script un center/scale sans log1p() avant
 * Eff2 valeurs <1 alors que captures qd mm significatives --> Daniel a envoyé un email à Carlos, il se trouve que ce sont les données du Ghana
   * sinon envoyer mail à l'ob7 (laurent et mathieu)
 * pour simulation: tester ajouter cluster BET avec fourchette de valeurs plausibles, càd tonnage bien inférieur au SKJ --> ce cluster sera-t-il détecté ?
 * regarder publications pour voir si papier SOM purement méthodo / comparaison méthodos
