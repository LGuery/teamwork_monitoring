# Weekly Reports

### Thèse IRD 

* [27 July 2020](#date-27-july-2020)

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
### Date: 13rd July 2020

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
