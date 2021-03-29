[PROJECT](./index.html) |[PROJECT](./index.html) | [MEETINGS](./meetings.html) | [TEAM](./team.html) | [ORGA](./orga.html) | [DATA](./pages/data.html)  | [TECH](./tech.html) | [ROADMAP](./roadmap.html) | [REFERENCES](./references.html)

> Ce document décrit le cadrage fonctionnel du projet OpenGeoScales présenté dans le cadre de la saison 9 du programme Data For Good. Un document technique complémentaire présentant des premières explorations des données liées aux émissions des gaz à effet de serre est disponible [dans ce lien](https://opengeoscales.github.io/CarbonData/).
>
> Mots clé: `Open Data`, `Geospatial scales`, `Climate Change`, `GHG emissions`, `Standardization`, `Open Source`
>
> Auteur & porteur de projet: Saif Shabou
> 
> Date: 05/03/2021



## Contexte

Les enjeux environnementaux prennent de plus en plus d’importance dans les politiques publiques ainsi que dans notre vie quotidienne.  La connaissance de l’état de notre planète et de l’impact des activités humaines sur l’environnement nécessite **un accès libre et facile à des données fiables, consolidées, agrégées et documentées**.
Alors que plusieurs plateformes et portails d’open data publient des données environnementales pertinentes (qualité d'air, émissions de gaz à effet de serre, risques naturels, ressources énergétiques…), l’usage de ces données s’avère souvent complexe et fastidieux. Un travail d’identification et de cartographie des différentes sources ainsi que des traitements de nettoyage, recodage, normalisation, croisement, consolidation et agrégation à différentes échelles géographiques est souvent nécessaire avant de pouvoir exploiter les données disponibles.

Pour remédier à ces difficultées, nous proposons dans le cadre du projet OpenGeoScales de construire **un point d'accès centralisé à des données environnementales standardisées et agrégées à différentes échelles géographiques**. En plus de fournir des données environnementales fiables et normalisées, OpenGeoScales propose un **accès libre aux traitements** implémentés sur les données brutes collectées de diverses sources et ambitionne de fédérer **une communauté open source** participant à la production des données et des outils nécessaires pour les explorer.

## Le projet

### Périmètre

Le projet proposé dans le cadre de la saison 9 de Data for Good consiste à implémenter la première brique d’OpenGeoScales consacrée à la consolidation et l’harmonisation des données liées aux **émissions des gaz à effets de serre (GESs)**. Pour ce prototype, seulement les données d’émissions de GESs à différentes échelles du **territoire français** seront considérées, tout en prenant en compte les contraintes d’adaptation à d'autres territoires. 

-------

**Le livrable principal de cette saison consiste en une base de données qui réunit les différentes données d’émissions de GESs à différentes échelles en France accompagnée des traitements appliqués sur les données brutes pour les harmoniser ainsi qu’une API permettant d’accéder et de requêter les données standardisées.**

-------


### Livrables 

Plusieurs livrables intermédiaires sont nécessaires afin d’atteindre le principal objectif défini pour la saison 9:

#### Données brutes schémas sources:

- Une **cartographie** complète des sources de données liées aux émissions de gaz à effets de serre à différentes échelles spatio-temporelles en France.
- Une **exploration** des données identifiées: Bilan carbone (ADEME), Inventaire national (CITEPA), inventaire territorialisé (CITEPA)...
- Une **documentation technique** des sources des données explorées: formats, champs,  couverture spatiale et temporelle, modes de collecte, protocole de mesure, fréquence de mise à jour, indice de confiance ou de fiabilité…

#### Données brutes schémas standardisés:

- Développement de **modèles de données** standardisés qui permettent d'intégrer les différentes données brutes identifiées avec des tables d'association par source de données.
- Alimentation d’une **base de données** qui centralise les différentes sources de données sélectionnées dans le nouveau format. Dans un premier temps, cette base sera alimentée uniquement au chargement initial des données sources. Une alimentation automatique de cette base en fonction de la fréquence d’actualisation des données est à prévoir pour des améliorations futures.

#### Données consolidées schémas standardisé:

- Application de **traitements de transformations** sur les données brutes: normalisation, recodage, agrégation, nettoyage...
- Génération de **rapports d'analyse des données** et d'articles de vulgarisation afin d’en identifier la complétude et d’en extraire des insights sur les émissions des GESs en France: comparaison par villes et secteurs, évaluation des sources...

#### API:

- Développement et déploiement d’**APIs** pour requêter la base de données standardisée et permettre d’accéder rapidement aux données des émissions par entité géographique, échelle spatiale, catégories d’activités, scope…
- Documentation technique de l’API

## Utilisateurs

OpenGeoScales s’adresse à différents profils de potentiels utilisateurs ayant besoin de données qualifiées sur les émissions de GESs à différentes échelles accompagnées d’une documentation exhaustive sur ces sources et sur les traitements d’amélioration qui leurs sont appliqués:

- **Journalisme:** Data journalistes, blogueurs  intéressés par les données carbone.
- **Bureaux d’études en conseil carbone et environnement**
- **Organismes non gouvernementaux** militants dans les questions climatiques et environnementales ([Notre affaire à tous](https://notreaffaireatous.org/), [The Shift Project](https://theshiftproject.org/), [Les amis de la terre](https://www.amisdelaterre.org/), [Association Bilan Carbone](https://www.associationbilancarbone.fr/), [Climate Chance](https://www.climate-chance.org/), [World Resources Institut](https://www.wri.org/data-lab), [Our World In Data](https://ourworldindata.org/), [Carbon Disclosure Project](https://www.cdp.net/en/investor/ghg-emissions-dataset)…)
- **Spécialiste des données** travaillant sur des projets nécessitant l’usage des données d’émissions de GESs.
- **Académique:** étudiants, doctorants et chercheurs ayant besoin d'exploiter et de croiser des indicateurs d’émissions de GESs

Un travail de recensement et de spécification des usages des données des GESs et des besoins de qualification associées est nécessaire tout au long de la première phase du projet

## Contributeurs

En tant que projet open source, la contribution à OpenGeoScales est ouverte à toute personne intéressée par les données liées aux enjeux climatiques, en fonction bien sûr des expertises et compétences:

- **Expertise data:**
  - Collecte et stockage des données
  - Exploration des données et identification des potentiels traitements nécessaires pour les exploiter (nettoyage, filtrage, recodage, agrégation…)
  - Modélisation de schémas standardisés pour regrouper les données collectés
  - Développement de pipeline de traitements 
  - Développement d’API de requêtage
  
- **Expertise métier:**
  - Cartographie et documentation des données d’émissions de GESs.
  - Spécification des cas d’usages des données 
  
- **Expertise scientifique:**
  - Vulgarisation scientifique des concepts et méthodes liées à la quantification des émissions des GESs.

## Partenaires

### Data For Good

Le projet OpenGeoScales présente des synergies avec des précédents projets d’accélération Data For Good au niveau de la thématique (émissions des GESs) et du livrable (Standardisation des données et API).

- Projets portant sur des thématiques liées aux émissions des GESs: [Outil BEGES](https://dataforgood.fr/projects/7_Beges.html), [2TONNES](https://dataforgood.fr/projects/7_2tonnes.html),  [CO2 Plume Detector](https://dataforgood.fr/projects/7_OCO2.html), [banque mondiale - risques naturels](https://github.com/dataforgoodfr/batch8_worldbank), [carbone 4](https://github.com/dataforgoodfr/batch8_carbone4).
- Projet aboutissant à une standardisation de données publiques et développement d’API pour y accéder: [ARKHN](https://dataforgood.fr/projects/5_arkhn.html)

Des rapprochements avec les contributeurs de ces projets sont nécessaires afin de profiter de leur retour d'expérience et de partager les connaissances (méthodologique, théorique et technique) pour mieux mener le projet OpenGeoScales.

### Appui métier

Un rapprochement avec les principaux acteurs publics et privés en conseil carbone est prévu tout au long du projet afin d’avoir un appui méthodologique et fonctionnel sur l’usage des données d’émissions de GESs. Parmi les acteurs identifiés, on peut citer: l’ADEME, l’Association Bilan Carbone, la CITEPA, l’Institut de Formation Carbone…

Le recensement des [principaux acteurs du conseil carbone](https://www.associationbilancarbone.fr/cartographie-des-acteurs/) effectué par l’Association Bilan Carbone peut être utilisé pour cibler des potentiels partenariats: 

### Projets inspirants

- [Covid Tracking Project:](https://covidtracking.com/)  Le Covid Tracking Project est un projet Open Source développé par des volontaires afin de collecter, compiler et partager des données et des indicateurs journaliers liés aux impacts du Covid-19 aux Etats-Unis. Le projet a eu un grand succès vu que les données publiées sont devenues les principales sources de différents médias et travaux scientifiques. Le format des produits délivrés dans le cadre du Covid Tracking Project correspondent aux livrables prévus pour le projet OpenGeoScales: une base de données consolidée téléchargeable, des APIS pour accéder aux données et un site web qui répertorient différents articles d’analyse de données montrant les potentialités des données associé à des outils de dataviz performants et adaptés aux métriques produites.

- [Our World In Data:](https://ourworldindata.org/co2-and-other-greenhouse-gas-emissions) Our World In Data est une ONG spécialisée dans les questions de développement et d’environnement. Elle publie à travers son site des rapports d’analyse de données liés aux problématiques environnementales et sociales : émissions CO2, énergie, déforestation, qualité d’air… 

- [The Shift Data Portal:](https://www.theshiftdataportal.org/) Outil d’exploration et visualisation des données énergétiques et climatiques développé par le think tank The Shift Project.

- [Climate Watch (World Resources Institute):](https://www.climatewatchdata.org/) Climate Watch propose des données ouvertes, des visualisations et des analyses pour aider les décideurs, les chercheurs et les autres parties prenantes à recueillir des informations sur les progrès climatiques des pays.

- [Open Climate Data:](https://openclimatedata.net/) Open Climate Data propose un repository Github de différentes données en rapport avec les enjeux climatiques (émissions CO2, actions climats, pays signataires des accords climats…) ainsi que des notebooks qui explorent leurs contenus.

## Roadmap

Le schéma ci-dessous présente une feuille de route préliminaire pour délivrer une première itération du projet OpenGeoScales restreinte sur la standardisation et l’exposition des données de GESs à différentes échelles du territoire Français.

![Roadmap](https://github.com/OpenGeoScales/Management/blob/main/images/Roadmap.png?raw=true)

### Et après?

La roadmap présentés ci-dessus présente les phases de développement durant l’itération de 3 mois de la saison 9 de Data For Good. Des perspectives d’évolution et d’élargissement sont prévus après la saison d’accélération:

- **Nouvelles fonctionnalités:**
  - Construction de site web pour héberger l’ensemble des articles produits et centraliser la documentation technico-fonctionnelle des données et de l’API ainsi que les différentes connaissances formalisées autour des émissions des GESs.
  - Construction de dashboards et d’outils de géo-visualisation des données compilées.
- **Reproduction sur d’autre thématiques:** Implémenter le même processus sur d’autres types de données liées aux enjeux climatiques: énergie, risques naturels, qualité d’air, déforestation…
- **Reproduction sur d’autres territoire:** Reproduire le travail effectué sur d’autres territoire et étendre la communauté Open Source
- **Communication:** 
  -  Partage et communication des résultats et du produit réalisé dans le cadre d'événements qui adressent les questions climate/data.
  -  Elargir le cercle de partenariat 
- **Performance:** Identifier les pistes d’améliorations en termes de performance et de structuration des traitements des données.

## Gestion de projet

Le code source sera disponible sur Github. Un repository dédié aux données carbone a déjà été créé et est utilisé: [Repository CarbonData](https://github.com/OpenGeoScales/CarbonData)

Github Projects sera utilisé comme outil de gestion du développement des différentes fonctionnalités. Il permet de suivre l'évolution des tâches matérialisées comme des ‘issues’ via **un board Kanban automatisé**. Un premier projet est en cours et qui peut être consulté ici: [CarbonData Project Board](https://github.com/OpenGeoScales/CarbonData/projects/2)

Les itérations seront basées sur des sprints de 2 semaines avec des objectifs bien précis à définir en amont.

Les modalités de contribution seront co-définies avant le début de la saison avec l’attribution de différents rôles aux contributeurs, en fonction de leurs appétences et expertises.

Un canal Slack sera mis en place pour assurer la communication entre les contributeurs.

[link to meetings](https://github.com/OpenGeoScales/Management/blob/gh-pages/Meetings.md)

[link to meetings](./Meetings.html)
