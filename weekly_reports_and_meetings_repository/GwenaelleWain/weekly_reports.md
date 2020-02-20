# Weekly Reports

## IE IRD - CPUE dFADs
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

