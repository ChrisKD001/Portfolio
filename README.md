# Analyse Interactive des Performances Hôtelières avec Power BI - HOTEL GROUP

## À Propos

Ce projet Power BI fournit des tableaux de bord interactifs pour Atliq, analysant des indicateurs clés de performance hôtelière tels que le chiffre d'affaires, le taux d'occupation et le revenu par chambre disponible (RevPAR). Il offre des informations sur les tendances de performance hebdomadaires, l'utilisation des chambres et la satisfaction client, aidant ainsi à optimiser les opérations hôtelières et la prise de décision.

## Présentation Power Point

À l'issue de ce travail, j’ai été amené à présenter le fruit de mon travail. Cependant, j’ai dû préparer une présentation Power Point. Vous pouvez consulter ma présentation Power Point en cliquant [ICI](lien_vers_votre_presentation).

## Contexte

HOTEL GROUP possède plusieurs hôtels 5 étoiles principalement situés dans des villes comme l'Égypte, le Cameroun, le Kenya et le Sénégal, totalisant 7 propriétés :

* Genesis Bouns
* Maxus Bouns
* Matrix Bouns
* Escape Bouns
* Maserati Bouns
* Infiniti Bouns
* Shelby Bouns

## Énoncé du Problème

HOTEL GROUP connaît un déclin de sa part de marché et de ses revenus dans les catégories d'hôtels d'affaires et de luxe. Ce déclin est attribué à des initiatives stratégiques prises par les concurrents et à une prise de décision inefficace au sein de la direction de HOTEL GROUP.

Le Directeur Général de HOTEL GROUP vise à regagner des parts de marché et des revenus en mettant en œuvre des décisions basées sur les données.

## Ma Tâche

Ma tâche consiste à concevoir un tableau de bord qui offre des informations clés sur l'activité de HOTEL GROUP en suivant les indicateurs essentiels du secteur hôtelier. L'objectif est deLocaliser les domaines où HOTEL GROUP perd des revenus et de fournir des informations et des recommandations exploitables pour reconquérir sa part de marché.

## Jeu de Données

Le jeu de données comprend cinq fichiers CSV couvrant les dates, les hôtels, les chambres, les réservations agrégées et les réservations individuelles. Les colonnes clés fournissent des informations sur les catégories de chambres, les détails des réservations, le nombre de clients, les revenus et les évaluations, soutenant une analyse complète des opérations hôtelières et du comportement des clients.

Dans ce projet, les données ont été initialement chargées à partir de fichiers Excel dans Power BI. J'ai utilisé Power Query pour nettoyer les données en supprimant les doublons, en corrigeant les valeurs manquantes et en formatant les colonnes. Des relations ont ensuite été établies entre les tables pour permettre une analyse complète. Une table nommée "Mesures Clés" a été créée pour calculer des indicateurs importants et fournir des informations exploitables.

À propos des fichiers, nous avons :

* **dim\_date :**
    * Contient des informations sur les dates en mai, juin et juillet.
* **dim\_hotels :**
    * Fournit des détails sur les hôtels.
* **dim\_rooms :**
    * Décrit les types de chambres disponibles dans les hôtels.
* **fact\_aggregated\_bookings :**
    * Fournit des informations agrégées sur les réservations.
* **fact\_bookings :**
    * Contient des informations détaillées sur les réservations.

Ce jeu de données fournit des informations complètes sur les hôtels, les chambres et les réservations, facilitant l'analyse et la prise de décision dans le secteur de l'hôtellerie.

## Étapes Suivies

1.  Importation des fichiers CSV dans l'éditeur Power Query.
2.  Nettoyage et transformation des données : vérification des doublons et des valeurs nulles, et assurance que le type de données de toutes les colonnes était correct.
3.  Note : dans l'industrie hôtelière, le vendredi et le samedi sont considérés comme des week-ends, et du dimanche au jeudi comme des jours de semaine.
4.  Création d'une colonne calculée à l'aide de DAX pour catégoriser les jours en jours de semaine ou week-ends.

## Création de Mesures

Le RevPAR (Revenu Par Chambre Disponible), l'ADR (Tarif Journalier Moyen), le DSRN (Nombre de Chambres Disponibles à la Vente), le taux d'occupation (%) et le taux de réalisation (%) sont quelques-uns des indicateurs clés utilisés dans le secteur hôtelier pour suivre la performance de l'industrie.

## Tableau de Bord Interactif

Vous pouvez consulter le tableau de bord Power BI interactif [ICI](lien_vers_votre_tableau_de_bord).

## Outils Utilisés

* **Excel :** Chargement et préparation des données.
* **Power Query :** Nettoyage et transformation des données.
* **DAX (Data Analysis Expressions) :** Modélisation et calculs des données.
* **Power BI :** Création et visualisation du tableau de bord.

## Informations Clés

**Métriques Générales :**

* Chiffre d'affaires total : 1709 millions $
* RevPAR moyen : 7,35
* Taux d'occupation moyen : 58%
* ADR moyen : 12,7
* % de Réalisation : 70%
* % d'Annulation : 24% - 26%

**Propriétés les Plus Performantes :**

* INFINITI Hôtel, Cameroun : CA : 101,51 M $, Taux d'occupation : 66,23%
* MAXUS Hôtel, Cameroun : CA : 212,44 M $, Taux d'occupation : 66%

**Propriétés les Moins Performantes :**

* SHELBY Hôtel, Cameroun : Revenus : 66,13 M $, Taux d'occupation : 44,62%
* GENESIS Hôtel, Sénégal : Revenus : 54,49 M $, Taux d'occupation : 44,40%

**Observations :**

* Le chiffre d’affaires net global est de 1709 M $.
* Le nombre total de réservations était de 135 K.
* Pourcentage d'annulations : 24,83%.
* Le revenu moyen par réservation est de 12700 $.
* Nombre total d’annulation : 33 521.
* Le montant de la perte de revenus due à l’annulation est d'environ 425,72 millions de dollars.

* Dans l’ensemble, le revenu moyen généré par les clients qui ont réservé des sièges le week-end et en semaine est similaire : 12,72 K $ pour les réservations de week-end et 12,68 K $ pour les réservations en semaine.

* Le plus grand nombre de réservations provenaient de sources classées dans la catégorie "autres". Une investigation plus approfondie est nécessaire pour identifier ces sources. La deuxième source de réservations la plus importante est MakeYourTrip. Étant donné que cette plateforme de réservation génère le plus de revenus, un élargissement du partenariat est recommandé. Les magasins hors ligne ont généré le moins de revenus, ce qui suggère un besoin d'expansion de ce canal pour toucher les clients qui ne réservent pas en ligne.

* Les plateformes ayant enregistré le plus grand nombre de réservations ont également enregistré le plus grand nombre d'annulations, et vice-versa.

* Les revenus par ville métropolitaine sont les suivants : Cameroun (669 M $) > Sénégal (420 M $) > Kenya (325 M $) > Égypte (295 M $).

* Dans chaque ville métropolitaine, l’hôtellerie de luxe a généré plus de chiffre d’affaires que l’hôtellerie d’affaires.

## Interprétation et Recommandations

Sur la base des informations tirées du tableau de bord, il est évident que les chaînes de HOTEL GROUP perdent des parts de marché et voient leurs revenus diminuer en raison d'une mauvaise utilisation des stratégies de tarification.

Les hôtels peuvent augmenter leurs revenus en utilisant une tarification dynamique, qui ajuste les prix en fonction de la demande. Pendant les périodes de forte affluence, comme les vacances, les prix augmentent, et pendant les périodes plus calmes, ils diminuent.

Les hôtels peuvent également augmenter leurs revenus en ajustant les prix pour les jours de semaine et les week-ends en fonction de la demande. Ils peuvent également promouvoir des offres de petit-déjeuner en semaine, souvent populaires pour les réunions d'affaires, afin d'améliorer leur stratégie de tarification.

Dans le paysage en ligne actuel, les évaluations des hôtels jouent un rôle crucial, car les clients choisissent souvent les hôtels en fonction des évaluations affichées. Pour les hôtels moins bien notés, il est essentiel de résoudre les problèmes directement en interagissant avec les clients, en comprenant leurs besoins et en résolvant les problèmes sur le terrain.

## Conclusion

Hotel Group peut reconquérir sa part de marché en utilisant une tarification dynamique et en ajustant les tarifs pour les week-ends et les jours de semaine, en attirant davantage de clients avec des options de prix flexibles.

## Contact

Pour toute question, veuillez envoyer un e-mail à carterchris571@gmail.com.
