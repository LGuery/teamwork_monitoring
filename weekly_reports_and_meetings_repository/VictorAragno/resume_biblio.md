---
title: "Biblio"
author: "Victor Aragno"
date: "13 decembre 2019"
output: pdf_document
---

# Resume bibliographique

## Contexte

### Le commencement. Fontenau 1999

Plusieurs problemes dans la relation CPUE-Abondance.
Une forte CPUE n'implique pas une forte abondance. Nous pouvons par exemple calculer de forte CPUE dans de grandes zones ou les navires ont passe peu de temps a pecher. A faire dans CPUE: Prendre en compte la prise totale par zone et espace de temps.

L'etude temporelle de la CPUE est biaisee:

- Evolution technologique des navires -> diminution de la CPUE

- Changement de methode et de peche avec passage progressif de peche sous banc libre a peche sous banc objets -> diminution de la CPUE

- Evolution du prix des espaces -> variation intra et extra annuelle

Choix ideologiques et pratiques sur la conception:

- Choix des variables explicatives 

- Choix de la stratification spatiale: quadrillage de carre de 1d, 5d. 
Laurec (1977) la relation entre CPUE et abondance peut etre altere par une repartition non aleatoire des thons dans la surface marine.

- Choix de la stratification spatio-temporelle

Un choix arbitraire retenu neanmoins comme acceptable est une duree de 3j pour un carre de 1d (Fonteneau, 1986, 1991, Foucher, 1994, Ravier et al., 2000)

### Annee 2005 et forte concentration. Fonteneau (2008)

Une forte concentration de thons a ete repertorie en 2005 dans l'ocean atlantique. Cette concentration se situe dans une zone d'environ 3500miles carre soit un carre de 6d (45;50)d E, (3;8)d S. Nous avons capture dans cette zone 22 000tones de YFT en 12 jours (donnees francaise et espagnoles tout type de banc). Soit 6.5% de la mortalite totale par peche pour l'annee. 
CPUE cette annee: 65t/j
prise moyenne par calee positive: 85t

Cet evenement survient 18 jours apres de tres fortes concentration de chlorophylle.

Resume suppose : forte concentration phytoplancton -> forte biomasse de proie -> forte concentration de thons (en periode de reproduction)

### Etude des concentrations Mohamed Toihir (2009)

Augmentation du nombre de "concentration" (capture > 500t pour une trihade 3j-1d) autour de 2004 
La zone de forte peche de 2005 est une zone ou generalement sont observes de fortes concentrations de YFT. 
Disparite saisonniere: sur 126 concentrations bancs libres, 54 ont eu lieu pendant le 1er trimestre (periode de reproduction des YFT), 29 pendant le 2eme trimestre, 17 pour le 3eme trimestre et 26 au cours du 4eme trimestre.
"Pour la concentration num 103 d'albacore (Figure 16a) les prises et l'effort evoluent de facon croissante au cours de l'exploitation jusqu'a epuisement de la ressource" La concentration num 103 fait reference a celle evoque par fonteneau mais sur une zone plus large.

#### Temperature de surface

(Marche pour le southern bluefin tuna) la capturabilite de cette espece augmente avec l'arrivee d'eau froide provenant du sud de l'ocean indien. Hsueh Jung LU (2008)

Variation des temperatures de surface pour les annees 1993-2004 a la Reunion: correlation negative entre CPUE et la temperature de surface (SST) Francois Conand (2007)

### Reduction de la biomasse apres grosses captures

Baisse fortement significative de la CPUE et des prises en 2006-07 dans l'ouest de l'ocean indien. Marsac, IOTC (2008)

## Modeles

### Actuel. Guery (NA)

modele d'estimation a trois composantes

### VAST vecteur auto-regressif spatio temporelle - delta GLMM. vignette VAST

Vast est un package servant entre autre a calculer des indices d'abondance. Il utilise pour se faire un modele a deux composantes. Une composance modelisant la probabilite de rencontre l'autre le taux de capture. Les modeles utilises sont de type GLM avec selection de modele basic type AIC ou crossvalidation. Ces modeles peuvent inclure des variation spatio et/ou-spatio temporelle. [James T.Thorson 2019](https://reader.elsevier.com/reader/sd/pii/S0165783618302820?token=76FFF5B826DDE56886047417091B0B2EF75184B35D3169E863CA15DB9CF018F70338FCDB6BCD7918128D0F6A8979B7BC)

A detailler.

Pour des raisons de calculabilite, ils utilisent prealablement une clusterisation des aires geographiques par k-means. Assumant l'hypothese que chaque aire suit la meme loi que le "centre" le plus proche. 
