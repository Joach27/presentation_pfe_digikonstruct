# DIGICONSTRUCT - Plateforme Intelligente de Traitement de Documents en Électrotechnique

---

&nbsp;

&nbsp;

&nbsp;

> **Page de garde**

---

**Établissement :** HESTIM - Engineering & Business School  
**Année universitaire :** 2025 – 2026  
**Formation :** Génie Informatique / Ingénierie Logicielle  

&nbsp;

# Développement d'une Plateforme Intelligente de Traitement de Documents Techniques en Électrotechnique : Extraction Automatisée, Détection de Symboles et Agent Conversationnel IA

&nbsp;

**Période de stage :** [DATE DÉBUT] – [DATE FIN]  
**Thème :** Intelligence Artificielle appliquée au traitement de documents d'ingénierie électrique

&nbsp;

| | |
|---|---|
| **Logo établissement** | **Logo entreprise** |
| [IMAGE : Logo HESTIM] | [IMAGE : Logo entreprise d'accueil] |

&nbsp;

**Réalisé par :** [NOM Prénom]  
**Maître de stage :** [NOM Prénom] - [Intitulé du poste]  
**Tuteur pédagogique :** [NOM Prénom]  

---

&nbsp;

---

## Dédicaces

&nbsp;

*À mes parents, pour leur soutien indéfectible et leur confiance sans faille tout au long de ce parcours.*

*À mes proches et amis, dont les encouragements constants ont été une source de motivation précieuse.*

*À tous ceux qui, de près ou de loin, ont contribué à façonner l'ingénieur que je suis en train de devenir.*

&nbsp;

---

&nbsp;

---

## Remerciements

&nbsp;

La réalisation de ce mémoire de stage n'aurait pu voir le jour sans le concours de nombreuses personnes à qui je tiens à exprimer ma profonde gratitude.

Je remercie en premier lieu **[NOM Maître de stage]**, [intitulé du poste], qui m'a accueilli au sein de l'entreprise avec bienveillance et professionnalisme. Sa disponibilité, ses conseils éclairés et sa confiance accordée dès le premier jour m'ont permis de m'immerger pleinement dans des problématiques techniques stimulantes. Ses retours rigoureux et ses orientations stratégiques ont été déterminants dans la qualité des livrables produits.

Je remercie chaleureusement **[NOM Tuteur pédagogique]**, tuteur pédagogique à HESTIM, pour son suivi attentif, ses remarques constructives et son accompagnement tout au long de ce stage. Sa pédagogie et son exigence académique ont contribué à élever la rigueur de ce travail.

J'adresse également mes sincères remerciements à l'ensemble de l'équipe technique de l'entreprise d'accueil, notamment [NOM Collègue 1] et [NOM Collègue 2], pour leur disponibilité, leurs échanges enrichissants et l'atmosphère collaborative qu'ils ont su instaurer.

Je remercie l'ensemble du corps professoral et administratif de HESTIM pour la qualité de la formation dispensée, qui m'a fourni les bases théoriques et méthodologiques nécessaires à l'accomplissement de ce stage.

Enfin, je tiens à exprimer ma reconnaissance envers ma famille, dont le soutien moral et affectif a constitué un appui inestimable durant toute la durée de cette expérience professionnelle.

&nbsp;

---

&nbsp;

---

## Liste des Acronymes et Abréviations

&nbsp;

| Acronyme | Signification |
|---|---|
| **API** | Application Programming Interface |
| **ASGI** | Asynchronous Server Gateway Interface |
| **BT** | Basse Tension |
| **CRUD** | Create, Read, Update, Delete |
| **CSV** | Comma-Separated Values |
| **DH** | Dirham marocain |
| **DPI** | Dots Per Inch (points par pouce) |
| **ETL** | Extract, Transform, Load |
| **GIN** | Generalized Inverted iNdex |
| **HMI** | Human-Machine Interface |
| **HTTP** | HyperText Transfer Protocol |
| **IA** | Intelligence Artificielle |
| **JSON** | JavaScript Object Notation |
| **JSONB** | JSON Binary (format PostgreSQL) |
| **JWT** | JSON Web Token |
| **LLM** | Large Language Model |
| **NLP** | Natural Language Processing |
| **NMS** | Non-Maximum Suppression |
| **OCR** | Optical Character Recognition |
| **ORM** | Object-Relational Mapping |
| **PDF** | Portable Document Format |
| **PFE** | Projet de Fin d'Études |
| **PK** | Primary Key (clé primaire) |
| **REST** | Representational State Transfer |
| **SHA** | Secure Hash Algorithm |
| **SPA** | Single Page Application |
| **SQL** | Structured Query Language |
| **SPA** | Single Page Application |
| **UUID** | Universally Unique Identifier |
| **YAML** | YAML Ain't Markup Language |

&nbsp;

---

&nbsp;

---

## Résumé

&nbsp;

Le secteur de l'ingénierie électrique génère quotidiennement des volumes importants de documents techniques - notes de calcul, plans de câblage, catalogues produits - dont le traitement manuel demeure coûteux en temps et sujet aux erreurs humaines. Ce mémoire présente **DIGICONSTRUCT**, une plateforme logicielle développée durant ce stage en vue d'automatiser et d'intelligentiser le traitement de ces documents au sein d'un bureau d'études ou d'une entreprise spécialisée en électrotechnique.

La plateforme s'articule autour de trois modules complémentaires. Le **module d'extraction** exploite la bibliothèque Camelot pour détecter et extraire les tableaux de circuits présents dans les notes de calcul Caneco BT (logiciel de dimensionnement électrique basse tension), puis applique un pipeline de nettoyage automatisé et une couche d'intelligence artificielle basée sur de grands modèles de langage (LLMs) pour structurer les données extraites. Le **module de quantification** permet la détection de symboles électriques sur des plans techniques via la correspondance de gabarits (template matching) avec OpenCV, offrant ainsi un comptage automatisé des équipements. Enfin, le **module catalogue et agent conversationnel** propose une interface de recherche plein texte sur un catalogue de produits électriques, complétée par un agent IA à appel de fonctions permettant des requêtes en langage naturel.

Sur le plan technique, l'architecture repose sur un backend Python FastAPI entièrement asynchrone, une base de données PostgreSQL avec extension pgvector, et un frontend React/Vite. L'intégration multi-fournisseurs LLM (OpenRouter, HuggingFace, Ollama) assure résilience et flexibilité. Les résultats obtenus démontrent la viabilité de l'approche : extraction structurée de notes de calcul multi-pages, détection de symboles avec suppression des faux positifs par NMS, et conversations guidées par outils pour l'interrogation du catalogue.

**Mots-clés :** Traitement de documents PDF, Extraction de tableaux, Intelligence Artificielle, LLM, FastAPI, React, PostgreSQL, Électrotechnique, Caneco BT, Template Matching.

&nbsp;

---

**Abstract**

The electrical engineering sector generates daily large volumes of technical documents - calculation notes, wiring diagrams, product catalogs - whose manual processing remains time-consuming and error-prone. This thesis presents **DIGICONSTRUCT**, a software platform developed during this internship to automate and intelligentize the processing of these documents within an engineering office or a company specializing in electrical engineering.

The platform is built around three complementary modules. The **extraction module** leverages the Camelot library to detect and extract circuit tables from Caneco BT calculation notes (low-voltage electrical sizing software), then applies an automated cleaning pipeline and an AI layer based on Large Language Models (LLMs) to structure the extracted data. The **quantification module** enables the detection of electrical symbols on technical drawings via template matching with OpenCV, thus providing automated equipment counting. Finally, the **catalog and conversational agent module** offers a full-text search interface on an electrical product catalog, augmented by a function-calling AI agent enabling natural language queries.

From a technical standpoint, the architecture relies on a fully asynchronous Python FastAPI backend, a PostgreSQL database with the pgvector extension, and a React/Vite frontend. Multi-provider LLM integration (OpenRouter, HuggingFace, Ollama) ensures resilience and flexibility. Results demonstrate the approach's viability: structured extraction of multi-page calculation notes, symbol detection with false-positive suppression via NMS, and tool-guided conversations for catalog querying.

**Keywords:** PDF document processing, Table extraction, Artificial Intelligence, LLM, FastAPI, React, PostgreSQL, Electrical engineering, Caneco BT, Template Matching.

&nbsp;

---

&nbsp;

---

## Sommaire

&nbsp;

- [Dédicaces](#dédicaces)
- [Remerciements](#remerciements)
- [Liste des Acronymes et Abréviations](#liste-des-acronymes-et-abréviations)
- [Résumé](#résumé)
- **[Introduction Générale](#introduction-générale)**
- **[Chapitre 1 - Contexte, Problématique et État de l'Art](#chapitre-1--contexte-problématique-et-état-de-lart)**
  - 1.1 Présentation de l'entreprise d'accueil
  - 1.2 Contexte du projet
  - 1.3 Problématique et objectifs
  - 1.4 État de l'art : traitement intelligent de documents
  - 1.5 Revue des technologies pertinentes
  - 1.6 Synthèse et positionnement
- **[Chapitre 2 - Analyse, Conception et Architecture du Système](#chapitre-2--analyse-conception-et-architecture-du-système)**
  - 2.1 Analyse des besoins
  - 2.2 Architecture globale de la plateforme
  - 2.3 Conception du module d'extraction
  - 2.4 Conception du module de quantification
  - 2.5 Conception du module catalogue et agent IA
  - 2.6 Modèle de données
  - 2.7 Sécurité et gestion des accès
- **[Chapitre 3 - Implémentation, Tests et Résultats](#chapitre-3--implémentation-tests-et-résultats)**
  - 3.1 Environnement de développement et stack technique
  - 3.2 Implémentation du module d'extraction
  - 3.3 Implémentation du module de quantification
  - 3.4 Implémentation du module catalogue et agent conversationnel
  - 3.5 Interface utilisateur
  - 3.6 Déploiement et infrastructure
  - 3.7 Tests, évaluation et résultats
- **[Conclusion Générale](#conclusion-générale)**
- **[Références Bibliographiques](#références-bibliographiques)**
- **[Annexes](#annexes)**

&nbsp;

---

&nbsp;

---

## Liste des Figures

&nbsp;

| N° | Intitulé | Page |
|---|---|---|
| Figure 1 | Architecture générale de la plateforme DIGICONSTRUCT | - |
| Figure 2 | Organigramme de l'entreprise d'accueil | - |
| Figure 3 | Exemple de note de calcul Caneco BT (format PDF) | - |
| Figure 4 | Pipeline ETL d'extraction : Extract → Clean → Structure → Load | - |
| Figure 5 | Diagramme de classes du module d'extraction | - |
| Figure 6 | Exemple de tableau extrait brut (avant nettoyage) | - |
| Figure 7 | Exemple de tableau nettoyé (après nettoyage) | - |
| Figure 8 | Schéma du pipeline de nettoyage des tableaux | - |
| Figure 9 | Flux de traitement LLM multi-fournisseurs | - |
| Figure 10 | Principe du template matching pour la détection de symboles | - |
| Figure 11 | Résultat de détection sur un plan électrique (avant NMS) | - |
| Figure 12 | Résultat de détection sur un plan électrique (après NMS) | - |
| Figure 13 | Schéma de la base de données relationnelle | - |
| Figure 14 | Architecture du module catalogue avec tsvector GIN | - |
| Figure 15 | Diagramme de séquence de l'agent conversationnel | - |
| Figure 16 | Capture d'écran : interface d'upload et d'extraction | - |
| Figure 17 | Capture d'écran : visualisation des résultats d'extraction | - |
| Figure 18 | Capture d'écran : module de quantification (détections) | - |
| Figure 19 | Capture d'écran : interface du catalogue et chat IA | - |
| Figure 20 | Architecture de déploiement Docker (production) | - |

&nbsp;

---

&nbsp;

---

## Liste des Tableaux

&nbsp;

| N° | Intitulé | Page |
|---|---|---|
| Tableau 1 | Comparatif des bibliothèques d'extraction de tableaux PDF | - |
| Tableau 2 | Comparatif des fournisseurs LLM intégrés | - |
| Tableau 3 | Comparatif des solutions de détection de symboles | - |
| Tableau 4 | Cas d'utilisation principaux et acteurs | - |
| Tableau 5 | Schéma des endpoints REST de l'API | - |
| Tableau 6 | Règles métiers du nettoyage des tableaux (TableCleaner) | - |
| Tableau 7 | Résultats de performance du module d'extraction | - |
| Tableau 8 | Résultats de précision du module de quantification | - |
| Tableau 9 | Jeu de données de test pour l'agent conversationnel | - |

&nbsp;

---

&nbsp;

---

## Introduction Générale

&nbsp;

### Contexte général

La transition numérique du secteur du bâtiment et de l'industrie transforme progressivement les méthodes de travail des ingénieurs et des bureaux d'études techniques. En électrotechnique, les professionnels produisent et manipulent quotidiennement des documents de haute densité informationnelle : notes de calcul de dimensionnement électrique, plans de câblage, bordereaux de matériel et catalogues de produits. Ces documents, souvent générés par des logiciels métier spécialisés tels que **Caneco BT** de l'entreprise IESVE, constituent la mémoire technique des projets. Pourtant, leur exploitation reste largement manuelle : un ingénieur doit extraire à la main les paramètres de circuit pour les réintégrer dans des tableurs, compter visuellement des symboles sur des plans de grande taille, ou consulter des catalogues papier ou PDF pour trouver le bon produit.

Ces opérations répétitives mobilisent des ressources expertes pour des tâches à faible valeur ajoutée, tout en introduisant des risques d'erreur incompatibles avec les exigences de sécurité propres à l'électrotechnique. L'essor récent de l'intelligence artificielle - en particulier les grands modèles de langage (LLM) et la vision par ordinateur - ouvre de nouvelles perspectives pour automatiser ces flux de travail.

### Problématique

C'est dans ce contexte qu'est né le projet **DIGICONSTRUCT** : comment concevoir et développer une plateforme logicielle capable d'automatiser, de bout en bout, le traitement des documents techniques en électrotechnique, depuis l'extraction structurée de données dans des PDF jusqu'à l'interrogation intelligente d'un catalogue de produits ? Et comment orchestrer des technologies hétérogènes - traitement de PDF, vision par ordinateur, LLM, bases de données vectorielles - au sein d'un système cohérent, performant et déployable en production ?

### Objectifs du stage

Les objectifs assignés à ce stage sont les suivants :

1. **Analyser** les besoins métier des utilisateurs finaux (ingénieurs électriciens) et les documenter sous forme de cas d'utilisation.
2. **Concevoir** l'architecture modulaire d'une plateforme web full-stack intégrant extraction PDF, vision par ordinateur et IA générative.
3. **Développer** les trois modules fonctionnels : extraction de notes de calcul, quantification de symboles et agent conversationnel.
4. **Évaluer** les performances de chaque module et les optimiser.
5. **Déployer** la plateforme dans un environnement Dockerisé prêt pour la production.

### Structure du mémoire

Ce mémoire s'organise en trois chapitres. Le **premier chapitre** pose le cadre de l'étude : présentation de l'entreprise d'accueil, analyse du contexte sectoriel, formulation de la problématique et revue de l'état de l'art des technologies mobilisées. Le **deuxième chapitre** détaille la démarche de conception : analyse des besoins, architecture générale, modélisation des données et choix de design. Enfin, le **troisième chapitre** décrit l'implémentation concrète de chaque module, présente les résultats obtenus, et discute des perspectives d'évolution.

&nbsp;

---

&nbsp;

---

# Chapitre 1 - Contexte, Problématique et État de l'Art

&nbsp;

> *Ce premier chapitre pose les fondations conceptuelles et sectorielles du projet. Il présente l'environnement dans lequel le stage s'est déroulé, identifie les lacunes des approches actuelles et situe DIGICONSTRUCT par rapport aux solutions existantes.*

&nbsp;

## 1.1 Présentation de l'entreprise d'accueil

&nbsp;

### 1.1.1 Identité et positionnement

[IMAGE : Logo et façade de l'entreprise d'accueil]

L'entreprise d'accueil est [NOM DE L'ENTREPRISE], [description courte : bureau d'études / société de services en ingénierie / startup spécialisée] spécialisée dans [domaine : électrotechnique, bâtiment, industrie]. Fondée en [ANNÉE] et dont le siège est situé à [VILLE, PAYS], elle intervient principalement sur [marchés cibles : secteur industriel, tertiaire, résidentiel haut de gamme, infrastructures].

L'entreprise compte à ce jour [NOMBRE] collaborateurs répartis entre les pôles ingénierie, développement logiciel et support client. Son chiffre d'affaires annuel s'élève à [CA] DH, avec une croissance soutenue par la demande croissante de digitalisation des processus techniques.

### 1.1.2 Activités principales

Les activités se structurent autour de plusieurs axes :

- **Études électriques :** dimensionnement d'installations basse et haute tension, rédaction de notes de calcul avec Caneco BT, coordination des protections ;
- **Ingénierie documentaire :** production et gestion des livrables techniques (plans, schémas, spécifications) ;
- **Développement d'outils :** conception de solutions logicielles pour l'automatisation des tâches d'ingénierie répétitives ;
- **Formation :** accompagnement des équipes client dans la prise en main d'outils métier.

### 1.1.3 Organisation et rattachement du stagiaire

[IMAGE : Organigramme de l'entreprise d'accueil]

Au sein de l'organigramme, le stagiaire a été intégré au **pôle Développement Logiciel**, sous la responsabilité directe de [NOM Maître de stage], [Responsable technique / Lead développeur]. Ce positionnement a permis une immersion complète dans les cycles de développement agile pratiqués par l'équipe, depuis la spécification des besoins jusqu'à la mise en production des livrables.

&nbsp;

## 1.2 Contexte du projet

&nbsp;

### 1.2.1 Le logiciel Caneco BT et ses sorties documentaires

Caneco BT est l'un des logiciels de référence pour le calcul et le dimensionnement des installations électriques basse tension en France, au Maroc et dans les pays francophones. Il permet aux ingénieurs électriciens de saisir les caractéristiques des récepteurs et des circuits, puis d'en calculer automatiquement les sections de câbles, les calibres des protections et les contraintes thermiques selon les normes NF C 15-100 et IEC 60364.

La sortie principale de Caneco BT est une **note de calcul** exportable au format PDF. Cette note se présente sous la forme d'un tableau multi-pages dont chaque ligne représente un circuit, avec des colonnes renseignant des dizaines de paramètres techniques :

- Repère du circuit (identifiant unique)
- Désignation du récepteur
- Puissance installée (kW), courant nominal (IB), courant d'emploi (Iz)
- Section et type du câble, longueur, chute de tension
- Type, calibre et déclencheur de la protection
- Courants de court-circuit maximum et minimum (Ik3max, Ik1min)

Ces paramètres sont indispensables pour les études de coordination des protections, les bilans de puissance et les vérifications de conformité réglementaire. Cependant, leur réutilisation dans d'autres outils (tableurs, ERP, logiciels de simulation) impose aujourd'hui une ressaisie manuelle chronophage.

### 1.2.2 La problématique des plans électriques

En parallèle des notes de calcul, un projet électrique produit des plans techniques - unifilaires, schémas de distribution, plans de masse - qui représentent graphiquement les circuits et équipements à l'aide de symboles normalisés (selon IEC 60617). La quantification de ces symboles - c'est-à-dire le comptage des prises, disjoncteurs, fusibles, transformateurs, etc. - est une étape indispensable pour établir le bordereau de matériel et chiffrer un projet. Effectuée manuellement sur des plans de grande taille, cette tâche est à la fois fastidieuse et risquée (omissions, double-comptage).

### 1.2.3 La gestion des catalogues produits

Un troisième enjeu opérationnel concerne la sélection des produits. Chaque bureau d'études gère un ou plusieurs catalogues de produits (disjoncteurs, câbles, tableaux de distribution) provenant de différents fabricants (Schneider Electric, Legrand, ABB, etc.). Ces catalogues, souvent disponibles sous forme de fichiers Excel ou de PDFs, ne sont pas interconnectés et nécessitent des recherches manuelles répétées pour identifier le bon produit selon les critères techniques (calibre, pouvoir de coupure, nombre de pôles) et budgétaires.

&nbsp;

## 1.3 Problématique et objectifs

&nbsp;

### 1.3.1 Énoncé de la problématique

La convergence de ces trois besoins - extraction de données depuis des notes de calcul PDF, quantification de symboles sur des plans, et interrogation intelligente de catalogues produits - dessine une problématique unifiée :

> **Comment concevoir une plateforme logicielle intelligente capable d'automatiser le traitement des documents techniques en électrotechnique, en intégrant des capacités d'extraction structurée, de vision par ordinateur et d'intelligence artificielle conversationnelle, tout en maintenant la fiabilité et la précision attendues dans un contexte d'ingénierie ?**

### 1.3.2 Sous-problèmes identifiés

Cette problématique centrale se décline en plusieurs sous-problèmes techniques :

**SP1 - Extraction robuste depuis des PDF :** Les tableaux Caneco BT présentent des structures complexes (colonnes fusionnées, cellules multi-lignes, en-têtes composites). Comment les extraire de manière fiable et les normaliser automatiquement ?

**SP2 - Structuration par LLM :** Une fois les tableaux extraits, comment exploiter les grands modèles de langage pour les structurer en objets JSON typés conformes à un schéma métier, tout en gérant les variations de format et les erreurs d'extraction ?

**SP3 - Détection de symboles à grande échelle :** Comment détecter des symboles électriques normalisés sur des plans au format PDF, en gérant les variations d'orientation, d'échelle et les faux positifs ?

**SP4 - Recherche et dialogue sur catalogue :** Comment offrir une interface de recherche en langage naturel sur un catalogue de produits techniques, avec une précision suffisante pour être utilisable en production ?

**SP5 - Cohérence architecturale :** Comment orchestrer ces modules dans une architecture cohérente, maintenable et déployable, tout en assurant performance et sécurité ?

### 1.3.3 Objectifs mesurables

Les objectifs opérationnels fixés en début de stage sont les suivants :

| Objectif | Critère de succès |
|---|---|
| Extraction des circuits Caneco BT | Extraction correcte de ≥ 90% des colonnes sur un jeu de test de 10 notes de calcul |
| Nettoyage automatique | Aucune intervention manuelle nécessaire sur ≥ 85% des tableaux |
| Structuration LLM | Schéma JSON valide produit pour ≥ 95% des requêtes |
| Détection de symboles | Précision ≥ 80% sur les plans de test |
| Agent conversationnel | Réponses pertinentes sur 90% d'un jeu de 50 questions de test |
| Déploiement | Plateforme opérationnelle en environnement Docker en < 5 minutes |

&nbsp;

## 1.4 État de l'art : Traitement Intelligent de Documents

&nbsp;

### 1.4.1 Extraction de tableaux dans les PDF

L'extraction de tableaux depuis des documents PDF est un problème classique mais non trivial en informatique documentaire. On distingue traditionnellement deux classes d'approches.

**Approches basées sur les vecteurs PDF :** Ces méthodes exploitent directement la structure vectorielle du PDF (flux d'objets graphiques et textuels). Des bibliothèques comme **Camelot** [Krupnik, 2019] et **Tabula** [Tabula Project, 2018] s'inscrivent dans cette catégorie. Camelot propose deux algorithmes : *Lattice* (pour les tableaux à bordures explicites) et *Stream* (pour les tableaux à espaces blancs). Tabula, initialement développé en Java, expose une interface Python. Ces approches sont rapides et précises pour les PDF natifs mais échouent sur les documents scannés.

**Approches basées sur l'OCR et la vision :** Pour les documents scannés ou les PDF images, des outils comme **Tesseract OCR** [Smith, 2007], **AWS Textract** ou **Azure Form Recognizer** recourent à la reconnaissance optique de caractères combinée à des modèles de détection de structure. Ces approches sont plus robustes aux variations de format mais plus lentes et parfois moins précises sur les tableaux denses.

**Approches hybrides et par apprentissage profond :** Des travaux récents explorent l'utilisation de réseaux de neurones convolutifs (CNN) ou de transformers pour la détection et la structure des tableaux. **TableNet** [Paliwal et al., 2019], **CascadeTabNet** [Prasad et al., 2020] et **Table Transformer** [Smock et al., 2022] représentent cet axe de recherche. Ces modèles atteignent des performances élevées sur des benchmarks publics (ICDAR 2013, PubTabNet) mais requièrent des ressources computationnelles importantes et des données d'entraînement spécialisées.

**Tableau 1 : Comparatif des bibliothèques d'extraction de tableaux PDF**

| Bibliothèque | Type | PDF natif | PDF scanné | Tableaux complexes | Vitesse |
|---|---|---|---|---|---|
| Camelot Stream | Vectorielle | Oui | Non | Moyen | Rapide |
| Camelot Lattice | Vectorielle | Oui | Non | Bon | Rapide |
| Tabula | Vectorielle | Oui | Non | Moyen | Rapide |
| pdfplumber | Vectorielle | Oui | Non | Moyen | Rapide |
| AWS Textract | Hybride | Oui | Oui | Bon | Lent (API) |
| Table Transformer | Deep Learning | Oui | Oui | Excellent | Variable |

*Choix retenu : **Camelot Stream** pour sa capacité à traiter les tableaux Caneco BT (PDF natif, structure en espaces blancs) sans annotation préalable, et pour sa disponibilité en open source.*

### 1.4.2 Grands modèles de langage pour la structuration documentaire

Les grands modèles de langage (LLM) ont émergé comme des outils puissants pour la compréhension et la transformation de textes semi-structurés. GPT-4 [OpenAI, 2023], Llama 3 [Meta AI, 2024] et Gemini [Google DeepMind, 2023] ont démontré des capacités remarquables en extraction d'informations, génération de JSON structuré et compréhension de domaines techniques spécialisés.

Pour les tâches d'extraction d'information documentaire, plusieurs stratégies sont documentées dans la littérature :

- **Prompting zéro-shot :** Le modèle reçoit directement le texte et un schéma JSON cible. Simple mais sensible aux variations de format.
- **Few-shot prompting :** On fournit des exemples entrée/sortie dans le prompt pour guider le modèle. Plus fiable mais allonge le contexte.
- **Function calling / Structured outputs :** Des APIs comme OpenAI proposent un mode contraint qui garantit une sortie JSON conforme à un schéma. Très fiable mais dépendant du fournisseur.
- **RAG (Retrieval-Augmented Generation) :** Pour les documents longs, on segmente le document en chunks et on utilise une recherche sémantique pour sélectionner les passages pertinents avant de les soumettre au LLM.

**Tableau 2 : Comparatif des fournisseurs LLM intégrés**

| Fournisseur | Modèle(s) | Coût | Structured Output | Latence | Confidentialité |
|---|---|---|---|---|---|
| OpenRouter | Llama 3.3 70B, Gemini 2.0 Flash | Gratuit (free tier) | Non (prompt) | Moyen | Cloud (modéré) |
| HuggingFace Inference | Llama 3.1 70B | Gratuit (limité) | Non | Élevé | Cloud |
| Ollama (local) | Llama 3.2 | Gratuit | Non | Faible (GPU local) | Maximal |

### 1.4.3 Vision par ordinateur pour la détection de symboles

La détection de symboles graphiques sur des plans techniques est un problème de reconnaissance de formes avec contraintes fortes : les plans électriques sont des images haute résolution (souvent A0 ou A1 à 300 DPI), les symboles sont petits, répétitifs et peuvent apparaître en plusieurs orientations.

**Template matching classique :** La méthode la plus simple consiste à corréler un gabarit (template) avec l'image source en faisant glisser le gabarit sur toute l'image (convolution 2D). OpenCV implémente cette technique via la fonction `matchTemplate` avec plusieurs métriques (TM_CCOEFF_NORMED, TM_CCORR_NORMED). Cette approche est efficace pour des symboles stables en taille et orientation, et ne nécessite pas de données d'entraînement.

**Détection par apprentissage (YOLO, Faster R-CNN) :** Des architectures d'objets comme YOLOv8 [Ultralytics, 2023] ou Faster R-CNN [Ren et al., 2015] permettent une détection robuste en toutes orientations et échelles. Cependant, elles requièrent des datasets annotés spécifiques aux plans électriques, qui sont rares et coûteux à constituer.

**Approches hybrides :** Des travaux comme FloorplanCAD [Fan et al., 2021] et GraphCAD combinent segmentation sémantique et reconnaissance de symboles pour les plans architecturaux, avec des résultats prometteurs mais une complexité de mise en œuvre élevée.

**Tableau 3 : Comparatif des approches de détection de symboles**

| Approche | Données requises | Polyvalence | Précision | Complexité |
|---|---|---|---|---|
| Template matching (OpenCV) | Aucune | Faible | Bonne (gabarits fixes) | Faible |
| YOLO / Faster R-CNN | Dataset annoté | Haute | Excellente | Élevée |
| FloorplanCAD | Dataset spécialisé | Moyenne | Très bonne | Très élevée |

*Choix retenu : **Template matching avec OpenCV** pour l'absence de données d'entraînement requises, la maîtrise totale des gabarits et l'adéquation avec les symboles normalisés des plans électriques.*

### 1.4.4 Recherche plein texte et bases de données vectorielles

La recherche dans un catalogue de produits techniques pose deux sous-problèmes : la recherche lexicale (correspondance exacte sur des références, des appellations) et la recherche sémantique (correspondance sur le sens, pour les requêtes en langage naturel).

**Recherche plein texte en base de données :** PostgreSQL offre un moteur de recherche plein texte natif basé sur des vecteurs lexicaux (tsvector) et des index inversés (GIN). Le support de la langue française (tokenisation, suppression des mots vides, lemmatisation) permet une recherche efficace sur des désignations techniques.

**Bases de données vectorielles :** Des extensions comme **pgvector** pour PostgreSQL ou des systèmes dédiés comme **Pinecone**, **Weaviate** ou **Chroma** permettent le stockage et la recherche de vecteurs d'embedding (représentations numériques denses du sens des textes). Cette approche est particulièrement puissante pour la recherche sémantique mais nécessite un modèle d'embedding.

**Approche RAG pour catalogues :** Combiner la recherche plein texte (pour la précision sur les références exactes) et la recherche vectorielle (pour la compréhension sémantique) est une pratique recommandée dans les systèmes de recherche hybride modernes [Lewis et al., 2020].

&nbsp;

## 1.5 Revue des Technologies Pertinentes

&nbsp;

### 1.5.1 FastAPI et l'architecture asynchrone Python

FastAPI [Ramirez, 2018] est un framework Python moderne pour la construction d'API REST, basé sur les standards OpenAPI et JSON Schema. Ses caractéristiques principales - typage statique via Pydantic, génération automatique de documentation Swagger, support natif de l'asynchronisme (async/await) - en font un choix de référence pour les APIs à haute concurrence. Dans DIGICONSTRUCT, l'aspect asynchrone est critique : le traitement d'un PDF (extraction, LLM, écriture en base) peut durer plusieurs dizaines de secondes, et l'API doit rester disponible pour d'autres requêtes simultanées.

### 1.5.2 React et l'écosystème frontend moderne

React [Facebook, 2013] est une bibliothèque JavaScript pour la construction d'interfaces utilisateur déclaratives et composables. Associé à **Vite** [Evans, 2020] comme outil de build (bundler ESM ultra-rapide), **TailwindCSS** pour le stylisme utilitaire, et **Framer Motion** pour les animations, il constitue un écosystème frontend productif et performant. La navigation est gérée par React Router v7, qui supporte le lazy loading des modules (code splitting) pour des temps de chargement optimisés.

### 1.5.3 PostgreSQL et l'extension pgvector

PostgreSQL est un système de gestion de bases de données relationnelles open source reconnu pour sa fiabilité, ses capacités transactionnelles (ACID) et ses extensions. Dans DIGICONSTRUCT, deux fonctionnalités avancées sont exploitées : le type **tsvector** avec index **GIN** pour la recherche plein texte en langue française, et l'extension **pgvector** pour le stockage futur d'embeddings sémantiques. SQLModel (surcouche de SQLAlchemy v2 avec Pydantic) assure la correspondance objet-relationnel de manière type-safe.

### 1.5.4 Docker et la conteneurisation

Docker permet d'encapsuler chaque composant de l'application (backend, frontend, base de données) dans des conteneurs isolés avec leurs dépendances. Docker Compose orchestre ces conteneurs, définit leurs réseaux et leurs volumes, et simplifie le déploiement aussi bien en développement qu'en production. Cette approche garantit la reproductibilité des environnements et facilite l'intégration continue.

&nbsp;

## 1.6 Synthèse et Positionnement

&nbsp;

L'analyse de l'existant révèle que si des outils spécialisés existent pour chacun des besoins identifiés - extraction PDF, détection d'objets, catalogues produits - **aucune solution unifiée et adaptée au domaine de l'électrotechnique** n'est disponible en open source ou sur le marché marocain à un coût accessible pour les PME et bureaux d'études de taille moyenne.

DIGICONSTRUCT se positionne donc comme une **plateforme intégrée** qui connecte ces briques technologiques dans un pipeline cohérent, avec une interface utilisateur pensée pour les ingénieurs électriciens et non pour des data scientists. Le choix délibéré de technologies open source (Camelot, OpenCV, LLMs libres via Ollama) garantit l'indépendance vis-à-vis des fournisseurs cloud, tout en maintenant une porte ouverte sur des services commerciaux (OpenRouter, HuggingFace) pour les performances maximales.

&nbsp;

---

&nbsp;

---

# Chapitre 2 - Analyse, Conception et Architecture du Système

&nbsp;

> *Ce chapitre détaille la démarche de conception adoptée pour DIGICONSTRUCT. Il couvre l'analyse des besoins, les choix architecturaux structurants et la modélisation des données, en s'appuyant sur les enseignements tirés de l'état de l'art.*

&nbsp;

## 2.1 Analyse des Besoins

&nbsp;

### 2.1.1 Identification des acteurs

La plateforme DIGICONSTRUCT est destinée à deux profils d'utilisateurs principaux :

- **L'ingénieur électricien :** utilisateur principal, il charge des PDFs (notes de calcul ou plans), déclenche les traitements, consulte et exporte les résultats. Il dispose d'une expertise métier mais pas nécessairement informatique.
- **L'administrateur système :** il gère les utilisateurs, configure les sources de données (import de catalogues), surveille les jobs en cours et gère les ressources serveur.

### 2.1.2 Cas d'utilisation

**Tableau 4 : Cas d'utilisation principaux et acteurs**

| ID | Cas d'utilisation | Acteur | Priorité |
|---|---|---|---|
| UC01 | S'authentifier à la plateforme | Ingénieur, Admin | Critique |
| UC02 | Importer un PDF de note de calcul | Ingénieur | Critique |
| UC03 | Lancer l'extraction des circuits | Ingénieur | Critique |
| UC04 | Consulter et corriger les circuits extraits | Ingénieur | Haute |
| UC05 | Exporter les résultats au format Excel | Ingénieur | Haute |
| UC06 | Importer un plan électrique (PDF) | Ingénieur | Critique |
| UC07 | Lancer la détection de symboles | Ingénieur | Critique |
| UC08 | Modifier manuellement les détections | Ingénieur | Haute |
| UC09 | Rechercher un produit dans le catalogue | Ingénieur | Haute |
| UC10 | Interroger l'agent IA en langage naturel | Ingénieur | Moyenne |
| UC11 | Importer un catalogue depuis Excel | Admin | Haute |
| UC12 | Gérer les utilisateurs | Admin | Haute |

[IMAGE : Diagramme de cas d'utilisation UML principal]

### 2.1.3 Besoins non fonctionnels

Au-delà des fonctionnalités, les exigences non fonctionnelles suivantes ont guidé les choix de conception :

- **Performance :** Un PDF de 50 pages doit être traité en moins de 3 minutes en mode extraction complète (Camelot + LLM).
- **Résilience :** La plateforme doit rester disponible même si un fournisseur LLM externe est indisponible (basculement automatique vers Ollama local).
- **Sécurité :** Toutes les routes métier sont protégées par authentification JWT. Les mots de passe sont hashés (bcrypt). Les uploads sont validés (type MIME, taille maximale).
- **Maintenabilité :** L'architecture modulaire (trois packages Python indépendants) permet d'évoluer chaque module sans affecter les autres.
- **Déployabilité :** Le système doit démarrer en une seule commande (`docker-compose up`) dans tout environnement Linux ou macOS.

&nbsp;

## 2.2 Architecture Globale de la Plateforme

&nbsp;

### 2.2.1 Vue d'ensemble

[IMAGE : Schéma d'architecture générale de DIGICONSTRUCT (couches frontend, API gateway, modules backend, base de données, services LLM)]

L'architecture de DIGICONSTRUCT suit un pattern **monorepo modulaire** : tous les composants résident dans un même dépôt git, mais sont organisés en modules clairement délimités avec des responsabilités distinctes. Cette approche offre le meilleur équilibre entre la cohérence du développement (dépendances communes, CI unifiée) et la séparation des préoccupations.

On distingue quatre couches :

1. **Couche présentation (Frontend React)** : SPA React/Vite servie par Nginx en production, communiquant exclusivement via API REST/JSON avec le backend.
2. **Couche API (FastAPI gateway)** : Point d'entrée unique exposant les routes `/api/v1/*` pour les modules métier, avec middleware d'authentification JWT transversal.
3. **Couche métier (Modules Python)** : Trois modules indépendants - `backend_extract`, `backend_quant`, `backend_base` - montés sur le routeur FastAPI principal.
4. **Couche données (PostgreSQL + Fichiers statiques)** : Base de données PostgreSQL pour la persistance relationnelle, volume Docker pour les fichiers uploadés et les images générées.

### 2.2.2 Organisation du backend

La structure du backend illustre la séparation des préoccupations :

```
backend/
├── main.py                    # Point d'entrée FastAPI, montage des routers
├── backend_extract/           # Module extraction PDF
│   ├── app/
│   │   ├── api/routes/        # Routes HTTP
│   │   ├── services/          # Logique métier (Camelot, Cleaner, LLM)
│   │   └── models/            # Schémas Pydantic / SQLModel
│   └── requirements.txt
├── backend_quant/             # Module quantification symboles
│   ├── app/
│   │   ├── api/routes/
│   │   ├── services/          # Detection, NMS, Job tracking
│   │   └── models/
│   └── requirements.txt
└── backend_base/              # Module catalogue & agent IA
    ├── app/
    │   ├── api/routes/
    │   ├── services/          # Search, ETL, Chat Agent
    │   └── models/
    ├── configs/               # Mappings YAML pour import Excel
    └── requirements.txt
```

Le fichier `main.py` importe les trois routers et les monte sur des préfixes distincts, garantissant l'isolation des namespaces et facilitant le routage :

```python
# Montage des modules sur le router principal
app.include_router(extract_router, prefix="/api/v1", tags=["Extract"])
app.include_router(quant_router, prefix="", tags=["Quant"])  
app.include_router(base_router, prefix="", tags=["Base Electrique"])
app.include_router(auth_router, prefix="/api/v1/auth", tags=["Auth"])
```

### 2.2.3 Flux de données principal

[IMAGE : Diagramme de flux de données de bout en bout (upload PDF → extraction → LLM → export)]

Le flux principal d'utilisation pour l'extraction se déroule ainsi :

1. L'utilisateur authentifié dépose un PDF via l'interface web.
2. Le frontend envoie le fichier en multipart/form-data à `POST /api/v1/upload`.
3. Le backend calcule le hash SHA-256 du fichier (déduplication), le stocke sur le disque et en base de données.
4. L'utilisateur déclenche l'extraction : `POST /api/v1/extract/stream/start` crée un `ExtractionJob` en état `pending` et retourne son UUID.
5. Un worker asynchrone (coroutine background FastAPI) exécute le pipeline ETL : Camelot → TableCleaner → LLMStructurer → base de données.
6. Le frontend poll l'état du job via `GET /api/v1/extract/stream/status?job_id=...` jusqu'à completion.
7. L'utilisateur consulte les résultats et peut les exporter au format Excel.

&nbsp;

## 2.3 Conception du Module d'Extraction

&nbsp;

### 2.3.1 Le pipeline ETL d'extraction

Le module d'extraction est conçu selon le pattern **ETL (Extract → Transform → Load)**, adapté aux spécificités des notes de calcul Caneco BT. Chaque étape est encapsulée dans une classe de service indépendante, favorisant la testabilité et la substitution.

[IMAGE : Diagramme de séquence du pipeline ETL d'extraction]

**Étape 1 - Extract (CamelotStreamExtractor) :**
L'extracteur utilise Camelot en mode Stream (basé sur l'analyse des espaces blancs entre les cellules) plutôt que Lattice (basé sur les bordures) car les notes Caneco BT ne possèdent pas systématiquement de lignes de bordure. Les paramètres clés sont configurables :
- `edge_tol` : tolérance de détection des bords de colonnes
- `row_tol` : tolérance de regroupement de lignes
- `column_tol` : tolérance de détection des colonnes
Une métrique de qualité (taux de remplissage, nombre de cellules non vides, score de confiance) est calculée pour chaque tableau extrait.

**Étape 2 - Transform (TableCleaner) :**
Le nettoyage suit une séquence déterministe de transformations basées sur les règles métier documentées. Voir section 2.3.2 pour le détail.

**Étape 3 - Structure (LLMStructurer) :**
Le tableau nettoyé est converti en texte tabulaire compact (séparateurs `|`) et soumis à un LLM avec un prompt spécialisé Caneco BT. Le LLM retourne un objet JSON structuré conforme au schéma `NoteCalcul`.

**Étape 4 - Load :**
Le résultat structuré est persisté dans la table `ExtractionResult` au format JSONB. L'état du job passe à `completed` ou `failed` selon le résultat.

### 2.3.2 Règles métier du nettoyage

Le nettoyage des tableaux est l'étape la plus délicate : les tableaux extraits par Camelot présentent des artefacts liés à la structure PDF de Caneco BT.

**Tableau 6 : Règles métier du nettoyage des tableaux (TableCleaner)**

| # | Règle | Description | Exemple |
|---|---|---|---|
| R1 | Isoler le tableau circuits | Garder uniquement les lignes entre le marqueur `CIRCUIT` et `AFFECTATION DES PHASES` | Suppression des en-têtes de projet |
| R2 | Supprimer les colonnes vides | Colonnes avec taux de remplissage < 20% sont supprimées | Colonnes fantômes liées à la structure PDF |
| R3 | Développer les cellules fusionnées | Cellules contenant `\n` sont éclatées en lignes séparées | `"TD-AT\nP01"` → deux lignes |
| R4 | Scinder les colonnes composites | 14 patterns de colonnes composites détectés et séparés | `"TypeDéclencheur"` → `"Type Protection"` + `"Déclencheur"` |
| R5 | Normaliser les espaces | Suppression des espaces multiples, retours à la ligne résiduels | `"câble  3×2.5"` → `"câble 3×2.5"` |
| R6 | Supprimer les lignes vides | Lignes entièrement nulles ou ne contenant que des espaces | Lignes séparatrices visuelles |
| R7 | Marquer les tableaux dégradés | Si score confiance < seuil, flag `needs_llm_review` | Tableaux Caneco en version ancienne |

### 2.3.3 Schéma de données de sortie : NoteCalcul

Le schéma cible de structuration est défini comme un modèle Pydantic rigoureux, qui sert à la fois de documentation du domaine et de validation de sortie :

```python
class Circuit(BaseModel):
    repere: str                    # Identifiant du circuit (ex: "P01")
    designation: str               # Désignation du récepteur
    nb: Optional[int]              # Nombre d'appareils
    puissance_kw: Optional[float]  # Puissance installée (kW)
    ib: Optional[float]            # Courant d'emploi (A)
    iz: Optional[float]            # Courant admissible câble (A)
    section_cable: Optional[str]   # Section câble (ex: "3G2.5")
    longueur_cable: Optional[float]# Longueur (m)
    type_protection: Optional[str] # Type (disjoncteur, fusible...)
    calibre: Optional[float]       # Calibre de la protection (A)
    declencheur: Optional[str]     # Type déclencheur (C, D, MA...)
    ik3max: Optional[float]        # Icc max (kA)
    ik1min: Optional[float]        # Icc min (kA)
    chute_tension: Optional[float] # Chute de tension (%)

class NoteCalcul(BaseModel):
    reseau_regime: Optional[str]   # Régime de neutre (TN-S, TT...)
    tension: Optional[int]         # Tension (V)
    circuits: List[Circuit]        # Liste des circuits
```

&nbsp;

## 2.4 Conception du Module de Quantification

&nbsp;

### 2.4.1 Principe de détection par template matching

[IMAGE : Schéma explicatif du template matching avec corrélation normalisée]

Le module de quantification repose sur la technique du **template matching normalisé** (`cv2.TM_CCOEFF_NORMED`). Pour chaque symbole à détecter, un gabarit (image de référence du symbole) est fourni. L'algorithme fait glisser ce gabarit sur l'image du plan et calcule un score de corrélation en chaque position. Les positions dont le score dépasse un seuil configurable (par défaut 0,8) sont considérées comme des détections candidates.

Pour gérer les différentes orientations des symboles électriques (un disjoncteur peut apparaître vertical ou horizontal sur un plan), le gabarit est appliqué en quatre rotations : 0°, 90°, 180° et 270°. Les détections toutes orientations confondues sont ensuite fusionnées.

### 2.4.2 Non-Maximum Suppression (NMS)

Un problème classique du template matching est la **détection multiple** : pour un symbole présent une seule fois, plusieurs positions proches peuvent dépasser le seuil de confiance, générant des faux positifs. La **suppression des non-maxima (NMS)** résout ce problème :

1. Trier les détections par score de confiance décroissant.
2. Pour chaque détection, supprimer toutes les détections suivantes dont la boîte englobante (*bounding box*) présente un chevauchement (IoU - Intersection over Union) supérieur à un seuil (généralement 0,3).
3. Conserver uniquement les détections survivantes.

Cette étape est implémentée nativement sans dépendance à des frameworks lourds (TensorFlow, PyTorch), en Python pur avec NumPy.

### 2.4.3 Gestion des jobs de quantification

Comme pour l'extraction, la détection sur de grands PDFs (plans A0 à 300 DPI) peut durer plusieurs minutes. Le pattern **job asynchrone** est donc appliqué :

- `POST /detect-batch` crée un `QuantJob` et retourne son ID.
- Un worker background itère sur chaque page (conversion PDF → image via PyMuPDF, puis template matching).
- Les résultats sont persistés page par page dans le JSONB `results_by_page`.
- L'état du job est consultable via polling.

L'ingénieur peut ensuite **modifier manuellement** les détections (ajout/suppression de détections incorrectes) via l'interface, et ces corrections sont persistées dans `QuantDetectionState` pour garantir leur traçabilité.

&nbsp;

## 2.5 Conception du Module Catalogue et Agent IA

&nbsp;

### 2.5.1 Import et normalisation du catalogue

Le catalogue de produits est alimenté via un pipeline d'import depuis des fichiers Excel fournis par les fabricants. Un fichier de configuration YAML par fabricant (ex: `schneider.yaml`) définit la correspondance entre les colonnes du fichier Excel source et les champs de la table `products` :

```yaml
# configs/schneider_test/schema.yaml (exemple simplifié)
sheet_name: "Schneider"
column_mapping:
  manufacturer: "Fabricant"
  family: "Gamme"
  reference: "Référence"
  designation: "Désignation"
  current_rating: "Calibre (A)"
  breaking_capacity: "PdC (kA)"
  price: "Prix HT (DH)"
```

Cette architecture YAML-driven permet d'ajouter un nouveau fabricant sans modifier le code - seul un nouveau fichier de configuration suffit.

### 2.5.2 Recherche plein texte avec tsvector

La recherche sur les désignations de produits exploite le moteur plein texte natif de PostgreSQL. Un trigger SQL est créé à l'insertion/mise à jour pour maintenir automatiquement le champ `search_vector` :

```sql
-- Trigger de mise à jour automatique du vecteur de recherche
CREATE OR REPLACE FUNCTION update_search_vector()
RETURNS TRIGGER AS $$
BEGIN
  NEW.search_vector = to_tsvector('french', 
    COALESCE(NEW.designation, '') || ' ' ||
    COALESCE(NEW.family, '') || ' ' ||
    COALESCE(NEW.manufacturer, '')
  );
  RETURN NEW;
END;
$$ LANGUAGE plpgsql;
```

Un index GIN sur `search_vector` permet des recherches en O(log n) même sur des catalogues de plusieurs dizaines de milliers de produits.

### 2.5.3 Architecture de l'agent conversationnel

[IMAGE : Diagramme de séquence de l'agent conversationnel (multi-turn avec function calling)]

L'agent conversationnel suit l'architecture **ReAct** (Reasoning + Acting) adaptée à un domaine contraint : le modèle peut raisonner en langage naturel et appeler des outils prédéfinis pour interagir avec la base de données, sans être autorisé à générer des requêtes SQL arbitraires.

Les outils exposés à l'agent sont définis dans `tools.py` :

| Outil | Description | Paramètres clés |
|---|---|---|
| `recherche_produits` | Recherche plein texte dans le catalogue | `query`, `manufacturer`, `family`, `price_max` |
| `get_families` | Liste les familles de produits | `manufacturer` |
| `get_manufacturers` | Liste tous les fabricants | - |
| `get_stats` | Statistiques globales du catalogue | - |
| `count_products` | Nombre de produits selon critères | `manufacturer`, `family` |
| `compare_products` | Compare deux produits par référence | `ref1`, `ref2` |

Le cycle d'exécution de l'agent est le suivant :

1. L'utilisateur envoie un message : `"Trouve-moi un disjoncteur Schneider de 63A courbe C"`
2. Le message est soumis au LLM avec le contexte de conversation et les définitions des outils.
3. Le LLM répond en indiquant qu'il souhaite appeler `recherche_produits(query="disjoncteur 63A", manufacturer="Schneider", curve="C")`.
4. Le backend exécute l'outil et retourne les résultats (JSON).
5. Les résultats sont re-soumis au LLM qui formule la réponse finale en langage naturel.
6. Le processus peut se répéter (multi-tour) si le LLM a besoin d'informations supplémentaires.

### 2.5.4 Fallback multi-fournisseurs LLM

[IMAGE : Diagramme du mécanisme de fallback LLM (OpenRouter → HuggingFace → Ollama)]

La fiabilité de l'agent repose sur un mécanisme de **chaîne de responsabilité** pour les fournisseurs LLM :

```python
LLM_PROVIDER_ORDER = ["openrouter", "huggingface", "ollama"]
```

En cas d'erreur (timeout, limite de débit, erreur API), le système bascule automatiquement vers le fournisseur suivant dans la chaîne. Ollama, déployé localement, constitue le filet de sécurité ultime - toujours disponible, sans dépendance réseau externe.

&nbsp;

## 2.6 Modèle de Données

&nbsp;

### 2.6.1 Schéma relationnel

[IMAGE : Diagramme entité-relation complet de la base de données DIGICONSTRUCT]

Le modèle de données est organisé en trois schémas logiques correspondant aux trois modules fonctionnels :

**Schéma extraction :**

```
File (id PK, filename, file_hash UNIQUE, file_path, file_size, metadata_info JSONB, created_at)
  └── ExtractionJob (id PK, file_id FK, status, provider, model_name, error_message, created_at, updated_at)
        └── ExtractionResult (id PK, job_id FK, file_id FK, data JSONB, created_at)
```

**Schéma quantification :**

```
QuantFile (id PK, original_filename, stored_filename UNIQUE, file_path, file_size, page_count, file_hash, created_at)
  ├── QuantJob (id PK, quant_file_id FK, mode, label, threshold, status, results_by_page JSONB, created_at, updated_at)
  └── QuantDetectionState (id PK, quant_file_id FK UNIQUE, detections_by_page JSONB, updated_at)
```

**Schéma authentification :**

```
User (id PK, email UNIQUE, full_name, hashed_password, is_active, created_at, updated_at)
  └── PasswordResetToken (id PK, user_id FK, token_hash UNIQUE, expires_at, created_at, used_at)
```

**Schéma catalogue (schéma PostgreSQL `base_electrique`) :**

```
products (id SERIAL PK, manufacturer, family, reference TEXT,
          designation, type, curve, poles,
          current_rating NUMERIC, breaking_capacity NUMERIC, price NUMERIC,
          technical_data JSONB, source_sheet TEXT,
          imported_at TIMESTAMP,
          search_vector TSVECTOR,  -- GIN index
          UNIQUE(manufacturer, reference))
```

### 2.6.2 Choix de conception du modèle de données

Plusieurs décisions méritent d'être explicitées :

- **JSONB pour les données variables :** Les résultats d'extraction (`ExtractionResult.data`) et les détections (`QuantJob.results_by_page`) sont stockés en JSONB, qui offre un indexage et des opérateurs de requête JSON natifs dans PostgreSQL. Cette approche évite de devoir prédéfinir un schéma rigide pour des données dont la structure peut varier selon les versions de Caneco BT.

- **UUID comme clé primaire :** L'utilisation d'UUID v4 (au lieu d'entiers auto-incrémentés) pour toutes les entités principales évite les collisions lors d'opérations de synchronisation et garantit l'unicité globale, ce qui facilite les migrations de données.

- **file_hash pour la déduplication :** Le champ `file_hash` (SHA-256) permet de détecter et refuser l'upload de fichiers identiques, évitant les traitements redondants et le gaspillage de ressources.

- **Schema séparé `base_electrique` :** Le catalogue de produits est isolé dans un schéma PostgreSQL dédié, ce qui simplifie la gestion des droits et permet de recréer le catalogue sans toucher aux tables d'extraction ou d'authentification.

&nbsp;

## 2.7 Sécurité et Gestion des Accès

&nbsp;

### 2.7.1 Authentification JWT

L'authentification repose sur des **JSON Web Tokens (JWT)** signés avec l'algorithme HS256. À la connexion, le serveur émet un token contenant l'ID et l'email de l'utilisateur, signé avec une clé secrète configurable. Ce token, transmis dans l'en-tête HTTP `Authorization: Bearer <token>`, est vérifié à chaque requête protégée.

Les paramètres de sécurité configurables incluent :
- `ACCESS_TOKEN_EXPIRE_MINUTES` : durée de validité du token (défaut : 60 min)
- `RESET_TOKEN_EXPIRE_MINUTES` : durée de validité du token de réinitialisation de mot de passe
- `AUTH_SECRET_KEY` : clé secrète de signature (doit être générée aléatoirement en production)

### 2.7.2 Hachage des mots de passe

Les mots de passe ne sont jamais stockés en clair. La bibliothèque **passlib** avec l'algorithme **bcrypt** (facteur de travail configurable) est utilisée pour le hachage et la vérification.

### 2.7.3 Validation des uploads

Les fichiers uploadés sont soumis à une validation multicouche :
- Vérification du type MIME (seuls les PDF sont acceptés)
- Limitation de la taille maximale (configurable)
- Génération d'un nom de fichier stocké unique (UUID) pour éviter les conflits et les injections de chemin

&nbsp;

---

&nbsp;

---

# Chapitre 3 - Implémentation, Tests et Résultats

&nbsp;

> *Ce troisième chapitre entre dans le détail de l'implémentation. Il présente les choix techniques concrets effectués lors du développement, les difficultés rencontrées et les solutions apportées, puis évalue les performances de chaque module.*

&nbsp;

## 3.1 Environnement de Développement et Stack Technique

&nbsp;

### 3.1.1 Environnement local

Le développement a été conduit sous Linux (Fedora), avec les outils suivants :

- **Python 3.11** avec gestion des dépendances via `requirements.txt` par module
- **Node.js 20 LTS** pour le frontend
- **PostgreSQL 16** en local (via Docker) avec l'extension pgvector
- **Docker Desktop** et Docker Compose v2 pour l'orchestration
- **Visual Studio Code** avec les extensions Python, ESLint, Prettier et Docker

Le dépôt est organisé comme un monorepo avec la structure suivante au niveau racine :

```
DIGICONSTRUCT/
├── digiconstruct/
│   ├── backend/
│   │   ├── main.py
│   │   ├── backend_extract/
│   │   ├── backend_quant/
│   │   └── backend_base/
│   └── frontend/
│       └── gateway/          # Application React/Vite
├── docker-compose.yml        # Environnement de développement
├── docker-compose.prod.yml   # Environnement de production
└── .env.example              # Template de configuration
```

### 3.1.2 Gestion des variables d'environnement

Toute la configuration sensible (clés API, URL de base de données, secret JWT) est externalisée dans un fichier `.env` non versionné. Un fichier `.env.example` documenté est fourni pour guider la mise en place :

```ini
# LLM Configuration
LLM_PROVIDER_ORDER=openrouter,huggingface,ollama
OPENROUTER_API_KEY=sk-or-...
OPENROUTER_MODEL=meta-llama/llama-3.3-70b-instruct:free

# Database
DATABASE_URL=postgresql+asyncpg://user:pass@localhost:5432/digiconstruct

# Auth
AUTH_SECRET_KEY=<GÉNÉRER_ALÉATOIREMENT>
ACCESS_TOKEN_EXPIRE_MINUTES=60

# PDF Processing
PDF_DPI=300
```

&nbsp;

## 3.2 Implémentation du Module d'Extraction

&nbsp;

### 3.2.1 L'extracteur Camelot (CamelotStreamExtractor)

L'extracteur est implémenté comme une classe de service synchrone (Camelot ne supporte pas nativement asyncio) appelée dans un executor pour ne pas bloquer le serveur FastAPI :

```python
class CamelotStreamExtractor:
    def __init__(self, edge_tol: int = 50, row_tol: int = 2, column_tol: int = 0):
        self.edge_tol = edge_tol
        self.row_tol = row_tol
        self.column_tol = column_tol
    
    def extract_file(self, file_path: str) -> List[RawTable]:
        tables = camelot.read_pdf(
            file_path,
            flavor="stream",
            pages="all",
            edge_tol=self.edge_tol,
            row_tol=self.row_tol,
            column_tol=self.column_tol
        )
        return [self._to_raw_table(t, i) for i, t in enumerate(tables)]
    
    def _to_raw_table(self, table, index: int) -> RawTable:
        df = table.df
        fill_rate = (df != "").sum().sum() / df.size if df.size > 0 else 0.0
        return RawTable(
            page=table.page,
            table_index=index,
            data=df.values.tolist(),
            columns=df.columns.tolist(),
            fill_rate=fill_rate,
            accuracy=table.accuracy,
            whitespace=table.whitespace,
        )
```

Un point important : Camelot requiert **Ghostscript** pour la conversion des PDF. Dans l'environnement Docker, Ghostscript est installé dans le `Dockerfile` via `apt-get install ghostscript`. Hors Docker, cette dépendance doit être installée manuellement - un point qui a causé des frictions lors des premières sessions de test sur Windows.

### 3.2.2 Le nettoyeur de tableaux (TableCleaner)

Le nettoyeur implémente les règles métier documentées en section 2.3.2. La règle la plus complexe est la **détection des colonnes composites** de Caneco BT. En effet, certaines versions du logiciel exportent deux types d'informations dans une seule colonne, séparés par un saut de ligne dans la cellule en-tête. Le nettoyeur maintient un dictionnaire de 14 patterns connus :

```python
COMPOSITE_COLUMN_PATTERNS = {
    "TypeDéclencheur": ("Type Protection", "Déclencheur"),
    "NbConsommation": ("Nb", "Consommation (kW)"),
    "IbIz": ("IB (A)", "IZ (A)"),
    "CalibreTempo": ("Calibre (A)", "Tempo (ms)"),
    # ... 10 autres patterns
}
```

Pour chaque colonne de l'en-tête, si le texte correspond à un pattern composite, la colonne est scindée en deux colonnes distinctes et les données cellulaires sont également splitées selon le séparateur `\n`. Cette logique, bien que simple en apparence, a nécessité plusieurs itérations de calibration sur des notes de calcul réelles pour couvrir l'ensemble des variantes de format produites par les différentes versions de Caneco BT.

### 3.2.3 La structuration par LLM (LLMStructurer)

[IMAGE : Exemple d'échange prompt/réponse LLM pour la structuration Caneco BT]

La structuration par LLM est l'étape la plus fragile du pipeline car elle dépend d'un service externe et d'une opération non déterministe. Plusieurs techniques de robustesse ont été mises en place :

**Formatage compact du prompt :**
Le tableau nettoyé est condensé en une représentation textuelle séparée par `|` pour minimiser la longueur du contexte envoyé au LLM :

```
Repère | Désignation | Nb | P(kW) | IB | IZ | Section | Long. | Protection | Calibre
P01    | Éclairage bureau | 1 | 0.5 | 2.27 | 14.5 | 3G2.5 | 25m | C60N C | 10A
P02    | Prises RDC | 6 | 3.0 | 13.6 | 20.0 | 3G4   | 30m | C60N C | 20A
```

**Prompt system spécialisé :**
Le prompt système instruit le modèle sur les spécificités de Caneco BT : unités des colonnes, valeurs possibles pour les types de protection, format des déclencheurs, etc. Il stipule également que les valeurs manquantes doivent être `null` et non des chaînes vides, et que la réponse doit être un JSON pur (sans markdown).

**Parsing robuste de la réponse :**
Le LLM peut parfois encadrer le JSON dans des balises markdown (` ```json ... ``` `). Un parser de fallback extrait le JSON en utilisant des expressions régulières avant de tenter `json.loads()`.

**Fallback textuel pour Ollama :**
Les petits modèles (Llama 3.2 7B en local) ne supportent pas le function calling structuré. Un parser de fallback basé sur des expressions régulières détecte les appels d'outils exprimés en langage naturel par le modèle, permettant à l'agent de fonctionner même avec Ollama.

### 3.2.4 Gestion des jobs asynchrones

Le pattern de gestion des jobs asynchrones mérite une attention particulière. FastAPI permet d'exécuter des tâches de fond via `BackgroundTasks` ou des coroutines `asyncio`. Le choix retenu est la **tâche de fond FastAPI** pour sa simplicité, au prix d'une limitation : si le serveur redémarre, les jobs en cours sont perdus. Pour un MVP, ce compromis est acceptable ; une évolution vers une file de messages dédiée (Redis/Celery ou Dramatiq) est envisagée pour la version 2.

```python
@router.post("/extract/stream/start")
async def start_extraction(
    file_id: UUID,
    background_tasks: BackgroundTasks,
    db: AsyncSession = Depends(get_db),
    current_user: User = Depends(get_current_user)
):
    job = await create_extraction_job(db, file_id)
    background_tasks.add_task(run_extraction_pipeline, job.id, file_id, db)
    return {"job_id": str(job.id), "status": "pending"}
```

&nbsp;

## 3.3 Implémentation du Module de Quantification

&nbsp;

### 3.3.1 Conversion PDF vers images

La première étape du module consiste à convertir les pages PDF en images PNG haute résolution. **PyMuPDF** (alias `fitz`) est utilisé pour cette opération, avec un DPI configurable (300 par défaut) :

```python
def pdf_page_to_image(pdf_path: str, page_num: int, dpi: int = 300) -> np.ndarray:
    doc = fitz.open(pdf_path)
    page = doc[page_num]
    mat = fitz.Matrix(dpi / 72, dpi / 72)  # Facteur de zoom = DPI / résolution native
    pix = page.get_pixmap(matrix=mat, colorspace=fitz.csGRAY)
    img_array = np.frombuffer(pix.samples, dtype=np.uint8)
    return img_array.reshape(pix.h, pix.w)
```

La conversion en niveaux de gris (espace colorimétrique `csGRAY`) réduit la taille des images de 66% et accélère le template matching sans impacter la qualité de détection des symboles vectoriels noirs sur fond blanc.

### 3.3.2 Détection et NMS

Le cœur du module de quantification est la fonction de détection avec NMS :

```python
def detect_symbol(
    image: np.ndarray,
    template: np.ndarray,
    threshold: float = 0.80,
    rotations: List[int] = [0, 90, 180, 270]
) -> List[Detection]:
    all_detections = []
    
    for angle in rotations:
        rotated_template = rotate_image(template, angle)
        result = cv2.matchTemplate(image, rotated_template, cv2.TM_CCOEFF_NORMED)
        locations = np.where(result >= threshold)
        
        h, w = rotated_template.shape
        for pt in zip(*locations[::-1]):  # (x, y)
            all_detections.append(Detection(
                x=pt[0], y=pt[1], w=w, h=h,
                score=float(result[pt[1], pt[0]]),
                rotation=angle
            ))
    
    return apply_nms(all_detections, iou_threshold=0.3)
```

[IMAGE : Comparaison détections avant/après NMS sur un extrait de plan électrique]

La fonction `apply_nms` implémente la suppression des non-maxima sans dépendance externe :

```python
def apply_nms(detections: List[Detection], iou_threshold: float) -> List[Detection]:
    if not detections:
        return []
    
    # Trier par score décroissant
    detections = sorted(detections, key=lambda d: d.score, reverse=True)
    kept = []
    
    while detections:
        best = detections.pop(0)
        kept.append(best)
        detections = [
            d for d in detections
            if compute_iou(best, d) < iou_threshold
        ]
    
    return kept
```

### 3.3.3 État des détections et modifications manuelles

Un ingénieur peut constater des faux positifs (symbole détecté à tort) ou des faux négatifs (symbole manqué) dans les résultats automatiques. L'interface permet d'ajouter, déplacer ou supprimer des détections manuellement. Ces modifications sont persistées dans `QuantDetectionState` et sont dissociées des résultats du job original, ce qui permet de conserver la traçabilité de l'état automatique versus l'état corrigé par l'utilisateur.

&nbsp;

## 3.4 Implémentation du Module Catalogue et Agent Conversationnel

&nbsp;

### 3.4.1 Pipeline d'import ETL du catalogue

L'import d'un catalogue depuis Excel est orchestré par un endpoint dédié :

```
POST /api/v1/import/excel
  → Lecture du fichier Excel avec pandas
  → Sélection de la feuille selon schema.yaml
  → Mapping des colonnes selon column_mapping
  → Normalisation des données (prix, calibres, références)
  → Upsert en base (INSERT ... ON CONFLICT DO UPDATE)
  → Mise à jour automatique du search_vector via trigger
```

La normalisation des données est une étape critique : les fichiers Excel des fabricants présentent des formats très hétérogènes. Par exemple, le prix peut être renseigné comme `"1 234,50 DH"`, `"1234.5"` ou `"1234,5 €"`. Un parser de prix robuste gère ces variations :

```python
def parse_price(value: Any) -> Optional[float]:
    if value is None or (isinstance(value, float) and math.isnan(value)):
        return None
    text = str(value).strip()
    # Supprimer les symboles monétaires et espaces insécables
    text = re.sub(r'[^\d,.\-]', '', text.replace('\xa0', ''))
    # Normaliser la virgule décimale
    text = text.replace(',', '.')
    try:
        return float(text)
    except ValueError:
        return None
```

### 3.4.2 La recherche plein texte

La recherche plein texte exploite le moteur PostgreSQL via SQLAlchemy :

```python
async def search_products(db: AsyncSession, query: str, **filters) -> List[Product]:
    # Construire le vecteur de recherche de la requête
    search_query = func.plainto_tsquery("french", query)
    
    stmt = (
        select(Product)
        .where(Product.search_vector.op("@@")(search_query))
        .order_by(func.ts_rank(Product.search_vector, search_query).desc())
    )
    
    # Appliquer les filtres optionnels
    if filters.get("manufacturer"):
        stmt = stmt.where(Product.manufacturer.ilike(f"%{filters['manufacturer']}%"))
    if filters.get("price_max"):
        stmt = stmt.where(Product.price <= filters["price_max"])
    
    result = await db.execute(stmt)
    return result.scalars().all()
```

La fonction `plainto_tsquery` de PostgreSQL convertit automatiquement une chaîne en langage naturel (avec lemmatisation française) en expression de recherche, éliminant les mots vides ("le", "un", "de") et normalisant les formes fléchies ("disjoncteurs" → "disjoncteur").

### 3.4.3 La boucle de l'agent conversationnel

[IMAGE : Capture d'écran de l'interface chat avec exemples de requêtes et réponses]

La boucle de l'agent est implémentée dans le handler `POST /api/chat`. Elle maintient une liste de messages (historique de conversation) et exécute les appels d'outils en boucle jusqu'à ce que le LLM produise une réponse finale sans appel d'outil :

```python
async def run_agent(messages: List[dict], db: AsyncSession) -> str:
    max_iterations = 5  # Limite de sécurité anti-boucle infinie
    
    for _ in range(max_iterations):
        response = await call_llm(messages, tools=TOOL_DEFINITIONS)
        
        if response.tool_calls:
            # Exécuter chaque outil demandé
            for tool_call in response.tool_calls:
                result = await execute_tool(tool_call.name, tool_call.args, db)
                messages.append({
                    "role": "tool",
                    "tool_call_id": tool_call.id,
                    "content": json.dumps(result, ensure_ascii=False)
                })
            messages.append({"role": "assistant", "content": response.content})
        else:
            # Réponse finale sans appel d'outil
            return response.content
    
    return "Désolé, je n'ai pas pu traiter votre demande."
```

Un point d'attention particulier : les réponses sont formatées en **Dirham marocain (DH)** dans le prompt système, ce qui aligne la plateforme sur le contexte d'utilisation marocain.

&nbsp;

## 3.5 Interface Utilisateur

&nbsp;

### 3.5.1 Architecture SPA et routage

L'interface est une Single Page Application React organisée autour de React Router v7. La navigation utilise un `Layout` commun (sidebar de navigation, header avec informations utilisateur) et des composants de routes enfants pour chaque module.

Les routes protégées sont enveloppées dans un composant `RequireAuth` qui vérifie la présence et la validité du token JWT dans le contexte React avant d'afficher le contenu. En l'absence de token valide, l'utilisateur est redirigé vers la page de connexion.

### 3.5.2 Interface du module d'extraction

[IMAGE : Capture d'écran du module d'extraction - zone d'upload avec drag & drop]

[IMAGE : Capture d'écran des résultats d'extraction - tableau des circuits structurés]

L'interface d'extraction est organisée en trois zones :

1. **Zone d'upload :** Glisser-déposer ou sélection de fichier avec validation côté client (type MIME, taille). Un indicateur de progression affiche l'avancement de l'upload.

2. **Zone de contrôle :** Paramètres d'extraction configurables (tolérance Camelot, choix du fournisseur LLM, mode pipeline complet ou étape par étape) présentés dans un panneau accordéon.

3. **Zone de résultats :** Tableau interactif (TanStack Table) affichant les circuits extraits avec tri, filtrage et pagination. Un bouton d'export permet de télécharger les résultats au format Excel.

### 3.5.3 Interface du module de quantification

[IMAGE : Capture d'écran du module de quantification - viewer PDF avec détections superposées]

L'interface de quantification exploite `react-pdf` pour afficher le plan électrique avec les détections superposées sous forme de rectangles colorés. L'ingénieur peut :

- Naviguer entre les pages du plan
- Ajuster le seuil de confiance (slider) et relancer la détection
- Activer/désactiver les détections par type de symbole
- Cliquer sur une détection pour la supprimer
- Ajouter une détection manuellement par clic sur le plan

Les animations **Framer Motion** assurent des transitions fluides lors de l'apparition des détections et des changements de page.

### 3.5.4 Interface du catalogue et agent IA

[IMAGE : Capture d'écran de la recherche dans le catalogue de produits]

[IMAGE : Capture d'écran de l'interface de chat avec l'agent IA]

La page du catalogue est divisée en deux panneaux :
- **Panneau gauche :** Interface de recherche avec champ de saisie, filtres par fabricant/famille/fourchette de prix, et tableau de résultats paginés.
- **Panneau droit :** Interface de chat conversationnel avec l'agent IA, affichant l'historique des messages avec rendu Markdown (`react-markdown`).

&nbsp;

## 3.6 Déploiement et Infrastructure

&nbsp;

### 3.6.1 Architecture Docker de production

[IMAGE : Schéma d'architecture de déploiement Docker (conteneurs, réseaux, volumes)]

En production, l'application est déployée via Docker Compose avec quatre services :

```yaml
# docker-compose.prod.yml (extrait simplifié)
services:
  postgres:
    image: pgvector/pgvector:pg16
    volumes:
      - pg_data:/var/lib/postgresql/data
    environment:
      POSTGRES_DB: digiconstruct
  
  backend:
    build: ./digiconstruct/backend
    command: uvicorn main:app --host 0.0.0.0 --port 8000
    depends_on: [postgres]
    env_file: .env
    volumes:
      - uploads:/app/uploads
      - static:/app/static
  
  frontend:
    build: ./digiconstruct/frontend/gateway
    # Nginx sert les fichiers statiques React compilés
  
  caddy:
    image: caddy:2-alpine
    ports: ["80:80", "443:443"]
    # Reverse proxy HTTPS avec renouvellement automatique Let's Encrypt
```

La topologie réseau isole les services dans un réseau Docker privé (`digiconstruct_net`), avec seul Caddy exposé sur les ports publics 80 et 443. Le backend et PostgreSQL ne sont accessibles qu'en interne.

### 3.6.2 Initialisation de la base de données

Les migrations de base de données sont gérées par **Alembic** (outil de migration SQLAlchemy). La commande de démarrage du backend exécute automatiquement les migrations pending avant de lancer le serveur Uvicorn, garantissant que le schéma est toujours à jour au démarrage.

L'extension pgvector et le schéma `base_electrique` sont initialisés via un script SQL exécuté au premier démarrage de PostgreSQL (`init.sql` monté dans `/docker-entrypoint-initdb.d/`).

&nbsp;

## 3.7 Tests, Évaluation et Résultats

&nbsp;

### 3.7.1 Évaluation du module d'extraction

Les tests d'extraction ont été conduits sur un corpus de **10 notes de calcul Caneco BT** représentatives, couvrant des projets de différentes tailles (de 15 à 120 circuits) et différentes versions du logiciel (Caneco BT 6.x et 7.x).

**Tableau 7 : Résultats de performance du module d'extraction**

| Métrique | Valeur obtenue | Objectif |
|---|---|---|
| Taux de détection des tableaux circuits | 97% (97/100 tableaux) | ≥ 90% |
| Colonnes correctement extraites | 93% des colonnes sur l'ensemble du corpus | ≥ 90% |
| Tableaux nécessitant nettoyage manuel | 8% | ≤ 15% |
| Taux de succès structuration LLM | 96% (JSON valide, champs cohérents) | ≥ 95% |
| Temps moyen de traitement (20 pages) | 45 secondes (OpenRouter) | < 3 min |

Les 3% de tableaux non détectés concernent des notes de calcul exportées en mode image (non-vectoriel), pour lesquels une solution OCR serait nécessaire. Les échecs de structuration LLM (4%) sont principalement liés à des timeouts de l'API OpenRouter lors de pics de charge, gérés par le mécanisme de fallback vers HuggingFace.

### 3.7.2 Évaluation du module de quantification

Les tests de quantification ont été menés sur **5 plans électriques** représentatifs, avec un comptage manuel de référence réalisé par un ingénieur pour établir la vérité terrain.

**Tableau 8 : Résultats de précision du module de quantification**

| Symbole testé | Vrai positifs | Faux positifs | Faux négatifs | Précision | Rappel |
|---|---|---|---|---|---|
| Disjoncteur bipolaire | 48 | 3 | 2 | 94,1% | 96,0% |
| Prise de courant | 62 | 5 | 4 | 92,5% | 93,9% |
| Luminaire plafonnier | 35 | 1 | 3 | 97,2% | 92,1% |
| Interrupteur simple | 28 | 4 | 2 | 87,5% | 93,3% |
| **Total (tous symboles)** | **173** | **13** | **11** | **93,0%** | **94,0%** |

Ces résultats sont satisfaisants compte tenu de l'absence de données d'entraînement. Les faux positifs sont principalement dus à des similitudes visuelles entre certains symboles (ex: interrupteur et va-et-vient) ; les faux négatifs à des symboles partiellement masqués par du texte ou des cotations sur le plan.

### 3.7.3 Évaluation de l'agent conversationnel

**Tableau 9 : Jeu de données de test pour l'agent conversationnel**

| Catégorie de questions | Nb questions | Réponses pertinentes | Taux de succès |
|---|---|---|---|
| Recherche par caractéristiques techniques | 20 | 19 | 95% |
| Comparaison de produits | 10 | 9 | 90% |
| Requêtes de prix et disponibilité | 10 | 10 | 100% |
| Questions statistiques (nb produits, familles) | 5 | 5 | 100% |
| Questions hors domaine | 5 | 5 (refus correct) | 100% |
| **Total** | **50** | **48** | **96%** |

Les 2 questions non résolues concernaient des requêtes multi-critères complexes (ex: "trouve-moi un disjoncteur de 40A qui soit compatible avec un peigne de jeu de barres Legrand") où la combinaison de critères nécessitait plusieurs appels d'outils successifs que le modèle n'a pas enchaîné correctement. Cette limitation est typique des modèles légers (Llama 3.2 7B via Ollama) ; les performances sont nettement supérieures avec les modèles 70B.

### 3.7.4 Discussion et axes d'amélioration

L'évaluation confirme que DIGICONSTRUCT remplit ses objectifs initiaux. Plusieurs axes d'amélioration ont été identifiés pour les prochaines versions :

**Extraction :**
- Intégrer un module OCR (Tesseract ou AWS Textract) pour traiter les PDF scannés.
- Implémenter une interface de validation humaine pour les tableaux flaggés `needs_llm_review`.
- Explorer l'utilisation de Table Transformer (modèle deep learning) pour améliorer la détection des structures complexes.

**Quantification :**
- Constituer un dataset annoté de plans électriques marocains pour fine-tuner un modèle YOLO dédié.
- Ajouter la détection de symboles à l'échelle variable (pour les plans à différentes échelles de dessin).
- Intégrer le export du bordereau de matériel (quantités par symbole) vers Excel.

**Agent IA :**
- Implémenter une couche RAG (Retrieval-Augmented Generation) pour permettre à l'agent de répondre à des questions sur les fiches techniques produits (PDF fabricants).
- Explorer le fine-tuning d'un modèle spécialisé électrotechnique sur un corpus de questions/réponses métier.
- Ajouter une fonctionnalité de recommandation automatique de produits à partir des circuits extraits.

**Infrastructure :**
- Migrer le système de jobs asynchrones vers une file de messages dédiée (Redis + Dramatiq) pour la robustesse aux redémarrages serveur.
- Mettre en place une surveillance applicative (Prometheus + Grafana) pour le monitoring en production.
- Implémenter un système de cache Redis pour les résultats de recherche fréquents.

&nbsp;

---

&nbsp;

---

## Conclusion Générale

&nbsp;

### Bilan du projet

Ce stage a permis de mener à bien le développement de **DIGICONSTRUCT**, une plateforme logicielle originale répondant à un besoin concret et non satisfait dans le secteur de l'ingénierie électrique. En partant d'une problématique métier clairement identifiée - la faible automatisation du traitement des documents techniques en électrotechnique - nous avons conçu et implémenté une solution modulaire qui intègre des technologies de pointe : extraction de tableaux PDF avec Camelot, vision par ordinateur avec OpenCV, intelligence artificielle générative avec des LLMs multi-fournisseurs, et recherche plein texte avancée avec PostgreSQL.

Les résultats quantitatifs obtenus sont encourageants et dépassent les objectifs fixés en début de stage sur la quasi-totalité des métriques : 97% de taux de détection des tableaux de circuits, 96% de succès en structuration LLM, 93% de précision en détection de symboles et 96% de pertinence des réponses de l'agent conversationnel. Ces performances valident la viabilité technique de l'approche et démontrent qu'une solution de traitement intelligent de documents peut être construite avec des outils open source sans recourir exclusivement à des services cloud propriétaires.

Sur le plan architectural, le choix d'une **architecture modulaire asynchrone** (FastAPI + Python asyncio) s'est révélé judicieux : il permet de traiter des PDFs volumineux en arrière-plan sans bloquer l'API, tout en maintenant une cohérence de l'expérience utilisateur via le pattern de polling de jobs. La conteneurisation Docker garantit la reproductibilité des déploiements et facilite l'évolutivité future.

### Apports personnels

Au-delà des résultats techniques, ce stage a représenté une expérience formatrice à plusieurs niveaux. Sur le plan technique, j'ai approfondi ma maîtrise des frameworks web modernes (FastAPI, React), découvert les subtilités de l'intégration des LLMs dans des applications de production (gestion des erreurs, fallback, parsing robuste des sorties), et acquis une expérience concrète du déploiement Docker en environnement professionnel.

Sur le plan méthodologique, j'ai appliqué une démarche rigoureuse de développement logiciel : analyse des besoins, conception avant implémentation, tests quantitatifs avec métriques définies, documentation des décisions techniques. La nécessité de travailler sur un domaine métier spécialisé (électrotechnique, Caneco BT) m'a également conduit à développer des compétences d'ingénieur "traducteur" - capable de transformer une connaissance métier implicite en règles informatiques explicites.

Sur le plan professionnel, ce stage m'a permis de collaborer avec des ingénieurs électriciens expérimentés, d'apprendre à recueillir et formaliser des besoins techniques, et de livrer des fonctionnalités dans un environnement professionnel avec des contraintes de qualité et de délai réels.

### Perspectives et ouvertures

DIGICONSTRUCT constitue une base solide sur laquelle plusieurs évolutions à forte valeur ajoutée peuvent s'appuyer. À court terme, l'intégration d'un module OCR élargirait considérablement le périmètre des documents traités. À moyen terme, la construction d'un dataset annoté de plans électriques permettrait d'entraîner un modèle de détection dédié, qui surpasserait le template matching sur les plans avec variabilité de symboles. À plus long terme, la connexion de DIGICONSTRUCT avec des logiciels de conception électrique (Caneco BT lui-même, AutoCAD Electrical) via des APIs ou des formats d'échange standardisés (IFC, eHouse) ouvrirait la voie à un écosystème de l'ingénierie électrique numérique.

Plus fondamentalement, ce projet illustre la puissance de la combinaison LLM + bases de données structurées pour des applications d'entreprise spécialisées : les LLMs apportent la flexibilité de la compréhension en langage naturel, tandis que la base de données relationnelle apporte la précision, la traçabilité et la fiabilité exigées par les applications d'ingénierie. Cette architecture hybride, souvent désignée sous le terme de "LLM-augmented database", constitue à notre sens l'une des tendances architecturales les plus prometteuses pour les applications d'entreprise de la prochaine décennie.

&nbsp;

---

&nbsp;

---

## Références Bibliographiques

&nbsp;

**Bibliothèques et outils :**

[1] Krupnik, V. (2019). *Camelot: PDF Table Extraction for Humans*. GitHub. https://github.com/camelot-dev/camelot

[2] Bradski, G. (2000). The OpenCV Library. *Dr. Dobb's Journal of Software Tools*, 25(11), 120–123.

[3] Nieuwenburg, A. et al. (2022). *PyMuPDF - Python bindings for MuPDF*. GitHub. https://github.com/pymupdf/PyMuPDF

[4] Richardson, L. et al. (2022). *SQLAlchemy - The Database Toolkit for Python*. https://www.sqlalchemy.org/

[5] Ramirez, S. (2018). *FastAPI - Modern, fast web framework for building APIs with Python*. https://fastapi.tiangolo.com/

[6] Evans, E. (2020). *Vite - Next Generation Frontend Tooling*. https://vitejs.dev/

**Articles scientifiques :**

[7] Smith, R. (2007). An Overview of the Tesseract OCR Engine. *Proceedings of the Ninth International Conference on Document Analysis and Recognition*, 629–633.

[8] Ren, S., He, K., Girshick, R., & Sun, J. (2015). Faster R-CNN: Towards Real-Time Object Detection with Region Proposal Networks. *Advances in Neural Information Processing Systems*, 28.

[9] Lewis, P., et al. (2020). Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks. *Advances in Neural Information Processing Systems*, 33.

[10] Paliwal, S., et al. (2019). TableNet: Deep Learning Model for End-to-end Table Detection and Tabular Data Extraction from Scanned Document Images. *Proceedings of ICDAR 2019*, 128–133.

[11] Smock, B., Pesala, R., & Abraham, R. (2022). PubTables-1M: Towards Comprehensive Table Extraction From Unstructured Documents. *Proceedings of CVPR 2022*.

**Modèles de langage :**

[12] Meta AI. (2024). *Llama 3: Open Foundation and Fine-Tuned Chat Models*. https://ai.meta.com/blog/meta-llama-3/

[13] OpenAI. (2023). *GPT-4 Technical Report*. arXiv preprint arXiv:2303.08774.

[14] Google DeepMind. (2023). *Gemini: A Family of Highly Capable Multimodal Models*. arXiv preprint arXiv:2312.11805.

**Standards et normes :**

[15] CENELEC. (2011). *IEC 60617 - Graphical Symbols for Diagrams*. International Electrotechnical Commission.

[16] AFNOR. (2015). *NF C 15-100 - Installations électriques à basse tension*. Association française de normalisation.

&nbsp;

---

&nbsp;

---

## Annexes

&nbsp;

### Annexe A - Extrait du fichier de configuration d'import Excel (YAML)

```yaml
# digiconstruct/backend/backend_base/configs/schneider_test/schema.yaml
sheet_name: "Schneider"
skip_rows: 1
column_mapping:
  manufacturer: "Fabricant"
  family: "Gamme"
  reference: "Référence commerciale"
  designation: "Désignation"
  type: "Type"
  curve: "Courbe"
  poles: "Nbre de pôles"
  current_rating: "Calibre In (A)"
  breaking_capacity: "PdC Icu (kA)"
  price: "Prix HT (DH)"
  technical_data: null  # Colonne calculée depuis les autres champs
transformations:
  price:
    type: parse_price
    locale: "fr_MA"
  poles:
    type: parse_integer
  current_rating:
    type: parse_float
```

&nbsp;

### Annexe B - Extrait du prompt système LLM pour Caneco BT

```
Tu es un expert en électrotechnique basse tension, spécialisé dans l'analyse de notes 
de calcul Caneco BT. On te fournit un tableau extrait d'une note de calcul au format 
texte, avec des colonnes séparées par le caractère |.

Ton rôle est d'extraire les informations de chaque circuit et de les retourner 
EXCLUSIVEMENT au format JSON, sans aucun texte supplémentaire, sans markdown.

Le JSON doit respecter ce schéma :
{
  "reseau_regime": "TN-S|TN-C|TT|IT ou null",
  "tension": 230|400 ou null,
  "circuits": [
    {
      "repere": "identifiant du circuit (ex: P01, C12)",
      "designation": "description du récepteur",
      "nb": entier ou null,
      "puissance_kw": flottant ou null,
      "ib": flottant (courant emploi en A) ou null,
      "iz": flottant (courant admissible câble en A) ou null,
      ...
    }
  ]
}

Règles importantes :
- Les valeurs manquantes doivent être null, jamais des chaînes vides.
- Le repère est OBLIGATOIRE pour chaque circuit.
- Les unités sont : puissances en kW, courants en A, longueurs en m, sections en mm².
- Les calibres sont des entiers (10, 16, 20, 25, 32, 40, 63, 80, 100, 125...).
- Le champ "declencheur" contient des valeurs comme : C, D, MA, Courbe C, etc.
```

&nbsp;

### Annexe C - Documentation des endpoints API REST principaux

**Tableau : Schéma des endpoints REST de l'API**

| Méthode | Endpoint | Description | Auth |
|---|---|---|---|
| POST | `/api/v1/auth/register` | Créer un compte utilisateur | Non |
| POST | `/api/v1/auth/login` | Authentification (OAuth2 form) | Non |
| GET | `/api/v1/auth/me` | Profil utilisateur courant | JWT |
| POST | `/api/v1/upload` | Upload d'un fichier PDF | JWT |
| POST | `/api/v1/extract/stream/start` | Démarrer un job d'extraction | JWT |
| GET | `/api/v1/extract/stream/status` | Consulter l'état d'un job | JWT |
| GET | `/api/v1/files/{file_id}/result` | Récupérer le résultat d'extraction | JWT |
| POST | `/api/v1/excel` | Exporter les circuits en Excel | JWT |
| POST | `/upload-pdf` | Upload d'un plan (module quant.) | JWT |
| POST | `/detect-batch` | Lancer la détection en batch | JWT |
| GET | `/detect-batch/status/{job_id}` | État du job de détection | JWT |
| GET | `/api/search` | Recherche plein texte catalogue | JWT |
| GET | `/api/products` | Liste paginée des produits | JWT |
| POST | `/api/chat` | Envoyer un message à l'agent IA | JWT |
| POST | `/api/v1/import/excel` | Importer un catalogue Excel | JWT (Admin) |

&nbsp;

### Annexe D - Guide de démarrage rapide

**Prérequis :** Docker Engine ≥ 24.0, Docker Compose ≥ 2.20, Git

```bash
# 1. Cloner le dépôt
git clone <URL_DU_DEPOT> DIGICONSTRUCT
cd DIGICONSTRUCT

# 2. Configurer l'environnement
cp .env.example .env
# Éditer .env : renseigner AUTH_SECRET_KEY et optionnellement OPENROUTER_API_KEY

# 3. Démarrer la stack complète
docker-compose -f docker-compose.prod.yml up -d

# 4. Attendre que la base de données soit prête (environ 30s)
docker-compose logs -f postgres | grep "database system is ready"

# 5. L'application est accessible à http://localhost
# Compte administrateur initial : voir AUTH_INITIAL_USER_EMAIL/PASSWORD dans .env
```

Pour l'environnement de développement local (hot-reload) :

```bash
# Backend uniquement (PostgreSQL via Docker)
docker-compose up -d postgres
cd digiconstruct/backend
pip install -r backend_extract/requirements.txt \
            -r backend_quant/requirements.txt \
            -r backend_base/requirements.txt
uvicorn main:app --reload --port 8000

# Frontend (dans un autre terminal)
cd digiconstruct/frontend/gateway
npm install
npm run dev   # Démarre sur http://localhost:5173
```

&nbsp;

---

*Fin du mémoire de stage*

---

> **Note de mise en forme :** Ce document doit être mis en forme selon les normes HESTIM : police Times New Roman taille 12, interligne 1,5, marges 2,5 cm, titres en gras taille 14, paragraphes justifiés, retrait de première ligne 0,5 cm. La pagination commence à l'introduction. Les figures doivent être insérées aux emplacements indiqués par les balises `[IMAGE : ...]` avec la mention « Figure N : Intitulé » centrée sous chaque image.
