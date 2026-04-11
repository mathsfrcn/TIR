# État de l'Art : Applications Interdisciplinaires du Solveur Toulbar2

![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Termin%C3%A9-brightgreen)
![Version](https://img.shields.io/badge/Version-v12.5-blue)

## 📖 Présentation du Projet
Ce projet présente une revue de l'état de l'art du solveur Toulbar2 et de son impact interdisciplinaire. Toulbar2 est un solveur C++ open-source spécialisé dans les problèmes d'optimisation discrète utilisant le formalisme des réseaux de fonctions de coût (Cost Function Networks - CFN). 

Il est conçu pour résoudre des problèmes de satisfaction de contraintes valuées (VCSP) et pondérées (WCSP) en s'appuyant sur un algorithme de recherche par séparation et évaluation (Branch-and-Bound) couplé à des techniques de cohérence d'arc souple (Soft Arc Consistency).

## 🧬 Domaines d'Application Explorés

Ce document analyse les performances et les adaptations du solveur à travers quatre domaines majeurs :

### 1. Résolution de Problèmes Combinatoires
Toulbar2 surpasse régulièrement d'autres solveurs de pointe sur des problèmes complexes.
* **Théorie des graphes :** Résolution du problème d'édition de clusters (Zahn's problem) via la programmation par contraintes.
* **Intégration discrète :** Calcul de fonctions de partition en haute dimension en contournant la malédiction de la dimensionnalité.
* **Problèmes classiques NP-difficiles :** Optimisation du problème des N-Reines pondéré, du problème d'affectation quadratique, et du problème du sac à dos avec graphe de conflits (KPCG).

### 2. Bio-informatique et Sciences de la Vie
Le solveur est un outil de référence pour la modélisation moléculaire.
* **Conception de protéines (CPD) :** Identification de la séquence d'acides aminés minimisant l'énergie de la protéine (GMEC).
* **Conception multi-états :** Capacité à favoriser des interactions ciblées tout en évitant les assemblages indésirables.
* **Approches hybrides :** Couplage de modèles d'apprentissage profond avec Toulbar2 pour générer des séquences avec une meilleure qualité globale et un contrôle explicite des contraintes.

### 3. Gestion et Planification des Ressources
Les CFN se révèlent particulièrement adaptés aux problèmes classiques de recherche opérationnelle.
* **Allocation spatio-temporelle :** Planification de la rotation des cultures agricoles et résolution des conflits de trajectoires dans le trafic aérien (méthode Lumberjack).
* **Ressources humaines :** Génération d'emplois du temps complexes (ex: personnel infirmier) grâce à l'intégration de contraintes globales souples.
* **Réseaux :** Gestion et minimisation des conflits d'abonnement aux services de télécommunications.

### 4. Intelligence Artificielle et Machine Learning
Face à des environnements incertains, Toulbar2 évolue pour s'intégrer à des architectures neuronales et probabilistes.
* **Systèmes Neuro-symboliques :** Utilisation de réseaux de neurones pour traiter les données sensorielles brutes (perception), tandis que Toulbar2 assure le raisonnement et l'optimisation discrète exacte.
* **Satisfiability Modulo Counting (SMC) :** Amélioration des systèmes hybrides intégrant la logique et les probabilités (comme KOCO-SMC) en réduisant les temps de calcul.

## ⚙️ Méthodologie et Algorithmes
Le solveur exploite diverses transformations préservant l'équivalence (EPT) pour déplacer les coûts et obtenir des bornes inférieures optimales. Les techniques d'inférence incluent :
* FDAC (Full Directional Arc Consistency).
* EDAC (Existential Directional Arc Consistency).
* VAC (Virtual Arc Consistency).
* OSAC (Optimal Soft Arc Consistency).

De plus, l'utilisation d'algorithmes heuristiques gloutons (comme MinCost MaxClique) en amont permet d'accélérer significativement l'élagage de l'arbre de recherche sur des problèmes massifs.

## 👥 Auteurs
Ce projet a été réalisé dans le cadre du M1 IMA/RO en UE Simulation aléatoire :

-  GARCIA Hugo.
  hugo.garcia@univ-tlse3.fr
-  GAUTHIER Philippe.
  philippe.gauthier@univ-tlse3.fr 
-  SANFILIPPO Marco.
  marco.sanfilippo@univ-tlse3.fr
-  FRANCINE-HABAS Mathis.
  mathis.francine-habas@univ-tlse3.fr
