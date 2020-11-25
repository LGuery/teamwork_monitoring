# Weekly Reports

### Thèse IRD 

* [25 November 2020](#date-25th-november-2020)

* [23 November 2020](#date-23th-november-2020)

* [5 October 2020](#date-5th-october-2020)

* [28 September 2020](#date-21th-september-2020)

* [21 September 2020](#date-21th-september-2020)

* [14 September 2020](#date-14th-september-2020)

* [7 September 2020](#date-7th-september-2020)

* [13 August 2020](#date-13th-august-2020)

* [3 August 2020](#date-3rd-august-2020)

* [27 July 2020](#date-27th-july-2020)

* [13 July 2020](#date-13rd-july-2020)

* [3 June 2020](#date-3rd-june-2020)

* [27 April 2020](#date-27th-april-2020)

* [20 April 2020](#date-20th-april-2020)

* [13 April 2020](#date-13th-april-2020)

* [6 April 2020](#date-6th-april-2020)

* [30 March 2020](#date-30th-march-2020)

* [16 March 2020](#date-16th-march-2020)  

* [28 February 2020](#date-28th-february-2020)  

* [21 February 2020](#date-21th-february-2020)  

* [14 February 2020](#date-14th-february-2020)  

* [31 January 2020](#date-31th-january-2020)  

* [24 January 2020](#date-24th-january-2020)  

* [17 January 2020](#date-17th-january-2020)  

* [10 January 2020](#date-10th-january-2020)  

* [20 December 2019](#date-20th-december-2019)

* [12 December 2019](#date-12th-december-2019)  


-------------------------------------------------------------------  

### Date: 25th November 2020

# Semaine 4 (23-29)

* 

-------------------------------------------------------------------  

### Date: 23th November 2020

Update depuis 27 octobre:

# Semaine 3 (16-22)

* Lundi: correction rapport DPMA, bouclé le mercredi 18
* Lundi soir: réunion avec Sosthène pour travailler sur le papier corrections des FSC-SMO. Création d'un plan.
* Mardi réunion avec L&D : présentation du projet SMO avec Sosthène, discussions pour la réunion 1 an de thèse avec Matthieu.
* Mardi aprem: réunion #2 GEO Blue PLanet
* Mercredi : Vide intersidéral mis à part le summary DPMA
* Jeudi : REUNION 1 AN DE THESE PLANIFIEE POUR LE LUNDI 30 Novembre
* Vendredi: réunion logistique avec Pauline pour son stage.
* Venredi: Thierry galère a mettre les documents sur l'adum...ca prend du etard et ça m'inquiète !
* Week end: travai lavec Sosthène pour écrire l'abstract pour la soumission du papier SMO.

# Semaine 2 (9-15)

* Réunion le lundi pour parler papier Symposium et orga
* DATA perdues sur local heureusement récupérées sur HDD (pb Github à régler)
* Mardi retour sur site pour signer les avenants de contrats. 
* Mardi, contact avec David et l'assistance ifremer pour régler les pb de connexions à Pulse Secure et au cluster en distanciel.
* Mercredi : pb de pulse secure en passe d'être réglé.
* Jeudi : Pb Pulse secure réglé + participation première présentation GEO Blue Planet
* Vendredi  + Week end : Envoie documents école doc pour THierry + Ecriture rapport pour la DPMA


# 1ere semaine de confifi (2-8 novembre)

* Retour au ryhtme confinement un peu compliqué car malade, première réunion pour voir les objectifs d'ici la fin de l'année.
* Retrait du papier dans le Redbook ICCAT pour le garder pour le symposium
* Suivi de la conférence IA "Que veux dire apprendre pour une machine ?"
* Lecture du papier INLA sur la pêche thonnière Lezama-Ochoa et al., 2020 => utilisation de SPDE... On doit faire ça aussi !
* Contact avec Julien Ansquer pour le remboursement de l'état de frais => toujours au point mort



-------------------------------------------------------------------  

### Date: 5th October 2020

# SEJOUR A LA ROCHELLE SEMAINE 2

#### What did you achieve?

* **Lundi**: Discussion avec Matthieu. Présentation des premières sorties de modèle spatialisé et temporalisé, pour une année et pour tous les mois. Covariables: Effort continu, effet mois, effet bateau. Observation d'une zone où les estimations de capture sont overestimées (2000000 t !).

Besoin de tester de nouveaux modèles pour l'effet mois,  random walk 1 ou iid.

* **Mardi**: Test de iid, impossible de faire tourner. Rw1 fonctionne pour l'effet mois, pas d'utilisation de custom priors. Toujours des surestimations du modèle impossible d'avoir des estimations fiables. Premier test, mettre des NA sur les cellules qui ne sont pas sur terre. Toujours un effet de bord.

* **Mercredi**: Test avec des priors semi-normaux pour contraindre la variance. Pas d'effet intéressant sur les valeurs prédites non plus. Réunion avec Lorelei et Daniel en Skype: Proposition de 1) Virer les UNK et les FSC des données, pour exclure les zéros des Captures de Juv, 2) Virer les données qui sont trop excentrées de la zone (Est Inde, Mer Rouge), 3) Travail sur la Mesh et son buffer.

Idées : Comparer les zones à faible et forte densité de DCPs.

* **Jeudi**: Travail sur la mesh. J'ai réussi à contraindre la mesh le long des côtes du bassin indien. Réduction du bffer au minimum pour limiter les mauvaises estimations mais toujours impossible. Quelques pixels sont largement surestimés en bordure. Abandon de la méthode SPDE; ne trouvant pas de solution. Retour sur le spatial Besag (champ discret)


* **Vendredi**: Difficultés avec le spatial Besag, problème d'identité des cellules et de création de la matrice d'adjacence. Solutions présentes dans le script, le modèle tourne et donne des résultats satisfaisants. Cependant, besoin de trouver une moyen d'intégrer l'effet mois sur la grille.


> **LG**: Excellent, excellent! Super encourageant! :clap: :clap: :clap: On se fait un point/debrief quand tu rentres de vacances, profites bien!



-------------------------------------------------------------------

### Date: 28th September 2020

# SEJOUR A LA ROCHELLE SEMAINE 1

#### What did you achieve?

* **Lundi**: Première réunion avec Lola Gilbert sur son rapport de stage de M2. Discussions autour de 2 méthodes d'estimation de l'effet spatial par INLA: Besag (CAR model) ou SPDE.
Réu avec Matthieu avec l'après midi. Présentation des données ECD à Matthieu, des données environnementales disponibles. Plusieurs questions posées :
 + quelle méthode pour le spatial ? => objectif création de la maille pour le CAR et de la mesh SPDE. 
 + contact avec l'Ob7 pour correction des positions réelles des activités de pêche (problème (d'en)quadrant + conversion).
 + réflexions à avoir sur les hypothèses de modélisation (effet des covariables change-t-il avec le temps ? Restent fixes ? ; Mois par mois ou sélection de périodes; année en effet aléatoire ?)

* **Mardi**: Construction des mailles. Bibliographie sur les deux méthodes.

* **Mercredi**: Finition de la maille spde pour le modèle spatio temporel.
Réunion skype avec Lo&Da. 
 + Décision de se concentrer sur la méthode SPDE car le continu est intéressant dans notre cas car on ne doit pas faire d'hypothèse sur l'autocorrélation spatiale entre les cellules.
 + Choix d'une approche plutôt hotspot -> habitat. Car dans l'objectif de la gestion, une zone d'habitat sans pêche n'est pas une zone de hotspot, et on a pas de données.
 + Question sur l'utilisation de GLM ou de GAM pour l'effet des variables environnementales. Pour l'instant GLM puis utilisation de GAM si besoin plus tard.
 
 + Inclusion du Nb de callée/jour comme proxy de l'effort. Inclusion de variables propres au bateau (capacité, âge..) plus tard, comme pour CPUE.
 
 + Effet année en aléatoire
 
 + Utilistation de la denstié de DCP ? A voir.
 
 + Mois comme effet temporel et spatial car les changements saisonniers ne sont pas uniformes sur la zone d'étude => interaction du mois sur la mesh
 
 
* **Jeudi**: Construction du modèle INLA sans effet spatial. Premier run rapide, moins de 90 secondes. Bons résultats de fit, similaires à un GAM avec l'effort + mois + annee + bateau en covariables. 

* **Vendredi**: Soutenance HDR de Jérôme Spitz, pas de travail le matin. Réunion avec Matthieu pour essayer d'intégrer le spatial. Crash de INLA. A voir ce week end et lundi.

 



-------------------------------------------------------------------



### Date: 21th September 2020

#### Who did you help this week?

* Nobody

#### Who helped you this week?

* No one loves me

#### What did you achieve?

* Organistation du séjour à LR + moult biblio sur INLA et la modélisation spatio-temporelle avec inférence bayésienne:

### What's INLA?

INLA (Integrated Nested Laplace Approximation) is an algorithm for fitting Bayesian models. It is differently built than the traditional MCMC algorithm: it is way faster for multidimensional integration, but attention has to be taken on the error and uncertainty.

It allows to deal with the spatial autocorrelation, a common issue in ecological sciences:
“Everything is related to everything else, but near things are more related than distant things.”

INLA has default priors for all the effects in the model but they can and should be changed to control the analysis.

### Building

INLA is built to fit Latent Gaussian Models (LGM) that are a wide class of models used in spatial ecology. A LGM consits of 3 levels:  the observations ($y$), an underlying latent structure/filed ($\eta$) and a vector of hyperparameters ($\theta$).

(A hyperparameter is a parameter from a prior distribution; it captures the prior belief, before data is observed (Riggelsen, 2008). For example, the hyperparameter η is a prior guess for the mean (μ) of some distribution X. Although the prior distribution can’t normally be described in full, it’s sometimes possible to make reasonable guesses about the distribution’s hyperparameters and thus construct a reasonable distribution.) 
  In INLA, the latent field is approximated by a Gaussian Markov random field (GMRF), i.e. a discrete approximation of the continuous Gaussian field on a spatial grid. It means that all the combination of random variables are centered. 
In  summary,  the  structure  of  the  latent  Gaussian  model allows INLA to speed up the fitting process by exploiting the fact that the latent field is Gaussian such that a Laplace approximation may be used. In practice, this implies that INLA is fast.

INLA is **deterministics**, compared with MCMC.
 
INLA is computationally efficient because it uses a SPDE (Stochastic Partial Differentiation Equation) to estimate the spatial autocorrelation of the data. This involves using a “mesh” of discrete sampling locations which are interpolated to estimate a continuous process in space.
 
## Model selection

There are no P values in INLA. Importance or significance of variables can be deduced by examining the overlap of their 2.5% and 97.5% posterior estimates with zero.

Must not include higly-correlated covariates.

Need to build everal models were you set constant correlation in area or time. And then you can add random effects of some covariables.

The selection of model is done using DIC or WAIC. But WAIC seems to be preferable for Bayesian models.

### Interests

Very fast for complex datasets.

** SOME USEFUL LINKS **

https://ourcodingclub.github.io/tutorials/inla/

https://www.precision-analytics.ca/blog/a-gentle-inla-tutorial/

#### What did you struggle with?

* C'était galère de comprendre le fonctionnement d'INLA, notamment la partie Latent Gaussian Model et Random Markov Gaussian Fields.

#### What would you like to work on next week?

* Boulot, boulot sur INLA

#### A faire pour l'avenir


#### Any other topics 



-------------------------------------------------------------------


### Date: 14th September 2020

#### Who did you help this week?

* Nobody

#### Who helped you this week?

* No one

#### What did you achieve?

* Reunion ICCAT dun lundi au mercredi. Présentation.

* Préparation du voyage à La Rochelle: OM + contact avec équipe gestion CNRS MARBEC

* Idées pour le papier ICCAT rentrées sur le document. Ces idées serviront à reprendre après le séjour à LR et les congés.



#### What did you struggle with?


#### What would you like to work on next week?

* Lecture de la litterature pour préparer le déplacement à La Rochelle

#### A faire pour l'avenir


#### Any other topics 



-------------------------------------------------------------------

### Date: 7th September 2020

# WHAT HAPPENED LAST 2 WEEKS

#### Who did you help this week?

* Nobody

#### Who helped you this week?

* Loreleï et Daniel pour la production du super papier ICCAT ;)  

#### What did you achieve?

##### Paper
* Fini le papier ICCAT, ajouté une partie des méthodes sur le matching.

* Présentation terminée pour le Groupe Espèce.

#### What did you struggle with?

* Avec le papier, plus long à écrire que prévu. Quelques efforts à fournir à l'avenir

* Décès dans la famille.

#### What would you like to work on next week?

* Lecture de la litterature pour préparer le déplacement à La Rochelle

* Biblio sur les Species Distribution Model
#### A faire pour l'avenir


#### Any other topics 



------------------------------------------------------------------- 
### Date: 13th August 2020

# SUMMARY OF ADVANCE ON ICCAT PAPER

#### Who did you help this week?

* Nobody

#### Who helped you this week?

* Nicolas Barrier for datarmor use: Learn how to Download files from $SCRATCH to local using a eftp connection.

#### What did you achieve?

##### Paper
* J'ai conclu les méthodes et les ai réadaptées à ce qui a réélement été fait. Bonne avancée de l'intro, mais j'hésite à aller plus loin. Peur de faire doublon avec ce que Gipsy a déjà vu que c'est la même étude ou presque. 

Toujours pas de résultats, mis à part ce que j'avais initialement pour le morat Rec15.

* Lecture approfondie de Fonteneau et al 2015, Hallier & Gaertner 2008 + papier d'Edgar pour l'intro

#### What did you struggle with?

* Encore le cluster... 5 échecs à faire tourner le moratoire 1998. J'ai changé le script, modifié le job à plusieurs reprises. Il tourne désormais longtemps (10h) mais est killé à la fin. J'ai modifié encore le job et verrai les résultats. POur l'instant, aucune autre piste de débogage...

* Gros doutes sur l'intention du papier, à discuter dès la rentrée si possible.

* Baisse de régime la semaine passée, rupture en cause, mais on est reparti.

#### What would you like to work on next week?

* VACANCES
* Lecture de littérature à faire, je n'ai pas donné assez de temps pour ça et c'est TRES MAL. Je manque encore de plein de connaissance pour pouvoir faire mes propres conclusions sans me fourvoyer.

* 4 jours d'écriture intensive au retour de vacances pour terminer ce papier.

#### A faire pour l'avenir

* Mettre en place la randomisation pour tester le RR pour le papier final
* Appliquer la méthode aux hotspots si possible => mais PB de données ?
* Utilsier les données d'effort pour évaluer si le moratoire est réellement efficace à long terme.

#### Any other topics 



------------------------------------------------------------------- 

### Date: 3rd August 2020

#### Who did you help this week?

* Nobody

#### Who helped you this week?

* Nobody

#### What did you achieve?

* FINALLY succeed to run RR computation script on the Datarmor cluster. The error was because of the R version I used locally was superior to the one loaded on the cluster. The `dplyr::bindrows()` function returned an error because it was not able to bind factor columns (re_MOIS). Changing the class from factor to character resolved the pb.

* Great SMO meeting: see report in the meetings reports section

#### What did you struggle with?

* Cluster, but it works now !

* MY TOOTH WERE HURTING. Hard to work on Friday.

#### What would you like to work on next week?

* Read bibliography for the ICCAT paper

* Finallise results, run randomization test on RR

#### Where do you need help from Daniel or others?


#### Decisions made during meetings


#### Any other topics 



------------------------------------------------------------------- 
### Date: 27th July 2020

#### Who did you help this week?

* Nobody

#### Who helped you this week?

* Friday Loreleï for datarmor uses

#### What did you achieve?

* CISEF Bayesian courses from Tuesday to Thursday

#### What did you struggle with?

* Cluster, can't run my scripts..

#### What would you like to work on next week?

* SMO, work with Sosthène and meeting with Daniel and Loreleï to decide what's next

* Run the RR script on the cluster

* Read bibliography for the ICCAT paper

#### Where do you need help from Daniel or others?


#### Decisions made during meetings


#### Any other topics 



------------------------------------------------------------------- 
### Date: 13rd July 2020

#### Who did you help this week?

* Nobody

#### Who helped you this week?

* Loreleï for datarmor uses

#### What did you achieve?

* SMO meeting with Sosthène. 

* Computation of RR for old moratoriums (REC 11 and REC 98) BUT the results are not good because I forgot to filter FAD data in the rec 11 script.


#### What did you struggle with?

* Cluster, can't launch a job and my scripts..

#### What would you like to work on next week?


#### Where do you need help from Daniel or others?


#### Decisions made during meetings

See : [here](https://github.com/LGuery/teamwork_monitoring/blob/master/weekly_reports_and_meetings_repository/IlanPerez/meetings_report.md#date-22nd-july-2020)

#### Any other topics 



------------------------------------------------------------------- 
### Date: 3rd June 2020
 
## Grooooooos update parce que j'ai pas été un bon élève
 
#### Who did you help this week?

* WE ARE CONFINED :trollface:

#### Who helped you this week?

* WE ARE CONFINED :trollface:

#### What did you achieve?

##### Methods for CISEF

* First draft of Methods is written !

##### Filtering 

* Finally find that we will filter out tunas with 3 days at liberty or less. Wilcoxon tests tell that those tunas significantly traveled less than others (true for YFT and SKJ, not significant for  BET).

##### Matching
* Developed and fitted a GAM model with spline on length to have better Propensity scores than with the native glm in the matchit() function.

* I tried to estimate a good caliper for matching, but didn't find a way for the moment. Set it at 0.2 x SD.

* Decided to reverse control and treated groups. The treated group will be the tuna from outside the moratorium because there are less data in this group if we only keep January and February and we want to keep the maximum data available.

* Succed with PSM Nearest neighbour matching. All indices show that balance is improved with this method.

* Random matching seems to give quite different results depending the iteration. I ran the matching algorithm 1000 times. Number of matched individiuals can vary about 10. It has a huge impact on RR computation, because INSIDE RCF tunas vary from 0 to 7. This makes the RR sometimes infinte or very high (~ 177 !!).

##### Seamounts

* 3 meetings with Sosthène about seamount project.

* Achieve ECD data colection from Ob7 and treatment.

* We created a grid from cwp squares, and selected all squares with seamounts in them and at least 1 ECD data (2008-2019 temporal footprint).

* Creation of buffers with METRIC diameter, and union of "polyseamount" buffers.

#### What did you struggle with?

* With EVERYTHING. Details coming

#### What would you like to work on next week?

* PhD comitee presentation !

#### Where do you need help from Daniel or others?


#### Decisions made during meetings


#### Any other topics 



------------------------------------------------------------------- 
### Date: 27th April 2020

* LG: tes deux derniers WR sont beaucoup mieux que les autres! Bravo! Continue à les étoffer :)
 
#### Who did you help this week?

* WE ARE CONFINED :trollface:

#### Who helped you this week?

* WE ARE CONFINED :trollface:

#### What did you achieve?

* I searched information about matching, why ANF tunas are kept. Tried new methods, CEM and exact matching, and explored analysis of balance. In fact, first attempt of matching creates more imbalance in the sampling.

* Skype with Sosthène, organization about seamounts bibliographic research and analysis

* Slight advance in methods writing

#### What did you struggle with?

* I struggled with matching. Exact matching does filter more tunas than nearest neighbour method, but ANF tunas are almost alll kept. I don't understand why, I tried everything in the code to correct it, red through litterature about matching but didn't find any answer. I ask on stack overflow and I'm waiting for an answer.

#### What would you like to work on next week?

* Finish script duplication

* Continue Writing.

* Bibliographic research seamount

* FInd a solution for matching

#### Where do you need help from Daniel or others?


#### Decisions made during meetings


#### Any other topics 



------------------------------------------------------------------- 
### Date: 20th April 2020

 
#### Who did you help this week?

* WE ARE CONFINED :trollface:

#### Who helped you this week?

* WE ARE CONFINED :trollface:

#### What did you achieve?

* I sent the form for GDR Ecostat grant to Stephane on Wednesday.

* I verified why we keep all tunas tagged inside moratorium area, even though they are tagged near ANF and they have no homologs outside the area. That's because I use the method "Nearest neighbour", which will match tunas with the nearest propensity score. So tunas can have different levels of covariables, if they have close propsensity score, they will be matched.

* I explored seamonts tagging data and showed thath there is no correlation between peak depth and catch. But there are catch on seamount down to 400 m depth, so we can keep this as a limit.
There are 7 spots of seamounts tagging, that are often not coded as "SMO" when tuna are recaptured. We need to work with Sosthène to point out mistakes in the AOTTP database.

* Still exploring methods to filter out tunas in distance = f(time) graphe.

* Little advance in methods writing.

#### What did you struggle with?
#### What would you like to work on next week?

* Finish script duplication

* Launch final scripts for all species 

* Continue Writing.

#### Where do you need help from Daniel or others?


#### Decisions made during meetings


#### Any other topics 



------------------------------------------------------------------- 
### Date: 13th April 2020

 
#### Who did you help this week?

* WE ARE CONFINED :trollface:

#### Who helped you this week?

* WE ARE CONFINED :trollface:

#### What did you achieve?

* Meeting on Wednesday 8th April. see in the [meeting report](https://github.com/LGuery/teamwork_monitoring/blob/master/weekly_reports_and_meetings_repository/IlanPerez/meetings_report.md)

* Bibliographic review of some articles

* Finished GDR Ecostat form

* Began to adapt script to all size classes


#### What did you struggle with?
#### What would you like to work on next week?

* Finish script duplication

* Launch final scripts for YFT

* Begin Writing.

#### Where do you need help from Daniel or others?


#### Decisions made during meetings


#### Any other topics 



------------------------------------------------------------------- 
### Date: 6th April 2020

 
#### Who did you help this week?

* WE ARE CONFINED :trollface:

#### Who helped you this week?

* WE ARE CONFINED :trollface:

#### What did you achieve?

* Meeting on Wednesday 1st April. see in the [meeting report](https://github.com/LGuery/teamwork_monitoring/blob/master/weekly_reports_and_meetings_repository/IlanPerez/meetings_report.md)

* MatchIt of data

* Descriptive statistics

* Filtering of data: determined the threshold of one week and 50 km

* Exporation of potato shaped data of the distance = f(time) graph

* Began bibliographic review of ecological trap


#### What did you struggle with?

* Matching: two methods and I didn't find the best one
* Evolution of RR each year, by taking different pre-moratorium period for tagging

#### What would you like to work on next week?

* Finish with Matching
* Table of historical moratorium 
* Biblio for GDR Ecostat  + Ecological trap

#### Where do you need help from Daniel or others?


#### Decisions made during meetings


#### Any other topics 



-------------------------------------------------------------------  
### Date: 30th March 2020

    * # LG: Essaie de faire attention aux fautes de frappe? Que penses-tu aussi en cette période de confinement d'être un poil plus assidu pour les dates des weekly reports et les faire à date fixe?

#### Who did you help this week?

* WE ARE CONFINED :trollface:

#### Who helped you this week?

* WE ARE CONFINED :trollface:

#### What did you achieve?

* PhD meeting on Tuesday 24th, with Daniel, Loreleï and Matthieu. Same presentation than the previous week but corrected

* Added to the presentation some corrections, see in the [meeting report](https://github.com/LGuery/teamwork_monitoring/blob/master/weekly_reports_and_meetings_repository/IlanPerez/meetings_report.md#date-25th-march-2020)

* Read papers from Daniel, currently doing the bibliographic report

* "Matching" methodology, red some bibliography, tried it

* Explored "Spill probability" (idea from Daniel) : gives nothing

#### What did you struggle with?

* Matching: two methods and I didn't find the best one
* Evolution of RR each year, by taking different pre-moratorium period for tagging

#### What would you like to work on next week?

* Finish with Matching
* Table of historical moratorium 
* Biblio for GDR Ecostat  + Ecological trap

#### Where do you need help from Daniel or others?

* Maybe Matthieu for Matching

#### Decisions made during meetings

* Need to match samples to have comparable ones between inside and outside the moratorium

#### Any other topics 




-------------------------------------------------------------------  
-------------------------------------------------------------------  
### Date: 16th March 2020

#UPDATE FOR THE 3 LAST WEEKS

#### Who did you help this week?

* Nobody

#### Who helped you this week?

* Antoine gave me some graphs and data about YFT/BET size frequencies under FADS and in freeschool for my presentation

#### What did you achieve?

* Exploring differences between tunas associated with immobile structures and the other
* Presentation with xaringan package
* GDR ecostat grant form

#### What did you struggle with?


* Hard to do the presentation.
* find a good threshold for time t liberty for tunas

#### What would you like to work on next week?

* find a good threshold for time t liberty for tunas
#### Where do you need help from Daniel or others?


#### Decisions made during meetings


#### Any other topics 




-------------------------------------------------------------------  
### Date: 28th February 2020


#### Who did you help this week?

* Friday: Njararatiana and her student Auriane on day field experiments to test the efficiency of para-depredation devices

#### Who helped you this week?



#### What did you achieve?

* Seamounts mapping, buffering and data filtering
* Contacted Kim & Wessel for their paper
* Asked and get the PhD project call MARBEC grant


#### What did you struggle with?


* Database from Fonteneau doesn't match with his figures, sf package.


#### What would you like to work on next week?

* 
#### Where do you need help from Daniel or others?


#### Decisions made during meetings


#### Any other topics 




-------------------------------------------------------------------  
### Date: 21th February 2020


#### Who did you help this week?

* 

#### Who helped you this week?


#### What did you achieve?

* AOTTP DAKAR Abstract


#### What did you struggle with?


* Database for seamounts


#### What would you like to work on next week?

* 
#### Where do you need help from Daniel or others?


#### Decisions made during meetings


#### Any other topics 




-------------------------------------------------------------------  
### Date: 14th February 2020


#### Who did you help this week?

* Antoine and Yoluene for maping on R

#### Who helped you this week?


#### What did you achieve?

* Seamounts mapping, some bibliography


#### What did you struggle with?



#### What would you like to work on next week?

* Abstract for AOTTP meeting in Dakar, test metrics from McGarvey (2004)

#### Where do you need help from Daniel or others?


#### Decisions made during meetings


#### Any other topics 




-------------------------------------------------------------------  
### Date: 31th January 2020


#### Who did you help this week?

* NA

#### Who helped you this week?

* David Kaplan: Long Discussions about Relative Risk. Maybe should we look to RR with exclusion of tuna tagged and/or recaptured in east Atlantic. Look to RR by zone of tagging

#### What did you achieve?




#### What did you struggle with?



#### What would you like to work on next week?


#### Where do you need help from Daniel or others?



#### Where do you need help from Daniel or others?



#### Decisions made during meetings


#### Any other topics 




-------------------------------------------------------------------  
### Date: 24th January 2020


#### Who did you help this week?

* I helped Amael for tidyverse functions to enahnce his cript (gather/spread, pipes...)

#### Who helped you this week?

* NA  

#### What did you achieve?

* RR in function of time at lib over 60 days  => there's an inversion of RR after 60 days

* RR in function of distance traveled => strange pattern  

* Stat descriptive
    + barplot distance traveled by tunas
    + barplot of velocity
    + compute maximal traveled distance with the maximum speed found in litterature:


#### What did you struggle with?

* RAS Except script writing 

#### What would you like to work on next week?

* RR with other zones and periods
* Find another metric to assess the effectivness of moratorium (Ask David)
* Find buffer distance

#### Where do you need help from Daniel or others?

* NA

#### Where do you need help from Daniel or others?


* 

#### Decisions made during meetings

* 

#### Any other topics 

*  


-------------------------------------------------------------------  

### Date: 17th January 2020


#### Who did you help this week?

* Amael for ftp url fil downloading script

#### Who helped you this week?

* NA

#### What did you achieve?

* Restart meeting with Daniel and Lorelei  

* Knitt the .md doc of Gipsy's script annotation.

* Computing relative risk in function of time at lib

#### What did you struggle with?

* Find where come from the differene between what i get in the script nd what is presented in Gipsy's paper

#### What would you like to work on next week?

* Median distance in function of time at lib

#### Where do you need help from Daniel or others?

* NA

#### Any other topics

* TAM TAM and PhD students meetings took 2 days this week.


-------------------------------------------------------------------  
### Date: 10th January 2020


#### Who did you help this week?

* NA

#### Who helped you this week?

* NA

#### What did you achieve?

* Finished Gipsy's script annotation, releving errors 

#### What did you struggle with?

* With the script from Gipsy, long and not really well documented

#### What would you like to work on next week?

* Begin my own analyses on AOTTP data => Relative risk and time sensibility

#### Where do you need help from Daniel or others?

* NA

#### Any other topics

* 

-------------------------------------------------------------------  
### Date: 20th December 2019


#### Who did you help this week?

* Absolutely no one, Alex for linux maybe ?

#### Who helped you this week?

* Lorelei, Lisa Ailloud
  * LG: Peux-tu donner un peu plus de détails sur l'objet, le temps que cela a pu prendre, ou toutes autres infos que tu jugeras utiles?

#### What did you achieve?

* Kick off meeting report, finished administrative stuff

#### What did you struggle with?

* With the script from Gipsy, long and not really well documented

#### What would you like to work on next week?

* On the script again I had no time to finish it

#### Where do you need help from Daniel or others?

* Maybe on my questions on ICCAT, AOTTP data etc..

#### Any other topics

* 



-------------------------------------------------------------------
### Date: 12th December 2019


#### Who did you help this week?

* 

#### Who helped you this week?

* 

#### What did you achieve?

* 

#### What did you struggle with?

* 

#### What would you like to work on next week?

* 

#### Where do you need help from Olivier or others?

* 

#### Any other topics

* 



-------------------------------------------------------------------
