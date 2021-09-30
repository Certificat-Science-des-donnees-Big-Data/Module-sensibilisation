# Module-sensibilisation
Retrouvez ici les contenus à étudier en autonomie du module *sensibilisation*.
_____
## Planning de travail

- 9 septembre 2021 : réunion de rentrée
- Du 13 au 29 septembre 2021 : faire les paragraphes 1, 2 et 3.
- Séance en présentiel le 30 septembre 2021 après-midi.
- Du 1 octobre au 24 octobre 2021 : faire les paragraphes 4, 5 et 6.
- Séances et TP les lundi 25 (toute la journée), mardi 26 octobre et mercredi 27 octobre 2021 (9h-14h).
______

Les ressources pédagogiques offrent plusieurs niveaux de lecture ou d'utilisation afin d'être au mieux adaptées à un public hétérogène. Plus précisément il faut voir ce certificat comme une introduction à la *Science des Données* qui propose des pistes et références pour des approfondissements ultérieurs.

1. Le premier niveau est constitué des documents de cours de base (format `.pdf`) ci-dessous présentant les 
*grands principes* des méthodes ainsi que de nombreux exemples d'utilisation. Ils suffisent à une compréhension générale.
2. Ces documents pointent (liens hypertextes) vers des ressources de *deuxième niveau* ou d'approfondissement car intégrant les formulatons mathématiques des méthodes et algorithmes. Ces ressources sont celles du site collaboratif [`wikistat`](http://wikistat.fr/).
3. Le troisième niveau, appliqué, est composé des tutoriels (calepins ou jupyter notebooks) explicitant le traitement élémentaire de données "jouet", les exemples illustrant les documents de cours et d'autres exemples sur des données réelles. Ils servent de base de travail durant les phases de présentiel. 
4. Un quatrième niveau est à rechercher avec d'autres exemples d'utilisation disponibles dans les dépôts: [`github-wikistat`](https://github.com/wikistat/).

## Environnement logiciel
*Deux solutions sont possibles*

1. Utilisation élémentaire avec *Google Colab*
2. Utilisation experte des *notebooks* d'un dépôt *Github* après installation de R et Python, puis chargement ou clônage du dépôt.

**Attention** l'utilisation de *Google Colab* nécessite une connexion internet correcte contrairement à une exécution en locale une fois le dépôt *Github* chargé ou clôné. De plus les fichiers de données sont nécessairement chargés sur internet  pour chaque tutoriel.

### 1 Solution élémentaire avec *Google Colab*
- Une seule fois: 
    - Installer puis exécuter le navigateur *Chrome*
    - Ajouter à *Chrome* l'extension *"open notebook in google colab"*
- Pour chaque tutoriel
   - Lancer *Chrome*
   - Se connecter avec son compte *Gmail*
   - Ouvrir l'URL de [Google Colab](https://colab.research.google.com/notebooks/welcome.ipynb)
   - Ouvrir dans *Chrome* le tutoriel ou *notebook* du dépôt à exécuter à partir de son URL
   - Cliquer sur l’icône d*"open notebook in google colab"*
   - Suivre le tutoriel en exécutant chaque cellule

### 2 Solution experte avec installations des logiciels

Pour les parties 1. Introduction à R, 2. Eléments d'analyse statistique de données et 3. Modélisation statistique, il faut installer le logiciel R. Il s'installe à partir du lien [R-project](https://www.r-project.org/) en choisissant la version qui correspond au système d’exploitation de la machine de l’utilisateur (Windows, ios, Linux). L’interface conseillée pour l’utilisation de R s’appelle [RStudio Desktop](http://www.rstudio.com/products/rstudio/download) en choisissant la version *Open Source License*.

Pour les parties suivantes, l'installation de Python 3 est requise pour la bonne exécution des tutoriels. Le plus simple est de l'installer à partir de la distribution [Anaconda](https://www.anaconda.com/download/). R nécessite également l'installation du noyau [IRkernel](https://irkernel.github.io/installation/).

Pour **exécuter les tutoriels**, il *suffit* de cloner ce dépôt, si vous avez un compte (gratuit) et les compétences nécessaires *GitHub*, ou encore, plus simplement, de [télécharger l'archive](https://github.com/Certificat-sciences-des-donnees-bigdata/Module-sensibilisation/archive/master.zip) puis de la dézipper. Lancer enfin *jupyter notebook* dans une fenêtre de commande. Le navigateur par défaut ouvre une fenêtre. Dans cette fenêtre, se déplacer dans le bon répertoire chargé ou clôné, puis ouvrir les différents calepins (fichiers d'extension.ipynb). L'exécution de chaque cellule d'un calepin est obtenue en cliquant sur le bouton `run`.

L'installation de certains paquets requis pour exécuter les codes peut causer des problèmes dans Windows, il est donc fortement recommandé de créer une partition Linux ou une machine virtuelle, ou autrement d'utiliser [Colab](https://colab.research.google.com)... si ça coince trop...


Les sections 1, 2 et 3 du module de sensibilisation portent sur des connaissances de base en analyse statistique de données, que d’aucuns auront sans doute abordées durant leurs études. Elles se clôtureront par une séance d’une demi-journée en présentiel, durant laquelle les notions acquises seront revisitées sur la base d’un jeu de questions-réponses entre les élèves de la classe et les enseignants, en s’appuyant sur les travaux personnels proposés dans ces sections.

## 1 Introduction à R pour le calcul statistique
*A faire sur la période du 10/09 au 29/09*

Le langage de programmation R est un langage reconnu pour l’analyse statistique de données, massives ou non.  L’acquisition de compétences dans l’utilisation de R est aujourd’hui un atout professionnel pour ceux qui le maîtrisent.

### 1.1 Documents de base à consulter en autonomie
- Cours introductif intitulé Logiciel R de [`wikistat.fr`](http://wikistat.fr/).
- [*Shortcut reference card*](https://cran.r-project.org/doc/contrib/Short-refcard.pdf) de Tom Short.
- [R pour les débutants](https://cran.r-project.org/doc/contrib/Paradis-rdebuts_fr.pdf) d’Emmanuel Paradis.
- De nombreux sites internet sont dédiés aux utilisateurs de R, parmi lesquels : www.r-bloggers.com (the «  R blogosphere »), https://datascienceplus.com/ (online learning resource), https://www.datacamp.com/ (online learning resource).

### 1.2 Travail personnel demandé 
L’exercice que vous soumettrez au terme de ce module, par binôme, vous permettra d’acquérir des compétences en langage R. Vous êtes invité à contacter vos enseignants (florent.bourgeois@ensiacet.fr et rachid.ouaret@ensiacet.fr ou via Slack) pour vous aider dans la réalisation de ce travail. L’exercice porte sur la manipulation de variables aléatoires et leurs distributions statistiques, un des socles de l’analyse statistique de données.

Soit X1 et X2 deux variables aléatoires indépendantes qui suivent une loi normale ou bien une loi uniforme, au choix. Écrivez en langage *R* les 6 fonctions (p, d, q, r, e et v)CertificatBigData, dans un même script R, qui permettent de calculer la fonction de répartition CDF (pour *Cumulative Distribution Function*), la fonction densité de probabilité PDF (pour *Probability Density Function*), les quartiles, la génération de nombres aléatoires, la moyenne et la variance des variables Y = X1+X2, Z = X1×X2 et Z = X1÷X2. Les dites fonctions produiront, selon le choix de l’utilisateur, les graphes pertinents qui permettent de visualiser les résultats attendus de ces 6 fonctions.

**Au terme de cet exercice, vous répondrez grâce à votre code de calcul à la question suivante : quelle est la distribution statistique de la somme de 2 variables aléatoires uniformes ?** La réponse à cette question sera discutée durant la séance en présentiel associée à ce module du certificat.

Le rendu de ce module est donc un code intitulé NOM1_NOM2_NOM3.R, du nom des membres du trinôme, avec les 6 fonctions suivantes :
- pCertificatBigData()
- dCertificatBigData()
- qCertificatBigData()
- rCertificatBigData()
- eCertificatBigData()
- vCertificatBigData()

Chaque fonction sera richement commentée. En particulier, la signature de chaque fonction devra indiquer :

- Les noms des auteurs
- La date
- La liste des arguments d’entrée et de sortie des fonctions, avec des valeurs par défaut des arguments d’entrée si elles se justifient.
- Un ou plusieurs exemples d’appel
- Le lien, optionnel, vers l’application Shiny associée (voir ci-après).

Pour celles et ceux qui veulent s’amuser, il vous est proposé en option au travail demandé de produire une version accessible et interactive de votre code depuis un navigateur web, via un ordinateur ou un téléphone. Pour ce faire, vous utiliserez le package « shiny » (voir https://www.r-bloggers.com/building-shiny-apps-an-interactive-tutorial/). Un exemple très basique de ce que vous avez à faire se trouve à l’adresse suivante https://flbourgeois.shinyapps.io/Exo_Introduction_R/. Notez qu’il s’agit d’un exemple illustratif, très basique, qui ne traite d’ailleurs que le cas de 2 variables normales. Vous pouvez faire beaucoup mieux !

**Le projet doit être soumis via [Moodle](https://foad-uftmip.univ-toulouse.fr/)**

[La solution](https://github.com/Certificat-Science-des-donnees-Big-Data/Module-sensibilisation/blob/master/Documents/CertificatBigData2020_Calcul_Statistique_SolutionRO.R)

## 2 Éléments d’analyse statistique de données
*A faire sur la période du 10/09 au 29/09*

Cette section vous permettra d’acquérir les notions élémentaires de l’analyse statistique de données. Elles sont la base des méthodes d’inférence et de modélisation mises en œuvre dans la suite.

### 2.1. Documents de base à consulter en autonomie sur [`wikistat.fr`](http://wikistat.fr/)

- [Statistique élémentaire : Introduction](http://wikistat.fr/pdf/st-l-Intro-statElem.pdf)
- [Statistique descriptive unidimensionnelle](http://wikistat.fr/pdf/st-l-des-uni.pdf)
- [Statistique descriptive bidimensionnelle](http://wikistat.fr/pdf/st-l-des-bi.pdf)
- [Estimation statistique](http://wikistat.fr/pdf/st-l-inf-estim.pdf)
- [Tests statistiques](http://wikistat.fr/pdf/st-l-inf-tests.pdf)

### 2.2. Travail personnel demandé

Le travail attendu est un travail personnel d’autoévaluation de votre maîtrise des concepts et méthodes d’analyse statistique étudiées dans les documents de base, en les appliquant au jeu de données du pic d’ozone de la ville de Rennes. Vous êtes invités à consulter le [tutoriel en R](https://github.com/wikistat/StatElem/blob/master/StatElem-R-Ozone.ipynb) sur lequel vous pourrez aussi récupérer le jeu de données. Vous trouverez ci-après, sans caractère limitatif, une liste de thèmes auxquels vous pouvez réfléchir en y apportant une ou plusieurs réponses basées sur les concepts étudiés dans cette section, comme par exemple:

- Décrire (type de données, moyenne, variance, moments,...) et tracer la distribution statistique des variables;
- Tester la normalité des variables;
- Calculer l’incertitude de la moyenne et de l’écart-type des variables;
- Analyser la corrélation entre 2 variables; 
- Tester la nullité du coefficient de corrélation linéaire ;
- ...

Toutes ces études feront l’objet d’une restitution en groupe lors de la séance en <ins> ligne du 1er octobre </ins> et de discussions lors des séances hors présentiel (contactez alors les enseignants florent.bourgeois@ensiacet.fr et rachid.ouaret@ensiacet.fr ou via Slack).


## 3 Modélisation statistique
*A faire sur la période du 10/09 au 29/09*

Cette section vous permettra d’acquérir et de mettre en œuvre 2 méthodes de régression couramment utilisées dans l’analyse de données massives : la régression linéaire multiple et la régression logistique.

### 3.1. Documents de base à consulter en autonomie [`wikistat.fr`](http://wikistat.fr/)
 
- [Introduction à la modélisation statistique](http://wikistat.fr/pdf/st-m-modlin-intro.pdf)
- [Modèle gaussien: régression linéaire multiple](http://wikistat.fr/pdf/st-m-modlin-regmult.pdf)
- [Modèle binomial ou régression logistique](http://wikistat.fr/pdf/st-m-modlin-reglog.pdf)
 
### 3.2. Travail personnel demandé

Le travail attendu est un travail personnel d’autoévaluation de votre maîtrise de la régression linéaire multiple et de la régression logistique, en les appliquant à la prédiction du pic d’ozone de la ville de Rennes. Vous pouvez également utiliser des données plus « locales », issues de http://data-atmo-occitanie.opendata.arcgis.com/datasets (données de la qualité de l’air en Occitanie) et/ou de https://data.toulouse-metropole.fr/pages/accueil/ (données publiques Toulouse Métropole, notamment données météo).
Vous trouverez ci-après, sans caractère limitatif, une liste de sujets auxquels vous êtes invité à réfléchir en y apportant une ou plusieurs réponses basées sur les concepts étudiés dans cette section : 

- Calculer les paramètres des modèles de régression (linéaire multiple et logistique) liant la variable pic d’ozone aux autres variables explicatives;
- Calculer l’intervalle de confiance de ces paramètres;
- Tester la significativité des paramètres;
- Examiner la qualité des modèles de régression, en ajustement et en prédiction;
- Quelles sont les incertitudes associées à la prédiction ?;
- Quel est le « bon » modèle à choisir : nombre de paramètres, valeurs des paramètres,... ?;
- ...

Vous pouvez également nous soumettre ce travail (florent.bourgeois@ensiacet.fr et rachid.ouaret@ensiacet.fr ou via [Moodle](https://foad-uftmip.univ-toulouse.fr/)), sous la forme d’un notebook R ou d’une application Shiny pour information et retour, si besoin.


_____

## 4 Introduction à Python
*A faire sur la période du 1/10 au 24/10*

*Python* et ses librairies produisent moins de résultat utiles que R à l'interprétation statistique mais fournissent des codes généralement plus efficaces pour aborder le traitement de données massives.

Des [tutoriels](https://github.com/wikistat/Intro-Python) proposent une introduction à Python et une sélection des commandes utiles au statisticien et / ou *data scientist*.  

Une connaissance experte de Python n'est pas indispensbale au suivi de ce module; ces tutoriels peuvent être sautés en première lecture. 


## 5 Exploration Multidimensionnelle
*A faire sur la période du 1/10 au 24/10*

Le choix a été fait de mettre plus particulièrement l'accent sur des exemples d'application issus du monde industriel (données physiques quantitatives) plutôt que des applications (données qualitatives) de type sondage,  marketing ou fouille de textes... Comme écrit plus haut, l'introduction à d'autres méthodes et d'autres exemples d'application sont à rechercher dans les ressources des autres niveaux (2 et 4) d'approfondissement.


### 5.1 Documents de base à consulter en autonomie

- [Introduction](https://github.com/Certificat-sciences-des-donnees-bigdata/Module-sensibilisation/blob/master/Documents/csdmsIntro.pdf): De la statistique à la *Science des Données* en passant par la fouille de données (*Data Mining*).
- [Exploration ](https://github.com/Certificat-sciences-des-donnees-bigdata/Module-sensibilisation/blob/master/Documents/csdmsExplo.pdf) en grande dimension avec l'analyse en composantes Principales (ACP), l'analyse factorielle discriminante (AFD); classification non supervisée (*clustering*) avec *k-means*.

### 5.2 Tutoriels à réaliser en automnomie

[**Télécharger**](https://github.com/Certificat-sciences-des-donnees-bigdata/Module-sensibilisation/archive/master.zip) l'ensemble de l'archive du dépôt ou *cloner* le dépôt si vous avez déjà un compte GitHub pour exécuter les tutoriels.

Réaliser ces tutoriels en autonomie:

1. [Intro-ACP-AFD](https://github.com/Certificat-sciences-des-donnees-bigdata/Module-sensibilisation/blob/master/Calepins/CSdD-Intro-ACP-AFD-Python.ipynb)
2. [Adaptation statistique](https://github.com/Certificat-sciences-des-donnees-bigdata/Module-sensibilisation/blob/master/Calepins/CSdD-Pic-Ozone-Python.ipynb) et prévision de la concentration en ozone. Traiter la première partie: *Exploration*.
3. [Segmentation d'image](https://github.com/Certificat-sciences-des-donnees-bigdata/Module-sensibilisation/blob/master/Calepins/CSdD-Cluster-Mars-Python.ipynb) et cartographie de la surface de Mars.

**Travail personnel demandé**: Préparer les réponses aux questions **Q** qui jalonnent chaque tutoriel.


### 5.3 Présentiel le lundi 25 octobre 2021

- Revue des points délicats du cours et des questions soulevées dans les tutoriels

- Tutoriel *fil rouge*: [Reconnaissance d'activité](https://github.com/Certificat-sciences-des-donnees-bigdata/Module-sensibilisation/blob/master/Calepins/CSdD-ML4IoT-Har-Python.ipynb) à partir des enregistrements d'un smartphone. Traiter la première partie: *Exploration*.

D'autres exemples sont disponibles dans le dépôt [`github - wikistat - Exploration`](https://github.com/wikistat/Exploration).

## 6 Principes de l'Apprentissage Statistique
*A faire sur la période du 1/10 au 24/10*

### 6.1 Document de base à consulter en autonomie

- [Principes de l'Apprentissage Statistique](https://github.com/Certificat-sciences-des-donnees-bigdata/Module-sensibilisation/blob/master/Documents/csdmsApprent.pdf) 

### 6.2 Tutoriels à réaliser en autonomie

- [Classification supervisée](https://github.com/Certificat-sciences-des-donnees-bigdata/Module-sensibilisation/blob/master/Calepins/CSdD-Intro-Apprent-Python.ipynb) de données synthétiques dans **R**²
- [Adaptation statistique](https://github.com/Certificat-sciences-des-donnees-bigdata/Module-sensibilisation/blob/master/Calepins/CSdD-Pic-Ozone-Python.ipynb) et prévision de la concentration en ozone. Deuxième partie: *Apprentissage et Prévision*.

**Travail personnel demandé**: Préparer les réponses aux questions **Q** qui jalonnent chaque tutoriel.

### 6.3 Présentiel le lundi 25 octobre 2021 

- Revue des points délicats du cours et des questions soulevées dans les tutoriels

- Tutoriel *fil rouge*: [Reconnaissance d'activité](https://github.com/Certificat-sciences-des-donnees-bigdata/Module-sensibilisation/blob/master/Calepins/CSdD-ML4IoT-Har-Python.ipynb) à partir des enregistrements d'un smartphone. Deuxième partie: *Apprentissage et Reconnaissance*.

D'autres exemples sont disponibles dans le dépôt [`github-wikistat-Apprentissage`](https://github.com/wikistat/Apprentissage).


## 7 Optimisation

<ins> Séance en présentiel le mardi 26 octobre 2021. </ins> 

## 8 Techniques de virtualisation et containerisation, les plateformes cloud

<ins> Séance en présentiel le mercredi 27 octobre 2021 </ins>


