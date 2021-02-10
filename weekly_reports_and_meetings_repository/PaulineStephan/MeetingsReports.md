# Meetings
* [25 janvier](#25-janvier)
* [3 février](#3-février)
* [10 février](#10-février)
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
