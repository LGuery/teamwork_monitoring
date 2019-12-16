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
