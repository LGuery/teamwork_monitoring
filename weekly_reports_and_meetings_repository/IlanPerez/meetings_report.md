# Meetings Reports

### Thèse IRD, rapports de nos réunions d'encadrement


* [28th July 2020](#data-28th-july-2020)réu SMO choix de la suite du projet
* [22nd July 2020](#data-22nd-july-2020)réu reprise et objectifs de l'été
* [13th May 2020](#data-13th-may-2020)Phd meeting with Matthieu => matching issues
* [4th May 2020](#data-4th-may-2020)Recoding SMO meeting with Sosthène
* [29th April 2020](#data-29th-april-2020)Matching test and filtering with box plot
* [22nd April 2020](#data-22nd-april-2020)CAH and distance for filtering
* [15th April 2020](#date-15th-april-2020)SMO + CAH
* [8th April 2020](#date-8th-april-2020)Decisions for the symposium
* [1st April 2020](#date-1st-april-2020)Filtering and matching the data 
* [24th March 2020](#date-24th-march-2020)PhD meeting  
* [18th March 2020](#date-18th-march-2020)Seamounts exploration   
* [20 January 2020](#date-20th-january-2020)Previous exploration    
* [13 January 2020](#date-13th-january-2020)Gipsy's script
* [12 December 2019](#date-12nd-december-2019) :airplane: :rocket: Kick-off! 
------------------------------------------------------------------
### Date: 28th July 2020

## Topics

* Présentation des résultats d'exploration des relations SMO/données ECD:

- Nous avons remarqué que le nombre de données par SMO était relativement faible autour des SMO, malgré les 11 ans de données FR et SP. Seulement 13 SMO présente plus de 100 données dans leur buffer de 50km de rayon. Parmis ces 13 SMO, aucun effet de la profondeur ne semble apparaître. Nous estimons que la profondeur n'est pas le critère prédominant dans l'aggrégation des thons. Les données environnementales **doivent** être prises en compte.



## What to do

* Laisser de côté le projet pour l'instant et se concentrer sur nos projets respectifs.
* Modifier l'apporche: 
- Initialement, nous faisions un buffer autour des SMO et nous avons séléctionné ceux avec au moins une donnée. Il a été proposé de définir la zone de pêche en recréant un polygone autour des cellules 1°x1° **NON-ISOLÉES**.
- Cette zone sera la zonne d'étude et tous les SMO présents dans cette zone et avec moins de 1000 m de profondeur seront sélectionnés.

3 hypothèses :
1) Si pas de captures autour de SMO dans Zone de pêche = pas attactif
2) SMO doit avoir un effet sur toute la période
3) Attraction = fonction profondeur + distance ?

### LG's comments

------------------------------------------------------------------
### Date: 22nd July 2020

## Topics

* Calcul du RR pour les anciens moratoires
* Test de randomisation pour sur données matchées 
* Cartographie de l'effort dans la zone sur carrés 1°x 1° et son évolution


## What to do

* Il faut retirer les captures sous DCP dans la zone des anciens moratoires pour être consistants avec le calcul de du RR du premier moratoire (pas de capture sous DCP dans la zone pendant les deux mois)

* Il faudrait faire un test de randomisation pour déterminer si les valeurs du RR sont dues aux hasard. 

* Commencer lepapier ICCAT sur le RR

* Lancer les scripts sur le cluster

### LG's comments

------------------------------------------------------------------
### Date: 13th May 2020

## Topics

* Presentation of advancement in the PhD, seamounts project with Sosthene, Methodes for the first paper.

* Organization of PhD comitee => changes needed

* Organization of stay in La Rochelle

* Discussions about matchong of data

* Abstract + Methods for CISEF

## What to do

* For matching: 
 - Try to fit a logit GAM, with spline on raw length values. 
 - Then verify goodness of fit => see Matthieu's papers
  - Then, extract the propensity scores from the fitted model and use them with `Matching`. Maybe try to complexify the model with year ? 
  
 * For filtering:
  - Filtering with boxplots was okay, we keep a 3 days limit. Try a one-way test for parametric significance test.
 

### LG's comments

------------------------------------------------------------------
### Date: 4th May 2020

## Topics

* Meeting with Sosthène about Seamounts recoding. We presented our bibliographic research. But after discussions, we decided to lead our own analysis, coupling seamounts data and ECD/AVDTH data. The aim will be to define height, depth and surface area where seamounts are actively attracting tunas.

## What to do

* Ask for data to Ob7

### LG's comments



-------------------------------------------------------------------
### Date: 29th April 2020

## Topics

* Good visualization with the boxplot graph time/distance. The FSC graph will be the reference because free tunas are the ones that have the "most natural behavior".

* Matching with nearest neighbour does not give good results. More imbalance is created with this method. Need to talk with Matthieu about these bad results. CEM methods seems to give better results.



## What to do

* Repport about matching for Matthieu
* Try more day at liberty bins for boxplot graph, 1 day, 2 days..up to 7 
* Look at matched pairs to understand matching process

### LG's comments



-------------------------------------------------------------------
### Date: 22nd April 2020

## Topics
* Meeting with Sosthène for seamounts recoding

* HAC didn't work well. Not the good filtering method
* Geometric distance was not the good method neither.

## What to do

* Try to do the same boxplot than David Kaplan et al. 2014.

### LG's comments



-------------------------------------------------------------------
### Date: 15th April 2020


## What to do

* Keep exploring to filter out points from fistance = f(time) graph. 
Some ideas: 
 - Look deeper in HAC: where are the points that are separated in the tree
 - Look at frequency by class of 10lm and 1 day 
 - Look at geometric distance from origni of each points & look at distibution
 
 * Explore why Matching keeps ANF tagged tunas :heavy_check_mark:
 
 * Send email to Hervé Demarcq, Francis Marsac & Alain Fontenau.
 
 * Do histogram of number of taggins on seamounts by peak height :heavy_check_mark:


### LG's comments



-------------------------------------------------------------------
### Date: 8th April 2020

## Decisions:

* Keep ideas about behavior  of tuna associated with SMO. 

* See distance = f(time) for all species and define the threshold => DONE

### What to do

* Ask to HErvé Demarcq + Francis + Alain for seamounts data (off Sierra Leone)

* Finish bibliographic report

* Prepare script for all length classes

* Begin to write MM + Results

### LG's comments

A faire:
1) Refaire la figure avec toutes les espèces puis une par espèce :heavy_check_mark:
2) CAH pour exclure :curly_loop:
3) Rédiger les méthodes du papier :curly_loop:
4) Réfléchir au moyen le plus optimal pour travailler de manière collaborative sur le papier (Github tous les jours puis un word par semaine en google doc?) :curly_loop:
5) Faire un excel partagé pour le planning 

**OBJECTIF fin Avril pour un draft de papier avec méthodes et résultats**
Garder en tête de demander à Lisa si soummission à Fisheries Research avant le symposium est possible

Garder sous le coude le sujet "comportement aggrégatif des thons):
* Comment définir le seuil SMO comme attractif -> histogramme des profondeur pour les SMO avec capture
* Patatoïde à étudier par bâteau. Explorer les groupes d'individus qui avaient été marqués ensemble puis recapturés ensemble -> comportement
* Faire le lien avec la thèse hotpot+SMO=ZFH?, utilisation de la présence/absence de SMO, distance et profondeur

-------------------------------------------------------------------
### Date: 1st April 2020

## Exploration of matching and filtering data discussions

I presented:

* Impossibility of computing annual RR because of the lack of data

* RR if we keep 2 to 8 weeks pre-moratorium period were tagging are kept for the analysis

* Matching on propensity score method and discussion about covariables to keep

### Decisions

* Use Release length, Release month and Release Structure as covariables for Matching and put together OIL and ANF codes

* Need to remove bias of recapture: filter data according to the extreme data on the bottom left of the  distance = f(time at liberty) graph for tunas relased under dFAD

* Explore what are the "PATATES" :potato: for seamounts data



### What to do

* 

### LG's comments

A faire:
1) Histogramme du nombre de poissons/catégorie de taille tous les 10cm :heavy_check_mark:
2) Figure Isolignes en gardant tous les individus - définition des seuils de temps de liberté/distance :heavy_check_mark:
3) Procédure de MatchIt :heavy_check_mark:
4) Explorer les patatoïdes :heavy_check_mark:

Décisions de tourner les analyses pour les 3 définitions de juvéniles - **A vérifier et ajouter les références correspondantes**:
- 56cm : Résolution ICCAT des individus de 3.2kg (**vérifier ces 56cm avec une relation taille/poids plus récente, si communication avec l'Ob7 à ce sujet, nous mettre en copie des mails**)
- 70cm : Double stanza
- 108cm : juveniles 50% repro

Garder en tête la pondération par la capture

-------------------------------------------------------------------
### Date: 24th March 2020

## PhD meeting. Postponed meeting with Matthieu. Put :sunny: during confinment

Same presentation than [18th March 2020](#date-18th-march-2020) but corrected and presented to Matthieu: show him the progression for the 1st objectif of the thesis.

### Remarks

* Discussions about new moratorium: since January 2020 (Rec[19-02]), FAD fishing forbidden over all the Altlantic Ocean, for 2 months in 2020 and 3 months in 2021  

* Be more precise on ecological trap definition !!! :shipit: See Daniel's ppt  

* No R output in the slides (Try `r kable ()` for tables )  

* Correct some mistakes : #6/27, #5/27  

* Don't forget to be precise on the filter applied for doing graphs

* KEEP Brazilian data that are now corrected

* Matthieu : Need to sub-sample the data to have two comparable samples

* Still need to find a threshold of time at liberty


### What to do

* 1: Test Matching (cf emails from Matthieu) to create 2 sub-samples that are comparable between inside and outside the moratorium. "COntrole" sample with tunas from outside the moratorium. Don't forget to use only variables that are known at the tagging time, to keep RC-1 and RCF tunas.

* 2: compute monthly RR from November 2016 to 2019

* 3: "Spill probability" (Daniel Idea): look at tunas that are Re In & Rc Out + Re OUt & Rc In 
:arrow_right: Look at the travel distance 

* 4: Verify if moratorium forbids anvhored FAD fishing (Ask Sosthène)

* 5: Bibliographic rewiew for Ecological Trap and Bycatch papers from Daniel

* 6: take a look to the schedule: where are we ?

### LG's comments
- *et al.* en italique - latin
- D5 : fautes tech**n**ology, sin**c**e
- D6 : nb de poissons? Pas en tonnage
- D7 : Attention explication du piège écologique pas encore matrisée -> **Faire une petite revue bibliographique sur le sujet** -> cf "What to do #5"
- Pas clair pourquoi tu te concentres sur les juvéniles
- Transition entre D7 et D8 à revoir
- D8 : Donner la définition d'un moratoire = interdiction de pêcher sous dFAD
- D11 : Inclure les données brésiliennes
- D13 Bravo, notation très claire
- D16 : Même table, attention à la forme
- **Traiter les données année par année?**
- **Indiquer à chaque analyse/graph les flitres opérés sur les données**
- D22 : Retirer "Homing"
- D23 : Titre erroné
- **Vérifier si pendant le moratoire on peut pêcher sous aFAD?** -> cf "What to do #4"
- **Faire la procédure de MatchIt avec le type de structure, la taille, le mois...** -> cf "What to do #1"
- **Faire un résumé/review des papiers envoyés par Daniel** -> cf "What to do #5"
- **Prendre du recul sur le planning de thèse et voir où on en est/réajustement des objectifs?/mide en place de deadlines?** -> cf "What to do #6"
- **Idée Daniel : Regarder le tps de liberté et distance des individus entrés et sortis du moratoire** -> cf "What to do #3"
- **OBJECTIF début de papier dans 2 semaines**

-------------------------------------------------------------------
### Date: 18th March 2020
## Presentation of exploration results and immobile structures effects

* I presented the "phd_meeting_13rdMarch.html" presentation available in my repository.

#### Questions/remarks

* Correct some mistakes in the presentation
* don't forget the references
* Find more recent data about FAD fisheries (slides 6-8)  

* Need to exclude tunas that are tagged and/or caught in January/February => no moratorium effect

* Try to do a 3D plot : time at lib, time and tagging location

#### What to to do next
* All explorations are good but we need to find a threshold for time at liberty to exclude tunas that are immediately recptured => in progress
-------------------------------------------------------------------
### Date: 20th January 2020
## First exploration of AOTTP data 


#### Results presented and issues/questions :question:  

* Presentation exploration about Relative Risk computation, in relation to time at liberty (period January-February) for juveniles YFT 
  + Can't explain the drop in RR between 0 and 10 daysj
  
  
* Distance = f(time at liberty)
  + No particular pattern  
  
  
#### What to explore next  
    
 * RR  
   + Extend the time at liberty after 60 days  
   + Find a way to check RR in relation to distance traveled 
   
 * Descriptive statistics:  
    + barplot distance traveled by tunas
    + barplot of velocity
    + compute maximal traveled distance with the maximum speed found in litterature:
    (Optimum = 25 km/h in Tuna: Physiology, Ecology and Evolution (2OO1),
    Max = 72 km/h in FAO from Magnuson (1978))  
    
   
  * Map6 :
    + What is this square at env. 9°N, -16°E ?  
    + Zoom on moratorium area to see what happens in Ivory cost
    + Count of CMR data



-------------------------------------------------------------------

### Date: 13th January 2020 

#Gipsy's script annotation discussion and first analysis planning 
#### Gipsy's script  

* Presentation of the content of the [.Rmd file](https://github.com/polarbear-tataki/tuna_dream_team/blob/master/obj_1_AOTTP_moratoria/GIPSY_TAGGING_AOTTP/tagging_data_explo_script_Ilan.md). Five parts in this script, everything is corrected. Some difference were found between Gipsy's paper and the results of the script. There are 4 more YFT individuals in the Table 3 generated by the script than the Table 3 in the paper.  
  
  
* Objectives for the following analysis:  
  + Compute Relative Risk in relation of time at liberty  
  + COmpute relative Risk in relation of distance traveled  
  + Comute RR for elder moratorium zone and period  
   
    
 * Afterwards  
   + Define a threshold distance/time traveled  
   + Use it to determine a consitent buffer



-------------------------------------------------------------------

### Date: 12nd December 2019

#Kick-off! :airplane: :rocket:  

#### Agenda  

* Presentation of the supervision team: Daniel, Lorelei and Matthieu  :busts_in_silhouette: : 


* Presenting the PhD project:
  + Objectives of the project:  
  
  :arrow_right: 3 big questions around the tropical tuna fisheries under FADs: :one: effects of FADs on high seas populations, communities & ecosystems, :two: efficiency of moratorias in Atlantic ocean and :three: we don't know what Fisheries Functionnal Zones (FFZ or ZFH) are for yellowfin (YFT), skipjack (SKPJ) and Big Eye (BET) tunas.  
  
  :arrow_right: This project aims to answer these questions in 4 steps:  
  
  :one:Use AOTTP (mark-recapture program in AO) data to evaluate the efficiency of current and past moratorias (2 periods x 2 zones)  
  
  :two:Defining ZFH for BET, YFT + SKJ in AO and IO using size and species structured, spatialized and time referenced (aggrgated 1°/month) landings data  :fish:  and define. A second part of this objective will be to link these data with environmental data (chl a, Temp, currents, sea height anomaly...)  
  
  :three:Assess the temporal and spatial evolution of ZFH, the connectivity between them and find if these zones are relevant for bycatch species as sharks  :shark:  
  
  :four: Use the knowledge acquired on ZFH to evalutate the moratorias and propose new type of moratorium based on adapted spatio-temporal strata  
  ry for 
  + Partipation to ICCAT  :earth_africa: & IOTC  :earth_asia: :  
  
 :arrow_right:16-23 July 2020: Dakar Symposium of AOTTP + Data preparatory  
 
 :arrow_right: ~October 2020: Maldivies IOTC  
 
 :arrow_right: 2021: Working group "Ecosystems" ICCAT + Sharks  
 
 
 * Implications of each supervisor :eyes: :  
 
 Everybody in copy of all emails, we'll see after  
 
 * Organization of meetings/reports :calendar: :
 
 :arrow_right: Weekly report each week on the [github](https://github.com/LGuery/teamwork_monitoring/tree/master/weekly_reports_and_meetings_repository/IlanPerez)  
 
 :arrow_right: 1 skype/month with Matthieu for briefing/avancement....  
 
 
  :arrow_right: Mini-commity each :three: months with a presentation of preliminary results :chart_with_upwards_trend:  
  
  :arrow_right: GDR Ecostat Grants to move to La Rochelle  
   
   
   * Communication & collaboration platforms :left_right_arrow: :  
   
   :arrow_right: GitHub will be used to monitor: :one: weekly the issues and solutions (see above), :two: the current work/scripts etc under .rmd format in the repository [tuna_dream_team](https://github.com/polarbear-tataki/tuna_dream_team) .  
   
   :arrow_right: [Slack](https://app.slack.com/client/TRQNP7NNQ/CRQNP8HC4) will be used to interact on diffrent subjects, in a clearer way than long strings of emails. We can follow what happens on the GitHub repository directly in the chanel discussion.  
   
   
   # LET'S GOOOOOOOOOOOOO!
   
