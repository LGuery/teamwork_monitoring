# Weekly Reports

### IE IRD - CPUE dFADs
* [20 December 2019](#date-20th-december-2019)
* [27 December 2019](#date-27th-december-2019)
* [3 January 2020](#date-3rd-january-2020)
* [10 January 2020](#date-10th-january-2020)
* [17 January 2020](#date-17th-january-2020)


-------------------------------------------------------------------
### Date: 20th December 2019


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
  * LG: ProblÃ¨me rÃ©solu?

#### What would you like to work on next week?

* Work on data.
* Start a report on Markdown (Intro)

#### Where do you need help from Daniel, LoreleÃ¯ or others?

* IDK

#### Any other topics

* 

### Date: 27th December 2019


#### Who did you help this week?

* Personne

#### Who helped you this week?

* Daniel et LoreleÃ¯ pour la mise en route des analyses
* Philippe m'a prÃ©sentÃ© le jeu de donnÃ©es observateurs
  * LG: Parfait! N'hÃ©site pas Ã  prendre des notes pour la mÃ©moire pour plus tard :blush:

#### What did you achieve?

* RÃ©installer PostGre SQL.
* CrÃ©ation d'un projet RMarkdown pour faire les analyses du jeu de donnÃ©es.
* SÃ©paration du jeu de donnÃ©es en deux. 

  * LG : ImpÃ©ccable, pas de souci particulier (choix de traitement de donnÃ©es par exemple)?
  * GW : J'ai quelques questions comme convenu hier, j'organise une présentation pour en discuter

#### What did you struggle with?

* 

#### What would you like to work on next week?

* Continuer les analyses exploratives du jeu de donnÃ©es

#### Where do you need help from Daniel, LoreleÃ¯ or others?

* 

#### Any other topics

* 

### Date: 3rd January 2020


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

  * LG: Bravo! :clap: N'oublie pas de garder une trace de tes requÃªtes et autres... 

#### What did you struggle with?

* PostGre SQL : impossible d'ouvrir les schemas crees precedement. J'ai ete oblige de rentrer a nouveau l'integralite des jeu de donnees. Probleme resolu.

#### What would you like to work on next week?

* Continuer les analyses du jeu de donnees

#### Where do you need help from Daniel, LoreleÃ¯ or others?

* 

#### Any other topics

* 

### Date: 10th January 2020


#### Who did you help this week?

* Personne

#### Who helped you this week?

* Loreleï, Daniel et David lors de la présentation des premiers résultats afin de partir sur de nouvelles analyses 

#### What did you achieve?

* J'ai préparé une rapide présentation des premiers résultats.  
* Ajout des scripts et query dans mon repository
* Lecture de la biblio sur le package sf
* Création d'une première carte avec ce package
* Présentation des premiers résultats (refaire les analyses avec les données de logbook)
* J'ai repris les join afin de vérifier qu'il n'y avait pas d'erreur

#### What did you struggle with?

J'ai utilisé les données logbook pour lesquelles j'avais un identifiant de bouée soit 45205 lignes. Après le join et suppression des doublons, j'ai toujours 45205 lignes. J'ai vérifié à la main plus de 30 lignes pour regarder l'accès à l'info et il ne semble pas y avoir d'erreur.
Pour autant j'obtiens les résutats suivants : 
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
	        <td>Nombre de calés accès info = t</td>
	        <td>886</td>
	        <td>3733</td>
	        <td>4817</td>
	        <td>6527</td>
	        <td>7326</td>
	        <td>6014</td>
	        <td>230</td>
	    </tr>
	    <tr>
	        <td>Nombre de calés accès info = f</td>
	        <td>583</td>
         <td>1340</td>
         <td>2020</td>
         <td>2241</td>
         <td>2310</td>
         <td>3221</td>
         <td>3956</td>
	    </tr>
 <tr>
	        <td>Nombre de calés total</td>
	        <td>1469</td>
         <td>5073</td>
         <td>6837</td>
         <td>8726</td>
         <td>9636</td>
         <td>9235</td>
         <td>4186</td>
  </tr>
  <tr>
	        <td>Nombre de calés t/f</td>
	        <td>1,52</td>
         <td>2,79</td>
         <td>2,38</td>
         <td>2,91</td>
         <td>3,17</td>
         <td>1,87</td>
         <td>0,06</td>
  </tr>
 <tr>
	        <td>Pourcentage de calés accès info = t</td>
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

* Récupérer les données de logbook contenant les informations sur les prises. Reprendre les analyses en utilisant ces données.

#### Where do you need help from Daniel, LoreleÃ¯ or others?

* 

### Date: 17th January 2020


#### Who did you help this week?

* Personne

#### Who helped you this week?

* David : explication des analyses sur l'appartenance des bouées  

#### What did you achieve?

* A partir des données logbook de Laurent :
  * Séparation du jeu de données 
  * Analyse des différents types d'actions
  * Analyse des calés
* A partir des données t3 de David :
  * Analyse graphique des calés (par années, par trimestres)
* Bibliographie
* Ecriture de quelques idées pour une intro

#### What did you struggle with?

*

#### What would you like to work on next week?

* Lancer les analyses sur les données de captures sur les données t3
* Commencer à travailler sur les scripts de standardisation des CPUEs

#### Where do you need help from Daniel, LoreleÃ¯ or others?

* 

#### Any other topics

* 

-------------------------------------------------------------------

