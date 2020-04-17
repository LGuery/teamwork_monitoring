# Weekly Reports

## IE IRD - CPUE dFADs
* [17 April 2020](#date-17th-April-2020)
* [10 April 2020](#date-10th-April-2020)
* [3 April 2020](#date-3rd-April-2020)
* [27 March 2020](#date-27th-march-2020)
* [20 March 2020](#date-20th-march-2020)
* [13 March 2020](#date-13th-march-2020)
* [6 March 2020](#date-6th-march-2020)
* [28 February 2020](#date-28th-february-2020)
* [20 February 2020](#date-20th-february-2020)
* [14 February 2020](#date-14th-february-2020)
* [7 February 2020](#date-7th-february-2020)
* [31 January 2020](#date-31st-january-2020)
* [24 January 2020](#date-24th-january-2020)
* [17 January 2020](#date-17th-january-2020)
* [10 January 2020](#date-10th-january-2020)
* [3 January 2020](#date-3rd-january-2020)
* [27 December 2019](#date-27th-december-2019)
* [20 December 2019](#date-20th-december-2019)

-------------------------------------------------------------------
## Date: 17th April 2020

#### Who did you help this week?

* Personne 

#### Who helped you this week?

* Personne

#### What did you achieve?

* Document sur les histogrammes 
* GAM en prenant en compte l'interaction entre les coordonnées et la catégorie
* Regarder les proportions des différents modèles de bouées
* Regarder la différence entre les BO et les BL

#### What did you struggle with?

* Exporter l'article car le package tmap ne fonctionne pas sur la nouvelle version de R. Comme discuté ce matin je vais essayer de télécharger un version plus ancienne.

#### What would you like to work on next week?

* Essentiellement sur le papier. Reprendre les commentaires de David. Modifier les tableaux pour les faires apparaître via des codes.
* Faire les nouvelles analyses demandées sur les espèces.

#### Where do you need help from Daniel, Lorelei or others?

#### Any other topics

#### Weekly meeting du 17/04

Effet sur les espèces : 

* L'idée est de regarder si les échosondeurs ont les mêmes effets sur les trois espèces. Pour cela, on va faire tourner deux modèles.
* GLM : catch_per_species_per_set ~ cwp55 + period + year + numbat + category * specie
* Modèle multinomial : espece_dominante ~ cwp55 + period + year + category + numbat
* Mettre les boxplot des captures par catégories et par espèces

Article : 

* Reprendre l'article 
* Modifier le YALM pour correcpondre au journal

## Date: 10th April 2020

#### Who did you help this week?

* Personne 

#### Who helped you this week?

* Victor : rappel de comment il a comparé les histogrammes dans ses analyses

#### What did you achieve?

* Intégrer tous les résultats et rédaction de l'article
* Préparation de la présentation de l'article du 9 Avril
* Ajout des tables des stepAIC dans l'article
* Modification de la partie matériel et méthode pour la partie attribution des bouées
* Modification du graphique du GAM
* Histogrammes avec différentes échelles

#### What did you struggle with?

* 

#### What would you like to work on next week?

* Faire la comparaison des histogrammes entre F et O+E
* Regarder la fraction de calées supérieures à 50 t et à 100t
* Avancer sur la partie discussion du papier
* Regarder la proportion des différents modèles de bouées
* Refaire le GAM en prenant l'interaction entre les coordonnées et la catégorie. Uniquement sur 2012-2017

#### Where do you need help from Daniel, Lorelei or others?

#### Any other topics

#### Weekly meeting 

Réunion pour préparer la visio du groupe  DCP :

* Modifier le titre de l'article
* Mettre tous les auteurs
* Lors de l'introduction bien parler de l'augmentation de la puissance de pêche liée aux échosondeurs
* Dans les titres de graphes et des cartes bien préciser capture médiane par calée
* Revoir la partie attribution des bouées
* Pour le nombre de calées positives, ne pas se focaliser sur l'année 2017 mais sur la forte augmentation les années précédentes
* Pour le graphe de sortie du GAM remettre les années
* Pour les résultats des GAM et GLM donner le coefficient et le pourcentage. Ajouter le tableau des anova.
* Regarder les cartes avec des cellules de 1°

Retours de la réunion DCP sur l'article :

* Attention à l'utilisation du terme calées nulles, vérifier la définition
* Mieux analyser les histogrammes
* Pour les captures médianes, voir pour faire des boîtes à moustache. Essayer de faire des comparaisons entre années et catégorie.
* Intéressant de regarder l'effet des modèles de bouées
* Intéressant de regarder si l'effet des échosondeurs est le même sur toutes les zones
* Comme pour les petites calées, regarder les proportions pour les grandes calées

Weekly meeting du 10/04 : 

* Mettre le document Rmarkdown et les documents annexes sur github
* Refaire les graphiques avec les grosses calées
* Pour le nombre de calées, ajouter un panneau avec les proportions
* Pour regarder l'effet spatial : refaire le GAM en prenant en compte l'interaction entre les coordonnées et la catégorie. Permettra de voir si des zones spatiales ressortent avec des coefficients différents.

## Date: 3rd April 2020

#### Who did you help this week?

* Personne 

#### Who helped you this week?

* Personne

#### What did you achieve?

* Correction de David sur l'intro du papier + compléter les infos
* Reprise du document résultats : ajout des tableaux récapitulatifs des analyses précédentes
* Information sur les cellules qui ressortent sur les cartes 
* Commencer à reprendre le papier pour la présentation du 9 Avril
* Faire tourner les 3 modèles discutés lors de la réunion du 27 Mars

#### What did you struggle with?

* 

#### What would you like to work on next week?

* Reprendre le papier et préparer la présentation du 9 Avril
* Faire tourner les nouveaux modèles 
* Lire le second article envoyé par Daniel

#### Where do you need help from Daniel, Lorelei or others?

#### Any other topics

#### Weekly meeting du 03/04

Conclusions sur les modèles précédents : 

* Le GAM montre une première partie de courbe qui augmente fortement puis une sorte de plateau. On peut donc distinguer deux phases : une phase d'apprentissage puis une phase d'utilisation des échosondeurs
* Ce modèles est à garder des les analyses

Modèles à tester :

* Faire un modèle GAM et l'équivalent GLM uniquement sur la période 2012 - 2017
* Ne pas prendre en compte l'interaction entre l'année et la catégorie dans les deux modèles
* Pour le GLM utiliser cwp55. Cela permettra aussi de regarder si l'indice spatiale utilisé modifie les résultats

Article : 

* Mat et mét : données 	

	* Explication de la suppression de la cwp55 avec 2 calées + mise en annexe de la cartographie sur laquelle on la voit
	* Tableau reprenant les bateaux avec les années de présence et le nombre de calées. Mettre en annexe les résultats du GAM avant suppression des deux bateaux. Permet de justifier la suppression des deux bateaux.
	
* Résultats : 

	* Graphe des calées nulles 
	* Graphe + tableaux sur le nombre de calées positives
	* Capture médiane par année. Voir pour mettre soit les captures médianes sans les intervalles ou les captures moyennes avec les écarts à la moyenne ou des boxplots
	* GAM total_catch~s(long,lat)+s(years)+s(years, by=category)+category+numbat+period. Parler des deux phases pour justifier les modèles suivants 
	* GAM sur 2012 - 2017 sans prendre l'interaction entre l'année et la catégorie
	* GLM 2012 - 2017 sans prendre en compte l'interaction et en prenant cwp55
	
* Discussion 

	* Calées inférieures à 25 t et calées inférieures à 10 t. Met en avant une évolution dans le choix des DCP ? Graphe en annexe
	* Eventuellement histogramme des captures sur toutes les années par catégorie. Graphe en annexe
	* Renvois aux cartes en annexe
	
* Annexes : 

	* Carte du début avec la cellule qui ressort (justification du retrait)
	* GAM avec les deux bateaux (justification du retrait)
	* Cartographie
	
Données : 

* Retrait des deux bateaux qui interviennent uniquement en 2010 - 2012. Ils ne sont pas utiles pour la comparaison qui nous intéresse.


## Date: 27th March 2020

#### Who did you help this week?

* Personne 

#### Who helped you this week?

* Victor : choix du package pour les GLMM. Compréhension de l'erreur affichée en sortie.

#### What did you achieve?

* Document résultats : corrections + mise en annexe des anciennes parties
* Histrogramme des captures par catégories et par années pour regarder si on voit un seuil à 25t.
* Identification des outliers et des paramètres responsables.
* Modèles GLM avec et sans l'intéraction entre l'année et la catégorie
* Modèles GLMM avec et sans l'intéraction entre l'année et la catégorie
* Article : reprise de l'introduction en divisant en 3 parties :

	* Contexte de l'étude : état des connaissances 
	* Enjeux scientifiques : cadre de l'étude, questions associées, les études actuelles ont déjà répondues à ces questions ? 
	* Stratégie d'étude : données utilisées, hypothèses de travail, objectifs et résultats attendus

#### What did you struggle with?

* Les erreurs en sortie des GLMM

#### What would you like to work on next week?

* Continuer d'écrire l'article 
* Bibliographie 
* Faire les modifications 
* Faire tourner les 3 modèles 

#### Where do you need help from Daniel, Lorelei or others?

#### Any other topics

#### Weekly meeting du 27/03

Pour le document : 

* Ajouter les tables pour résumer les résultats des différents modèles testés

Pour les outliers : 

* Ne retirer que les outliers qui tombent dans la cellule avec deux calées
* Faire le plot des résidus à la main 
* Faire les predict pour toutes les années 
* Regarder les petites calées 

Pour les cwp55 qui ressortent sur les cartes :

* Regarder la proportion de chaque bateau

Modèles déjà faits :

* Lorsque l'on fait le GLM avec l'intéraction entre l'année et la catégorie, les coefficients sont trop proches entre les deux catégories --> pas d'interprétation possible
* Il semble qu'il y ait un poids trop important des numbat et cwp55

3 modèles à tester : 2 GAM et 1 GLM 

* Remplacer les années par des valeurs de 0 à 7. Cela permet d'interpréter directement les coefficients
* Le GAM montre des effets presque linéaire pour tous les paramètres --> on peut donc passer sur un GLM
* Regarder si on peut faire une ANOVA sur les GAM pour regarder si tous les paramètres sont significatifs
* gam : s(lon x lat) + s(year, by=category) + category + numbat + period
* gam : s(lon x lat) + s(year) + category + numbat + period
* Ne pas faire de transformation sur les prises
* Variables continues : year, lon et lat
* Variables catégorielles : category, numbat, period et cwp55

	* ## LG: :+1: Super, vraiment bien détaillé et clair. Continue! :+1:

## Date: 20th March 2020

#### Who did you help this week?

* Victor : pour les figures et leur placement lors de l'export en pdf

#### Who helped you this week?

#### What did you achieve?

* Reprise de la bibliographie déjà faite pour faire la trame de la discussion
* Nouvelle biblio
* Ecriture d'idées pour la partie discussion
* Changement de la mise en page de l'article : une figure par page et à la fin du document

#### What did you struggle with?

#### What would you like to work on next week?

* Identifier les outliers
* Faire tourner les GLM et GLMM 
* Continuer l’article 

#### Where do you need help from Daniel, Lorelei or others?

#### Any other topics

#### Weekly meeting du 20/03

* Outliers : Identifier les outliers et leurs caractéristiques
* GLM : Faire tourner avec et sans l'intéraction (année * catégorie) + Comparer les résultats des deux et voir si on garde l'intéraction
* GLMM : Mettre l'effet numbat en aléatoire + Faire tourner avec et sans l'intéraction
* GAM : les laisser de côté pour le moment
* Article : Continuer l'écriture + Etre plus précise dans l'introduction + Développer les hypothèses et les objectifs généraux possibles + Ne pas faire apparaître les résultats sur les calées nulles

## Date: 6th March 2020

#### Who did you help this week?

* Yannick : discussion sur les résultats que l'on fait ressortir 

#### Who helped you this week?

* Yannick : discussion sur l'estimation des biomasses via les échosondeurs : les seuils qu'il est possible de détecter

#### What did you achieve?

* Remettre le document en ordre : Ajout de la partie de présentation + Mettre en annexe les analyses précédentes
* Mettre les NA sur les plots des calées nulles 
* Remplacer les noms de catégories
* Ajouter les déviations sur les erreurs dans le graphique des captures médianes
* Comparer les différents GLM
* Présentation du CDD lors de la réunion DCP
* Bibliographie
* Refaire les différents modèles GAM 
* Analyse des captures inférieures à 25t
* Article : Mise en forme via un template + Rédaction de l'intro + Insertion des premiers résultats

#### What did you struggle with?

 * 

#### What would you like to work on next week?

* Ecriture

#### Where do you need help from Daniel, Lorelei or others?

* 

#### Any other topics

* 
## Date: 13th March 2020

#### Who did you help this week?

#### Who helped you this week?

#### What did you achieve?

* Ecriture de l'article : écriture du résumé + écriture de la partie attribution des bouées + ajout des résultats + trame de discussion
* Bibliographie

#### What did you struggle with?

#### What would you like to work on next week?

* Continuer d'écrire l'artcile notamment la partie discussion 
* Recherche biblio

#### Where do you need help from Daniel, Lorelei or others?

#### Any other topics

#### Weekly meeting

## Date: 6th March 2020

#### Who did you help this week?

* Yannick : discussion sur les résultats que l'on fait ressortir 

#### Who helped you this week?

* Yannick : discussion sur l'estimation des biomasses via les échosondeurs : les seuils qu'il est possible de détecter

#### What did you achieve?

* Remettre le document en ordre : Ajout de la partie de présentation + Mettre en annexe les analyses précédentes
* Mettre les NA sur les plots des calées nulles 
* Remplacer les noms de catégories
* Ajouter les déviations sur les erreurs dans le graphique des captures médianes
* Comparer les différents GLM
* Présentation du CDD lors de la réunion DCP
* Bibliographie
* Refaire les différents modèles GAM 
* Analyse des captures inférieures à 25t
* Article : Mise en forme via un template + Rédaction de l'intro + Insertion des premiers résultats

#### What did you struggle with?

 * 

#### What would you like to work on next week?

* Ecriture

#### Where do you need help from Daniel, Lorelei or others?

* 

#### Any other topics

* 

#### Weekly meeting

Réunion DCP du 04/03/2020 : 

* Voir avec Yannick pour l'estimation des biomasses sous échosondeurs via les données acoustiques. Il semble que les échosondeurs poeuvent fournir des données qualitatives. 
* Les pêcheurs pensent que l'on pêche moins sous DCP. Il y a une publication de Francis qui montre que les captures diminuent (à vérifier).

## Date: 28th February 2020

#### Who did you help this week?

* Personne 

#### Who helped you this week?

* Personne

#### What did you achieve?

* Modifier les analyses :

  * Périodes basées sur les moussons 
  * Capture totale ne prenant en compte que les 3 espèces de thons
* Mettre les noms des colonnes et des légendes en anglais
* Regarder les résultat en ne prenant en compte que les années 2011 à 2014
* Bibliographie
* Ecriture : rédaction plus détaillée de la partie matériel et méthode

#### What did you struggle with?

 * 

#### What would you like to work on next week?

* Remettre en ordre le document en passant en annexe les parties non utiles et faire un paragraphe détaillé sur le jeu de données
* Faire les modification sur les analyses
* Faire les GLM en comparant les différents modèles
* Ecriture

#### Where do you need help from Daniel, Lorelei or others?

* 

#### Any other topics

* Je serais absente ce Lundi 2 Mars

#### Weekly meeting du 28/02

Généralité : 

* Ajouter un paragraphe qui décrit la table de données et les colonnes 
* Mettre NA pour OWN_ECHOSOUNDER en 2010 et NA pour OWN en 2015, 2016 et 2017
* Remplacer OWN par OWN-ECHO et OWN_ECHOSOUNDER par OWN+ECHO

Pour les graphes des captures par année : 

* Voir pour mettre les déviations sur les erreurs (STANDARD DEV ON MEAN OR ERROR)

GLM : 

* Comparer les résultat avec GAMMA link =identity et tansformation LOG + Gaussian
* Ajouter les facteurs numbat et cwp55
* Faire sortir la table d'ANOVA
* Mettre l'année en continue, la catégorie, la période en facteur, cwp55 en facteur et numbat en facteur

GAM : 

* Ajouer la variabe catégorie seule
* Regarder pour faire sortir la table d'anova
* Mettre la période en catégorielle
* Mettre l'année seule 
* Mettra la catégorie seule
* Mettre le nombre de points sous les graphiques
* Faire un predict des captures avec les trois catégories

## Date: 20th February 2020

#### Who did you help this week?

* Personne

#### Who helped you this week?

* Personne

#### What did you achieve?

* Bibliographie
* Refaire les GAM en mettant le numéro de bateau comme facteur 
* Choix du meilleur modèle GAM 
* Ecriture de la trame de l'article

#### What did you struggle with?

 * L'analyse des plots GLM : peut-on les analyser de manière robuste sachant que l'on utilise un inverse gamma ? 

#### What would you like to work on next week?

* Continuer d'écrire la trame du document
* Bibliographie

#### Where do you need help from Daniel, Lorelei or others?

* Prise de décision : 
  * Pour les trimestres : on reste sur les trimestre actuels (DJF-MAM-JJA-SON) ou on repasse sur les trimestres réels (JFM-AMJ-JAS-OND) ? 
  * Pour les captures totales : actuellement, on fait la somme des captures de toutes les espèces mais ne faut il pas regarder que les sommes des captures des 3 espèces principales de thons ? 

#### Any other topics

* Je serais absente ce Vendredi 21 Février

#### Weekly meeting 

## Date: 14th February 2020


#### Who did you help this week?

* Personne

#### Who helped you this week?

* Personne

#### What did you achieve?

* Modifier l'esthétique des graphiques (gris, nom de légende ...)
* Regarder la différence entre les captures sur bouées étrangères et sur bouées propres sans échosondeurs (Résultats différents selon le test)
* Faire un glm sur le ratio en groupant les FOREIGN et OWN
* Refaire les modèles GAM
* Faire les analyses :
  * En groupant FOREIGN et OWN
  * Sans grouper FOREIGN et OWN
* Bibliographie + écriture (mis sur github)
* Justification de l'utilisation du modèle GAMMA 

#### What did you struggle with?

 

#### What would you like to work on next week?

* Continuer d'écrire la trame du document
* Bibliographie
* VOir les modèles GAM en modifiant les bateaux et l'effort
* Faire des recherches sur l'utilisation des plot(glm) avec une loi gamma 

#### Where do you need help from Daniel, Lorelei or others?

* 

#### Any other topics

* 

#### Weekly meeting 

* GLM : 
  * Regarder si on peut analyser les résidus avec une loi GAMMA 
* GAM :
  * Voir la prise en compte des bateaux, les mettre en effet aléatoire ne fonctionne pas car il n'y a pas de hiérarchisation dans les numéros de bateaux
  * Regarder le fichier turbobat pour avoir plus d'infos sur les bateaux
  * Faire apparaître le nombre de calées sous les graphes pour avoir une idées de l'effort
  
## Date: 7th February 2020


#### Who did you help this week?

* Personne

#### Who helped you this week?

* Victor : comprehension de la fonction qui permet de tranformer les cwp55 en coordonnees.

#### What did you achieve?

* Reprise des graphiques et analyses (WM du 30/01)
  
  * Ramener les calees nulles / calees totales
  * Faire un graphique par annee avec les captures par trimestres
  * Faire une carte avec le nombre de calees par cellules
  * Refaire les cartes en prenant les cwp55 comme cellules
  * Faire un glm sur le ratio t/f par cellules par mois
  * Reprendre la partie sur les echosondeurs en divisant le jeu de donnees en 3
* Ecriture et envoie d'un pdf resume des premiers resultats 
* Bibliographie
* Realisation des modele GAM

#### What did you struggle with?

* Prise en compte des facteurs dans les modeles GAM 
  * Probleme resolu 

#### What would you like to work on next week?

* Changer les couleurs et les legendes des plots
* Reprendre les cartes de valeurs medianes par cellules de 5°
* Refaire les modèles GAM
* Refaire les plots des modeles glm
* Biblio pour regarder la difference entre ggeffect et ggemeans
* Ecrire une trame de papier

#### Where do you need help from Daniel, Lorelei or others?

* 

#### Any other topics

* 

#### Weekly meeting 

* Pour les analyses GLM : 
  * Il sera necessaire de justifier pourquoi utiliser un modele GAMMA plutot qu'un modele quasi-poisson
  * Verifier comment ggeffect prend en compte les valeur. Regarder si ggemeans n'est pas mieux
  * Faire en sorte que les plots sortent un à un et les analyser 
* Pour les modele GAM :
  * Mettre l'annee en continu avec un smooth
  * Mettre les numero des bateaux en aleatoire (car on ne s'interesse par à leur effet et donnera plus de poids aux autres facteurs)
  * Faire un modele en ajoutant les cwp55 et regarder s'il y  a un difference compare au long*lat
  * Faire les plots des modeles GAM
* Commencer a ecrire une trame pour le papier
* Commentaires de Daniel : 
  * Reprendre les gapphiques en retirant les couleurs et en modifiant les legendes :
    * TRUE = OWN
    * T+E = OWN-ECHOSOUNDER
    * FALSE = FOREIGN
  * Reprendre les captures medianes par cellules en zoomant sur la zone
  * Analyse GLM avec GAMMA et ratio 
    * Possible car les ratios ne peuvent pas etre negatifs
    
## Date: 31st January 2020


#### Who did you help this week?

* Personne

#### Who helped you this week?


#### What did you achieve?

* GLM avec numero de cellule de la grille 
* Premiere analyses des echosondeurs :
  * Evolution du nombre par an
  * Cartographie des annees avec assez de donnees (2011-2012)
  * GLM sur toutes les annees
  * GLM sur 2011-2012
* Bibliographie
* Ecriture d'un debut d'introduction (mis en ligne sur Github)
* GLM sur les ratios t/f en groupant les donnees par quinzaine

#### What did you struggle with?

*

#### What would you like to work on next week?

* Reprendre la partie sur les calees nulles
* Faire les graphique par trimestre 
* Faire une carte avec le nombre de calees par cellules 
* Voir les GLM et l'AIC
* Voir les GAM 
* Bibliographie 

#### Where do you need help from Daniel, Lorelei or others?

* 

#### Any other topics

* 

#### Weekly meeting 

* Pour les calees nulles : 
  * Ramener les calees nulles sur le nombre de calees total
* Pour voir s'il y a une saisonnalite dans les captures : 
  * Faire un graphique (t et f sur le meme graphique) avec les prise en fonction des trimestres pour chaque annee
* Pour les GLM : 
  * Ne mettre que le trimestre ou le mois. 
  * Regarder le type de distribution et pourquoi l'AIC ne fonctionne pas.
* Pour les graphique avec la grille : 
  * Faire une carte avec le nombre de calees par cellules
  * Reprendre la carte avec les captures medianes car les valeurs semblent tres importantes
* Faire des GAM de ce type :
  * S(own_fad * year) + S(year * trimestre) + S(long * lat)
  * Avec annee et trimestre en categoriels
  * Cela permet d'eliminer les variations spatio-temporelle et d'evaluer l'effet de balise et echosondeur
* Pour les analyses a venir, separer le jeu de donnees en 3 parties :
  * Peche sur une balise qui lui apprtient pas
  * Peche sur une balise qui lui appartient avec echosondeur
  * Peche sur une balise qui lui appartient sans echosondeur
* Pour les ratios :
  * Faire un ratio par cellule de 5*5 (cwp) par mois (evite les NA)
  * Faire un GLM avec annee, trimestre et cwp (factor)
* Envoyer par email un resume des resultats trouves jusqu'a maintenant 


## Date: 24th January 2020


#### Who did you help this week?

* Personne

#### Who helped you this week?

* Victor : prise de decision pour les donnees à expliquer (ratio, log(ratio), difference) pour les glm. 

#### What did you achieve?

* Refaire tourner les scripts avec les nouvelles donnees t3
* Ajout de la partie sur les calees nulles (en fonction des annnes, de t/f)
* Modification des graphes :
  * Retrait des calees nulles et de 2018
  * Regrouper t et f sur le meme graphe
  * Ajouter les ecarts types sur les graphes de moyenne
* Faire les memes graphes avec la mediane
* GLM : 
  * Ratio t/f --> facteur descriptifs mois, trimestre et annees
  * Difference t-f --> facteurs descriptifs mois, trimestre et annees
* Cartographies:
  * Cartographie t VS f
  * Cartographie en fonction des trimestres
  * Creation d'une grille de 1° * 1°
  * Calcul des données de capture dans les cellules

#### What did you struggle with?

*

#### What would you like to work on next week?

* Analyser l'effet spatial sur les donnees de capture
* COmparer les captures entre les donnees echosondeur et non echosondeur
* Lire la biblio envoyee par Daniel

#### Where do you need help from Daniel, Lorelei or others?

* 

#### Any other topics

* 

#### Weekly meeting 

Les analyses deja faites sont correctes. Il faut continuer d'utiliser les donnees fournies par David.

Pour limiter les biais dans les analyses : 

* Ragarder la fraction de calees nulles pour t et f
* Retirer les calees nulles 
* Retirer l'annee 2018

Pour avoir de meilleures estimations :

* Refaire les analyses en prenant la mediane
* Ajouter les ecarts types sur les graphes

Pour ameliorer la lecture des graphes : 

* Regrouper t et f sur le meme graphe
* Faire les graphes des ratios

Test statistiques : 

* Faire les tests statistiques en prenant le ratio t/f
* Faire une glm avec : annees, trimestres et zones geographiques en variables explicatives. Prendre l'annee en numerique et pas en facteur. cela permettrait de regarder s'il y a une evolution brutale ou si l'evolution se fait au cours des annees. Si l'evolution esr brutale et en 2012 : apparition des echosondeur. En revanche si l'evoltuion est progressive : meilleure utilisation des bouees d'annee en annee.

Regarder l'evolution spatiale de l'annee et/ ou du trimestre. Utiliser le packahe raster pour cela. 

## Date: 17th January 2020


#### Who did you help this week?

* Personne

#### Who helped you this week?

* David : explication des analyses sur l'appartenance des bouÃ©es  

#### What did you achieve?

* A partir des donnÃ©es logbook de Laurent :
  * SÃ©paration du jeu de donnÃ©es 
  * Analyse des diffÃ©rents types d'actions
  * Analyse des calÃ©s
* A partir des donnÃ©es t3 de David :
  * Analyse graphique des calÃ©s (par annÃ©es, par trimestres)
* Bibliographie
* Ecriture de quelques idÃ©es pour une intro

#### What did you struggle with?

*

#### What would you like to work on next week?

* Lancer les analyses sur les donnÃ©es de captures sur les donnÃ©es t3
* Commencer Ã  travailler sur les scripts de standardisation des CPUEs

#### Where do you need help from Daniel, LoreleÃƒÂ¯ or others?

* 

#### Any other topics

* 

## Date: 10th January 2020


#### Who did you help this week?

* Personne

#### Who helped you this week?

* LoreleÃ¯, Daniel et David lors de la prÃ©sentation des premiers rÃ©sultats afin de partir sur de nouvelles analyses 

#### What did you achieve?

* J'ai prÃ©parÃ© une rapide prÃ©sentation des premiers rÃ©sultats.  
* Ajout des scripts et query dans mon repository
* Lecture de la biblio sur le package sf
* CrÃ©ation d'une premiÃ¨re carte avec ce package
* PrÃ©sentation des premiers rÃ©sultats (refaire les analyses avec les donnÃ©es de logbook)
* J'ai repris les join afin de vÃ©rifier qu'il n'y avait pas d'erreur

#### What did you struggle with?

J'ai utilisÃ© les donnÃ©es logbook pour lesquelles j'avais un identifiant de bouÃ©e soit 45205 lignes. AprÃ¨s le join et suppression des doublons, j'ai toujours 45205 lignes. J'ai vÃ©rifiÃ© Ã  la main plus de 30 lignes pour regarder l'accÃ¨s Ã  l'info et il ne semble pas y avoir d'erreur.
Pour autant j'obtiens les rÃ©sutats suivants : 
<table>
	    <tr>
	        <th scope="col"> </th>
	        <th scope="col">2013</th>
         <th scope="col">2014</th>
         <th scope="col">2015</th>
	        <th scope="col">2016</th>
	        <th scope="col">2017</th>
	        <th scope="col">2018</th>
	        <th scope="col">2019</th>
	    </tr>
	    <tr>
	        <td>Nombre de calÃ©s accÃ¨s info = t</td>
	        <td>886</td>
	        <td>3733</td>
	        <td>4817</td>
	        <td>6527</td>
	        <td>7326</td>
	        <td>6014</td>
	        <td>230</td>
	    </tr>
	    <tr>
	        <td>Nombre de calÃ©s accÃ¨s info = f</td>
	        <td>583</td>
         <td>1340</td>
         <td>2020</td>
         <td>2241</td>
         <td>2310</td>
         <td>3221</td>
         <td>3956</td>
	    </tr>
 <tr>
	        <td>Nombre de calÃ©s total</td>
	        <td>1469</td>
         <td>5073</td>
         <td>6837</td>
         <td>8726</td>
         <td>9636</td>
         <td>9235</td>
         <td>4186</td>
  </tr>
  <tr>
	        <td>Nombre de calÃ©s t/f</td>
	        <td>1,52</td>
         <td>2,79</td>
         <td>2,38</td>
         <td>2,91</td>
         <td>3,17</td>
         <td>1,87</td>
         <td>0,06</td>
  </tr>
 <tr>
	        <td>Pourcentage de calÃ©s accÃ¨s info = t</td>
	        <td>60,3</td>
         <td>73,6</td>
         <td>70,5</td>
         <td>74,4</td>
         <td>76,1</td>
         <td>65,1</td>
         <td>5,49</td>
  </tr>
	</table>

#### What would you like to work on next week?

* RÃ©cupÃ©rer les donnÃ©es de logbook contenant les informations sur les prises. Reprendre les analyses en utilisant ces donnÃ©es.

#### Where do you need help from Daniel, LoreleÃƒÂ¯ or others?

* 

## Date: 3rd January 2020


#### Who did you help this week?

* Personne

#### Who helped you this week?

* Personne
  * LG: :disappointed: #vacancesscolairescouloirsvides?
  * GW : Exactement !! 

#### What did you achieve?

* Ajout des differents jeux de donnees sur PostGre SQL
* Creation de jointures entre ces jeux de donnees
* J'ai commence les analyses exploratoires sur les jeux de donnees

  * LG: Bravo! :clap: N'oublie pas de garder une trace de tes requÃƒÂªtes et autres... 

#### What did you struggle with?

* PostGre SQL : impossible d'ouvrir les schemas crees precedement. J'ai ete oblige de rentrer a nouveau l'integralite des jeu de donnees. Probleme resolu.

#### What would you like to work on next week?

* Continuer les analyses du jeu de donnees

#### Where do you need help from Daniel, LoreleÃƒÂ¯ or others?

* 

#### Any other topics

* 

## Date: 27th December 2019


#### Who did you help this week?

* Personne

#### Who helped you this week?

* Daniel et LoreleÃƒÂ¯ pour la mise en route des analyses
* Philippe m'a prÃƒÂ©sentÃƒÂ© le jeu de donnÃƒÂ©es observateurs
  * LG: Parfait! N'hÃƒÂ©site pas ÃƒÂ  prendre des notes pour la mÃƒÂ©moire pour plus tard :blush:

#### What did you achieve?

* RÃƒÂ©installer PostGre SQL.
* CrÃƒÂ©ation d'un projet RMarkdown pour faire les analyses du jeu de donnÃƒÂ©es.
* SÃƒÂ©paration du jeu de donnÃƒÂ©es en deux. 

  * LG : ImpÃƒÂ©ccable, pas de souci particulier (choix de traitement de donnÃƒÂ©es par exemple)?
  * GW : J'ai quelques questions comme convenu hier, j'organise une prÃ©sentation pour en discuter

#### What did you struggle with?

* 

#### What would you like to work on next week?

* Continuer les analyses exploratives du jeu de donnÃƒÂ©es

#### Where do you need help from Daniel, LoreleÃƒÂ¯ or others?

* 

#### Any other topics

* 

## Date: 20th December 2019


#### Who did you help this week?

* I helped Victor (create his mission order)

#### Who helped you this week?

* Victor helped on Github

#### What did you achieve?

* Create my repository on Github.
* Update bibliography, meetings on teamwork_monitoring.
* I read the CESAB formation.
* More bibliography.

  * LG: Super!

#### What did you struggle with?

* Downland MikTex or others and save my rmarkdown file in pdf.
  * LG: ProblÃƒÂ¨me rÃƒÂ©solu?

#### What would you like to work on next week?

* Work on data.
* Start a report on Markdown (Intro)

#### Where do you need help from Daniel, LoreleÃƒÂ¯ or others?

* IDK

#### Any other topics

* 

-------------------------------------------------------------------

