---
title: "Bibliographie"
author: "Gwenaelle"
date: "2 decembre 2019"
output:
  word_document: default
  pdf_document: default
  html_document: default
bibliography: Bibliographie_Gwenaelle.bib
---

# Methodologie  
Developper un indice CPUE standardise [@Guery2019]     
Differents facteurs influencent les CPUE. [@Guery2019]    
GLMM : Poisson + Binomial + log normal  [@Guery2019]   
CPUE sur serie de temps  [@Guery2019]   
Nouvelle approche  [@Guery2019]   
Necessaire d'inclure les variables environnementales  [@Guery2019]   

Donnees sur 42 ans.  [@Xu2019]    
Resolution de 1° * 1° et 1 journee  [@Xu2019]    
Modele divise en quart d'annee  [@Xu2019]    
Distribution spatiale varie d'annee en annee  [@Xu2019]     
L'indice d'abondance standardise varie au fil des annees  [@Xu2019]    
Modele lineaire mixte delta generalised  [@Xu2019]    
Inclure des variables environnementales  [@Xu2019]    

# CPUE

La relation entre CPUE et abondance est complexe  [@Fonteneau1999]  
Les comparaisons sont faites selon des strates spatio-temporelles  [@Fonteneau1999]  
L'augmentation de la qualite de peche pause probleme dans le calcul car on ne peux pas prendre en compte les ameliorations pour tous les bateaux  [@Fonteneau1999]  
Utilisation de l'AIC  [@Fonteneau1999]  

Prendre en compte les variations environnementales mais aussi chez les especes  [@Goodyear2003]  

Methode la plus commune pour standardiser les CPUE est la GLM  [@Hinton2003]  
Objectif de l'analyse est de determiner un effet annuel [@Hinton2003]   
Variation annuelle = representation biaisee de l'abondance  [@Hinton2003]  
qu'importe la methode statistique utilisee, il faut que les variables explicatives prises en compte soient les bonnes  [@Hinton2003]    

Les CPUE ne se referent pas a toute la population. Uniquement la population susceptible d'etre pechee (depend de la selectivite des engins)  [@Maunder2006]  
Les approches monospecifiques sont inutiles. Il faut des approches plurispecifiques qui prennent egalement en compte les ecosystemes  [@Maunder2006]  
Impossible de donner des predections uniquement en se basant sur les CPUE  [@Maunder2006]  

Mouvement migratoire qui rend plusieurs classes d'age vulnerable a la surexploitation  [@RodriguezMarin2003]  

CPUE = C/E = qN  [@Zhou2019]  
C = prise E = effort de peche q= constante N = abondance  [@Zhou2019]  
Pour standardiser les CPUE utilisation de GLM ou GAM  [@Zhou2019]  
Etudie l'avantage des geostatistiques (INLA) pour la standardisation des CPUE  [@Zhou2019]  
Le modele prenant en compte les interactions spatiales et temporelles est le meilleur  [@Zhou2019]  

Ajout d'une constante a toutes les donnees de prises pour eviter l'inclusion des 0  [@Langley2004]  
Prend en compte les phases lunaires dans les CPUE  [@Langley2004]  
4 manieres differentes de calculer les CPUE  [@Langley2004]  
Predictions en fonction des differents parametres pris en compte  [@Langley2004]  

Nombre de peche par jour (CPUE1) estimations du nombre de banc de thons et la capicite a les trouver  [@Chassot2012]  
La proportion de prise positive (CPUE2) --> capacite du bateau a pecher  [@Chassot2012]  
Le poids de poissons par remontee positive (CPUE3)  [@Chassot2012]  

CPUE = (YFT1 + BET1 + SKP)/ fh  [@Soto2008]  
avec YFT1 = prise de juvenile de yellowfin, BET1 = prise de juvenile de Bigeye, SKP = prise de skypjack et fh = heure de peche par jour  [@Soto2008]  
Skipjack diminue plus clairement que les deux autres  [@Soto2008]  

# Effort de peche
 
GLM methode la plus utilisee  [@Maunder2004]  
GAM, GLMM  [@Maunder2004]  
Trois methodes pour faire face aux 0  [@Maunder2004]  
  
CPUE : nombre de filets par jour, nombre de fois ou c'est positif et la prise  [@Gaertner2015]  
Ajouter une correlation spatiale dans la standardisation des CPUE  [@Gaertner2015]  
Prendre en compte le temps reste au niveau du DCP  [@Gaertner2015]  

Controle des FAD : fermeture saisonniere et limitation du nombre  [@Tolentino-Zondervan2018]  
La peche sur les FAd est la plus utilisee  [@Tolentino-Zondervan2018]  
Pendant la fermeture des FAd peche sur les freeshool  [@Tolentino-Zondervan2018]  
Le choix entre les deux se fait en prenant en compte les marges realisables  [@Tolentino-Zondervan2018]  

Analyse geospatiale avec postGre SQL [@Snouck2017]  
Pour les bouees : donnees "en eau" ou "a bord" [@Snouck2017]   
Effort de peche ne change pas car les francais peche essentiellement sur des FOB qui n'ont pas de GPS  [@Snouck2017]  

VMSTOols et VMSBase sur R pour analyser les donnees VMS et les logbooks  [@Natale2015]  
Permet en autre de faire un merge entre les VMS et les logbook  [@Natale2015]  
Permet de faire la discrimination entre peche et non peche et de faire des carte d'effort de peche  [@Natale2015]  
Utilisation de l'AIS  [@Natale2015]  
Repartition bimodale de la vitesse avec vitesse haute = periode de rechercher et vitesse basse = peche  [@Natale2015]  
Comparaison entre les points de peche issus des logbook et les trajets des bateaux en fonction de la vitesse  [@Natale2015]  
Pour les logbook : l'effort est calcule dans chaque rectangle ICES comme le nombre de jour en mer. Si un bateau passe sur pluisieurs rectangle on repartit le nombre de jours en mer entre les rectangles. [@Natale2015]    
Les deux approchs donnent un distribution spatiale de l'effort similaire [@Natale2015]    

Utilisation des logbooks pour recenser les activit�s de p�che [@Torres-Irineo2014]  
Comparaison entre p�che sur banc libre et p�che sur FAD [@Torres-Irineo2014]  
Essaye de comprendre comment les am�liorations sur les bateaux influencent les prises [@Torres-Irineo2014]  
L'effort de p�che est le nombre de jours o� p�che sur FAD / nombre de jours en mer [@Torres-Irineo2014]  
Les donn�es n�cessaires pour une bonne estimation des prises sur FAD [@Torres-Irineo2014] : 

* le nombre de FAD d�ploy�es par bateau  
* le temps de d�ploiement par FAD
* la distance entre les FAD
* la m�thode de d�tection des FAD  


<span style="color:#fb4141">L'effort de peche peut se calculer via le temps de recherche.  
Mais pour les DCP, le choix des zones n'est pas lie au hasard.  
Necessaire de trouver un nouveau moyen de calculer.  
Possible de calculer en fonction du temps passe a la bouee via   
les on /off effort ?  
les traces GPS des bateaux (diminution de vitesse, reste au meme endroit ) ?
Bouees "en eau" ou "a bord" ?
Nombre de jour de peche sur nombre de jour en mer ?</span>  


# Espece et prises accessoires  

350000 tonnes de prises accessoires de thons tropicaux [@Amande2010]  
Egalement prise accessoires d'autres especes : tortues, requins, mammiferes [@Amande2010]  
Prise accessoire plus importantes avec les DCP [@Amande2010]

Modele de croissance composite  [@Bard1991]  
35 a 65 cm : modele de croissance lente, lineaire  [@Bard1991]  
65 a 110 cm : croissance rapide, courbe  [@Bard1991]  
Biais : vulnerabilite aux engins de peche en fonction de la taille  [@Bard1991]  


# DCP

Les thons se regroupent autour des objets flottants [@Escalle2017]   
Augmentation de cette methode depuis les annees 90  [@Escalle2017]   
Utilisation des DCP augmente les prises accessoires  [@Escalle2017]   
Plusieurs mesures : moratoire sur les DCP ou zone de non peche  [@Escalle2017]   
Simulation d'un moratoire de 6 mois sur les DCP donne des resultats differents dans les deux regions [@Escalle2017]    

Description des especes et tailles pechees avec les DCP  [@Fonteneau2013]  
DFAD = tous types d'objets flottants equipes d'un satelitte  [@Fonteneau2013]  
Pose probleme pour standardiser les CPUE  [@Fonteneau2013]  
La moyenne des prises par peche est une meilleure estimation  [@Fonteneau2013]  
DFAD = trappe ecologique  [@Fonteneau2013]  

Les thons sont attires par les objets flottants  [@Hallier2008]  
Les thons se nourrissent moins au niveau des FAD  [@Hallier2008]  
Leur sante est moins bonne compare au "freeschool"  [@Hallier2008]  
Trappe ecologiques ; les DCP attirent les thons dans dez zones plus risquees  [@Hallier2008]  
 
50% des thons en vente proviennent des FAD [@Lopez2014]  
95% des pecheurs utilisent les sondeurs pour savoir quels FAD prospecter [@Lopez2014]  
Ces engins permettent d'augmenter les peche et donc les marges [@Lopez2014]  

Modification des mouvements naturels  [@Marsac2000]  
Augmente la competition pour la nourriture  [@Marsac2000]  
Augmente la predation  [@Marsac2000]  

Impossible de dire pourquoi un DCP plus efficace qu'un autre  [@Itano2005]  
Necessaire de mettre en place des donnees communes lors des peches  [@Itano2005]  

Augmentation de la production  [@Sharp2011]  
Moins d'import et plus d'export  [@Sharp2011]  
Diminue les temps de recherche  [@Sharp2011]  

## References  
Amandè, Monin Justin, Javier Ariz, Emmanuel Chassot, Alicia Delgado De Molina, Daniel Gaertner, Hilario Murua, Renaud Pianet, Jon Ruiz, and Pierre Chavance. 2010. “Bycatch of the European purse seine tuna fishery in the Atlantic Ocean for the 2003-2007 period.” Aquatic Living Resources 23 (4): 353–62. doi:10.1051/alr/2011003.

Bard, François Xavier, Claire Chabanet, and Nathalie Caouder. 1991. “Croissance du thon albacore (Thunnus Albacares) en océan Atlantique estimée par marquages.” papers3://publication/uuid/50CB3523-DACC-48DC-91FE-B04F0F193C11.

Chassot, Emmanuel, L. Dubroca, A. Delgado de Molina, C. Assan, M. Soto, Laurent Floch, and Alain Fonteneau. 2012. “Decomposing purse seine CPUEs to estimate an abundance index for yellowfin free-swimming schools in the Indian Ocean during 1981-2011,” 25 p. multigr. http://www.documentation.ird.fr/hor/fdi:010057904.

Escalle, Lauriane, Daniel Gaertner, Pierre Chavance, Alicia Delgado De Molina, Javier Ariz, and Bastien Mrigot. 2017. “Forecasted consequences of simulated FAD moratoria in the Atlantic and Indian Oceans on catches and bycatches.” ICES Journal of Marine Science 74 (3): 780–92. doi:10.1093/icesjms/fsw187.

Fonteneau, A, D Gaertner, and V Nordström. 1999. “An overview of problems in the CPUE-abundance relationship for the tropical purse seine fisheries” 49 (3): 9–39.

Fonteneau, Alain, Emmanuel Chassot, and Nathalie Bodin. 2013. “Global spatio-temporal patterns in tropical tuna purse seine fisheries on drifting fish aggregating devices (DFADs): Taking a historical perspective to inform current challenges.” Aquatic Living Resources 26 (1): 37–48. doi:10.1051/alr/2013046.

Gaertner, D, J Ariz, N Bez, S Clermidy, G Moreno, H Murua, and M Soto. 2015. “Catch, Effort, and Ecosystem impacts of FAD-fishing (CECOFAD).” Col. Vol. Sci. Pap. ICCAT 71 (1).

Goodyear, C Phillip, David Die, David W Kerstetter, Donald B Olson, and Eric Prince. 2003. “Habitat Standardization of Cpue Indices : Research Needs.” Iccat 55 (2): 613–23.

Guéry, Loreleï, David M. Kaplan, Camille Deslias, Francis Marsac, Francisco Abascal, Pedro Pascual, and Gaert. 2019. “Accounting for Fishing Days Without Set , Fishing Concentration and Piracy in the Cpue Standardisation of Yellowfin Tuna in Free Schools for the Eu Purse Seine Fleet Operating in Th ... Accounting for Fishing Days Without Set , Fishing Concentration and P,” no. October.

Hallier, Jean Pierre, and Daniel Gaertner. 2008. “Drifting fish aggregation devices could act as an ecological trap for tropical tuna species.” Marine Ecology Progress Series 353: 255–64. doi:10.3354/meps07180.

Hinton, Michael G, and Mark N. Maunder. 2003. “Methods for standardizing CPUE and how to select among them,” no. July.

Itano, David G. 2005. “An examination of vessel , gear and operational details useful for fishery-specific effort standardization , including FAD-related gear and fishing strategies,” 1–9.

Langley, Adam. 2004. “SA – 5 A standardised analysis of skipjack tuna CPUE from the WCPO drifting FAD fishery within skipjack assessment area 6 ( MFCL 6 ).” 6 (July).

Lopez, Jon, Gala Moreno, Igor Sancristobal, and Jefferson Murua. 2014. “Evolution and current state of the technology of echo-sounder buoys used by Spanish tropical tuna purse seiners in the Atlantic, Indian and Pacific Oceans.” Fisheries Research 155. Elsevier B.V.: 127–37. doi:10.1016/j.fishres.2014.02.033.

Marsac, F., A. Fonteneau, and F. Ménard. 2000. “Drifting FADs used in tuna fisheries: an ecological trap?” Proceedings of the 1st Symposium on Tuna Fisheries and FADs, Martinique, October 1999, no. JANUARY: 537–52.

Maunder, Mark N., and André E. Punt. 2004. “Standardizing catch and effort data: A review of recent approaches.” Fisheries Research 70 (2-3 SPEC. ISS.): 141–59. doi:10.1016/j.fishres.2004.08.002.

Maunder, Mark N., John R. Sibert, Alain Fonteneau, John Hampton, Pierre Kleiber, and Shelton J. Harley. 2006. “Interpreting catch per unit effort data to assess the status of individual stocks and communities.” ICES Journal of Marine Science 63 (8): 1373–85. doi:10.1016/j.icesjms.2006.05.008.

Natale, Fabrizio, Maurizio Gibin, Alfredo Alessandini, Michele Vespe, and Anton Paulrud. 2015. “Mapping fishing effort through AIS data.”

Rodriguez-Marin, E, H Arrizabalaga, M Ortiz, C Rodriguez-Cabello, G Moreno, and L.T Kell. 2003. “Standardization of bluefin tuna, Thunnus Thynnus, catch per unit effort in the baitboat fishery of the Bay of Biscay (Eastern Atlantic).” ICES Journal of Marine Science. doi:10.1016/S1054.

Sharp, Michael. 2011. “The Benefits of Fish Aggregating Devices in the Pacific.” SPC Fisheries Newsletter 135 (August): 28–36.

Snouck-Hurgronje, Julia E., David M. Kaplan, Emmanuel Chassot, Alexandra Maufroy, and Daniel Gaertner. 2017. “Fishing on floating objects (FOBs): How French tropical tuna purse seiners split fishing effort between GPS-monitored and unmonitored FOBs.”

Soto, M, P Pallarés, A Delgado De Molina, and D Gaertner. 2008. “Standardized Cpue for Juvenile Yellowfin, Skipjack and Bigeye Tuna From the European Purse Seine Fleet in the Atlantic Ocean From 1991 To 2006.” SCRS Sci. Pap. ICCAT 116 (644): 1044–53.

Tolentino-Zondervan, Frazen, Paul Berentsen, Simon R. Bush, and Alfons Oude Lansink. 2018. “FAD vs. free school: Effort allocation by Marine Stewardship Council compliant Filipino tuna purse seiners in the PNA.” Marine Policy 90 (December 2017). Elsevier Ltd: 137–45. doi:10.1016/j.marpol.2017.12.025.

Torres-Irineo, Edgar, Daniel Gaertner, Emmanuel Chassot, and Michel Dreyfus-Le�n. 2014. "Changes in fishing power and fishing strategies driven by new technologies: The case of tropical tuna purse seiners in the eastern Atlantic Ocean." Fisheries Research 155. Elsevier B.V.: 10-19. doi:10.1016/j.fishres.2014.02.017.  

Xu, Haikun, Cleridy E. Lennert-Cody, Mark N. Maunder, and Carolina V. Minte-Vera. 2019. “Spatiotemporal dynamics of the dolphin-associated purse-seine fishery for yellowfin tuna (Thunnus albacares) in the eastern Pacific Ocean.” Fisheries Research 213 (January): 121–31. doi:10.1016/j.fishres.2019.01.013.

Zhou, Shijie, Robert A Campbell, and Simon D Hoyle. 2019. “Catch per unit effort standardization using spatio-temporal models for Australia’s Eastern Tuna and Billfish Fishery.” ICES Journal of Marine Science 76: 1489–1504. doi:10.1093/icesjms/fsz034.
