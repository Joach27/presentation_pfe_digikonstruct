# Script de Soutenance de PFE — DigiKonstruct (Version 12 min Présentation + 3 min Démo)
**Présenté par :** Komivi Joachim AGBEVIADÉ  
**Filière :** Ingénierie Informatique et de l'Automatisme (IIA)  
**Spécialité :** Big Data & Intelligence Artificielle  
**Durée totale :** 15 minutes (12 min slides + 3 min démonstration)

---

## ⏱️ Structure Temporelle & Enchaînement

| N° | Section / Titre de la Diapositive | Durée slide | Temps cumulé |
|:---:|:---|:---:|:---:|
| **1** | **Couverture & Introduction** | 0:30 | **0:30** |
| **2** | **Plan de la présentation** | 0:20 | **0:50** |
| **3** | **00 · Entreprise : BIM Pioneers** | 0:35 | **1:25** |
| **4** | **01 · Contexte : Le quotidien du bureau d'études** | 0:35 | **2:00** |
| **5** | **02 · Problématique : La question centrale** | 0:35 | **2:35** |
| **6** | **03 · Objectifs du projet** | 0:30 | **3:05** |
| **7** | **03b · Besoins fonctionnels et non fonctionnels** | 0:30 | **3:35** |
| **8** | **04 · Planning Agile & Trajectoire** | 0:30 | **4:05** |
| **9** | **05 · Solution : Les trois modules** | 0:45 | **4:50** |
| **10**| **06 · Architecture globale de la plateforme** | 0:45 | **5:35** |
| **11**| **Module 1 : Extraction des notes de calcul** | 0:40 | **6:15** |
| **12**| **Module 2 : Quantification automatique** | 0:40 | **6:55** |
| **13**| **Module 2 · Démo : Balayage OpenCV (Interactif)** | 0:30 | **7:25** |
| **14**| **Module 3 : Chiffrage & Catalogue** | 0:40 | **8:05** |
| **15**| **07 · Interface Agent : Dialogue interactif** | 0:30 | **8:35** |
| **16**| **08 · Choix techniques (Tableau de synthèse)** | 0:35 | **9:10** |
| **17**| **09 · Résultats réels sur projets** | 0:40 | **9:50** |
| **18**| **10 · Conclusion & Perspectives** | 0:30 | **10:20** |
| **19**| **🎬 DÉMONSTRATION DE LA PLATEFORME** (Vidéo/Live) | **3:00** | **13:20** |
| **20**| **09b · Positionnement & Valeur Ajoutée** | 0:40 | **14:00** |
| **21**| **Merci pour votre attention** | 0:20 | **14:20** |

---

## 🎙️ Script Oral Détaillé (Slides : 12 minutes)

### 🔹 1. Couverture & Introduction (0:30)
* **Visuel :** *Logo Hestim & BIM Pioneers, Titre "DigiKonstruct", noms jury et encadrantes.*
* **Script oral :**
  > "Madame la présidente, Mesdames et Messieurs les membres du jury, bonjour.  
  > Je suis honoré de vous présenter aujourd'hui mon Projet de Fin d'Études intitulé **DigiKonstruct** : une plateforme d'extraction, de quantification et de chiffrage automatisés, augmentée par l'intelligence artificielle.  
  > Ce travail de fin d'études a été co-encadré par Mme Saida HAIDRAR et Mme Chaimae BALAKI au sein de la filière Ingénierie Informatique et de l'Automatisme, spécialité Big Data & IA."
* **🔄 Transition :** 
  > "Pour introduire notre sujet, voici le plan de notre intervention." *(Suivant)*

---

### 🔹 2. Plan (0:20)
* **Visuel :** *Agenda du projet en 7 points (00 à 06).*
* **Script oral :**
  > "Nous débuterons par la présentation de BIM Pioneers. Nous aborderons ensuite le contexte et la problématique métier, suivis des objectifs et du planning agile.  
  > Puis, nous analyserons l'architecture technique, le fonctionnement détaillé de nos trois modules métiers et les décisions d'ingénierie associées.  
  > Enfin, après une démonstration pratique de 3 minutes, nous conclurons avec l'analyse de nos résultats."
* **🔄 Transition :** 
  > "Commençons par faire connaissance avec notre structure d'accueil." *(Suivant)*

---

### 🔹 3. 00 · Entreprise : BIM Pioneers (0:35)
* **Visuel :** *Identité de BIM Pioneers à Casablanca, CEO Sadik EL ABASSI, expertises.*
* **Script oral :**
  > "J'ai réalisé mon stage chez **BIM Pioneers**, entreprise marocaine d'ingénierie basée à Casablanca, fondée par M. Sadik EL ABASSI, ingénieur EHTP et expert BIM.  
  > L'entreprise est spécialisée dans l'accélération des performances de construction en combinant le BIM et l'intelligence artificielle.  
  > Ses expertises s'organisent autour de quatre piliers : le conseil BIM stratégique, la modélisation multidisciplinaire, la formation et le développement d'outils d'IA sur mesure au sein du Pôle Innovation où mon projet a été conçu."
* **🔄 Transition :** 
  > "Découvrons le contexte opérationnel à l'origine de notre projet." *(Suivant)*

---

### 🔹 4. 01 · Contexte : Le quotidien du bureau d'études (0:35)
* **Visuel :** *Note de calcul Caneco BT, Plan électrique, Devis Excel. KPIs : 2h par affaire, erreurs, non traçable.*
* **Script oral :**
  > "Le quotidien d'un ingénieur en bureau d'études électricité repose sur trois documents distincts : la note de calcul PDF issue de Caneco BT, le plan d'implantation technique au format DWG ou PDF, et le catalogue tarifaire des fabricants.  
  > Actuellement, le chiffrage s'effectue manuellement : l'ingénieur compte les symboles à l'œil nu sur le plan et saisit les lignes de circuits une par une dans Excel.  
  > Ce travail prend en moyenne **deux heures par dossier**, comporte des risques importants d'erreurs de comptage, et manque de traçabilité lors des révisions."
* **🔄 Transition :** 
  > "Ce constat nous amène à formaliser la problématique du projet." *(Suivant)*

---

### 🔹 5. 02 · Problématique : La question centrale (0:35)
* **Visuel :** *Question centrale et trois sous-problèmes (SP-01, SP-02, SP-03).*
* **Script oral :**
  > "Notre question centrale est la suivante : **Comment automatiser le traitement de ces documents techniques en électricité afin d'extraire, quantifier et chiffrer ces composants, tout en conservant la fiabilité requise en ingénierie ?**  
  > Nous avons décomposé ce défi en trois sous-problèmes :  
  > Le **SP-01** : l'extraction et la structuration de notes de calcul PDF hétérogènes.  
  > Le **SP-02** : la détection et le comptage automatique de symboles sur plans haute résolution.  
  > Et le **SP-03** : l'appariement sémantique fiable avec le catalogue produits et l'interaction en langage naturel."
* **🔄 Transition :** 
  > "Pour relever ces défis, nous avons fixé cinq objectifs précis." *(Suivant)*

---

### 🔹 6. 03 · Objectifs du projet (0:30)
* **Visuel :** *Escalier des 5 objectifs corrélés aux phases.*
* **Script oral :**
  > "Nos objectifs suivent une trajectoire rigoureuse :  
  > Premièrement, analyser les besoins métier des électriciens.  
  > Deuxièmement, concevoir une architecture logicielle modulaire.  
  > Troisièmement, développer les trois modules métiers d'extraction, de quantification et de chiffrage.  
  > Quatrièmement, évaluer précisément les performances des algorithmes.  
  > Et cinquièmement, packager et déployer l'application sous forme de conteneurs Docker."
* **🔄 Transition :** 
  > "Pour répondre à ce premier objectif d'analyse, voyons en détail les exigences fonctionnelles et non fonctionnelles identifiées." *(Suivant)*

---

### 🔹 7. 03b · Besoins fonctionnels et non fonctionnels (0:30)
* **Visuel :** *Deux colonnes comparatives présentant d'un côté l'extraction/quantification/chiffrage et de l'autre la performance/résilience/sécurité.*
* **Script oral :**
  > "Cette phase d'analyse a permis de formaliser nos besoins.  
  > Sur le plan fonctionnel, le système doit assurer l'extraction automatisée des notes de calcul, la détection visuelle de composants sur plans, et l'aide au chiffrage via un agent conversationnel.  
  > Sur le plan non fonctionnel, nous ciblons un temps de traitement inférieur à 3 minutes, une sécurité via authentification JWT, et surtout une souveraineté grâce au basculement automatique sur un LLM local en cas de perte de connexion."
* **🔄 Transition :** 
  > "Voyons comment ces travaux se sont planifiés dans le temps pour satisfaire ces exigences." *(Suivant)*

---

### 🔹 8. 04 · Planning Agile & Trajectoire (0:30)
* **Visuel :** *Timeline de 5 mois, Gantt et Kanban GitHub.*
* **Script oral :**
  > "Pour mener à bien ce projet de 5 mois, nous avons adopté une méthodologie agile rythmée par des sprints hebdomadaires et des revues avec le Product Owner.  
  > Après la phase d'étude, nous avons développé le module d'extraction au mois 2, la quantification au mois 3 et le chiffrage au mois 4.  
  > Le dernier mois a été dédié à l'interface React, aux tests de performance et aux préparatifs de déploiement."
* **🔄 Transition :** 
  > "Présentons maintenant la structure de notre solution." *(Suivant)*

---

### 🔹 9. 05 · Solution : Les trois modules (0:45)
* **Visuel :** *Les modules d'Extraction, Quantification et Chiffrage avec leurs flux d'entrées/sorties.*
* **Script oral :**
  > "Notre plateforme **DigiKonstruct** s'articule autour des trois modules conçus pour répondre à nos sous-problèmes :  
  > **Module 1 (Extraction) :** Convertit les rapports PDF Caneco en données JSON de circuits structurés.  
  > **Module 2 (Quantification) :** Analyse le plan technique et génère la nomenclature des symboles détectés.  
  > **Module 3 (Chiffrage) :** Associe sémantiquement les circuits et symboles aux tarifs du catalogue pour exporter le devis final.  
  > Le système repose sur **FastAPI** en backend, **PostgreSQL** pour la base de données, et **React** en frontend."
* **🔄 Transition :** 
  > "Voyons l'architecture technique qui soutient ces modules." *(Suivant)*

---

### 🔹 10. 06 · Architecture globale de la plateforme (0:45)
* **Visuel :** *Diagramme d'architecture SVG (React, FastAPI, PostgreSQL, pgvector, LLMs).*
* **Script oral :**
  > "L'architecture technique est orientée micro-services et intègre des briques d'intelligence artificielle.  
  > Le frontend React interroge de manière asynchrone notre API FastAPI.  
  > Côté données, PostgreSQL stocke notre catalogue et gère les recherches vectorielles grâce à l'extension **pgvector**.  
  > Enfin, pour les interactions IA, nous exploitons une passerelle multi-LLM intelligente. Elle interroge en priorité les modèles distants via OpenRouter ou HuggingFace, et bascule sur un modèle **Ollama local** en cas de coupure réseau ou pour garantir une confidentialité totale."
* **🔄 Transition :** 
  > "Entrons dans le détail algorithmique de chaque module." *(Suivant)*

---

### 🔹 11. Module 1 : Extraction des notes de calcul (0:40)
* **Visuel :** *Note de calcul Caneco PDF -> Camelot Stream -> TableCleaner -> LLM -> JSON.*
* **Script oral :**
  > "Le premier module extrait les données tabulaires des notes de calcul.  
  > Nous utilisons la bibliothèque Python **Camelot** (en mode Stream) pour cibler et extraire les lignes de tableaux bruts.  
  > Ces données sont ensuite nettoyées et réalignées par notre algorithme **TableCleaner** pour corriger les sauts de lignes et les colonnes mal fusionnées.  
  > Enfin, ces informations textuelles sont transmises au LLM pour être transformées sémantiquement en un fichier **JSON structuré** contenant toutes les caractéristiques électriques des circuits."
* **🔄 Transition :** 
  > "Parallèlement, le second module assure l'analyse visuelle des plans." *(Suivant)*

---

### 🔹 12. Module 2 : Quantification automatique (0:40)
* **Visuel :** *Plan technique avec boîtes de détection. OpenCV matchTemplate et NMS.*
* **Script oral :**
  > "Pour localiser et compter les équipements sur le plan d'implantation, nous avons choisi une approche par vision par ordinateur classique : le **Template Matching OpenCV**.  
  > L'algorithme fait glisser un gabarit (un symbole type) sur le plan et calcule une corrélation croisée normalisée. Les détections multiples sur un même symbole sont éliminées grâce à un algorithme de **suppression des non-maxima (NMS)**.  
  > Cette approche présente l'avantage majeur de ne nécessiter **aucun dataset annoté ni entraînement lourd**, s'adaptant immédiatement à tout nouveau symbole de légende."
* **🔄 Transition :** 
  > "Voici une illustration interactive de ce balayage en temps réel." *(Suivant)*

---

### 🔹 13. Module 2 · Démo : Balayage OpenCV (Interactif) (0:30)
* **Visuel :** *Interface interactive avec bouton "Détecter les symboles", réticule de visée et terminal de log.*
* **Script oral :**
  > "Sur cette interface, nous simulons le fonctionnement du module de vision.  
  > *(Optionnel : Cliquer sur le bouton 'Détecter les symboles' pour lancer l'animation)*  
  > Le système balaie le plan technique et détecte ici instantanément nos 8 luminaires, comme le montre le terminal de log en temps réel.  
  > Cette méthode assure une détection géométrique fiable et rapide, sans surcharge de calcul."
* **🔄 Transition :** 
  > "Passons maintenant au troisième module, le chiffrage et l'accès au catalogue." *(Suivant)*

---

### 🔹 14. Module 3 : Chiffrage & Catalogue (0:40)
* **Visuel :** *Lien JSON -> Matching -> Devis Excel final, et à droite le diagramme animé du pipeline ETL (Extract -> Transform -> Load).*
* **Script oral :**
  > "Une fois les composants extraits et quantifiés, le module de chiffrage prend le relais.  
  > Pour alimenter notre catalogue de prix, nous avons conçu un **pipeline d'import ETL automatisé**. Il extrait les données des catalogues Excel bruts des fabricants, les nettoie et les normalise via Pandas (calibre, pôles, courbe), puis les charge dans PostgreSQL.  
  > Lors du chiffrage, chaque composant est associé sémantiquement au catalogue par recherche plein texte et score pondéré, générant automatiquement le devis Excel final."
* **🔄 Transition :** 
  > "Voyons comment l'utilisateur interagit en langage naturel avec ce système." *(Suivant)*

<!--
---

### 🔹 14. Module 3 : Équivalences inter-marques (0:30)
* **Visuel :** *Écran d'équivalences de produits, calcul du prix net avec remise.*
* **Script oral :**
  > "Le module intègre un comparateur d'équivalences de produits entre fabricants.  
  > En cas d'indisponibilité ou pour optimiser les coûts, l'algorithme utilise **pgvector** pour calculer la similarité cosinus entre les descriptions des équipements.  
  > Un filtrage strict par type de produit garantit la pertinence technique, et le système calcule le prix net réel après application de la remise négociée avec le fournisseur."
* **🔄 Transition :** 
  > "Voyons comment l'utilisateur interagit en langage naturel avec ce système." *(Suivant)*
-->

---

### 🔹 15. 07 · Interface Agent : Dialogue interactif (0:30)
* **Visuel :** *Simulateur de chat à gauche ; panneau d'analyse (1/3 hauteur) et capture d'écran de la réponse générée (2/3 hauteur) à droite.*
* **Script oral :**
  > "Pour simplifier l'accès aux données, nous avons intégré un agent conversationnel.  
  > *(Optionnel : Cliquer sur 'Simuler' pour lancer l'animation)*  
  > L'utilisateur peut demander en langage naturel d'ajouter un équipement, de remplacer une référence ou d'exporter un devis.  
  > Le panneau de droite montre l'analyse en temps réel de l'agent : extraction de l'intention, appel de la base vectorielle, exécution des fonctions métiers et génération du tableur Excel."
* **🔄 Transition :** 
  > "Pour valider l'ensemble de ces briques, voici une synthèse de nos choix d'ingénierie." *(Suivant)*

<!--
---

### 🔹 16. 07 · Cœur IA : Boucle function-calling (0:40)
* **Visuel :** *Code Python asynchrone du function-calling, mécanisme de cascade et robustesse.*
* **Script oral :**
  > "Le cœur de l'agent IA repose sur une boucle de **Function-Calling** asynchrone.  
  > À chaque message, le LLM analyse si l'action requiert l'appel d'un outil (comme interroger le catalogue ou modifier le devis). L'application exécute alors cet outil en base de données et renvoie le résultat au LLM.  
  > Nous limitons la boucle à 5 itérations pour éviter les comportements infinis, et un parser tolérant nettoie les retours du modèle pour garantir la stabilité du système, même avec des modèles locaux plus légers."
* **🔄 Transition :** 
  > "Pour valider l'ensemble de ces briques, voici une synthèse de nos choix d'ingénierie." *(Suivant)*
-->

---

### 🔹 16. 08 · Choix techniques (Tableau de synthèse) (0:35)
* **Visuel :** *Tableau récapitulatif des choix technologiques et des critères de sélection.*
* **Script oral :**
  > "Ce tableau résume nos arbitrages techniques.  
  > Nous avons systématiquement privilégié des outils open source et légers : **Camelot** pour les PDF, **OpenCV** pour la vision, et **pgvector** intégré dans PostgreSQL pour la recherche vectorielle.  
  > Ce choix d'infrastructure unifiée nous évite de déployer une base vectorielle dédiée ou d'avoir recours à des services cloud onéreux, facilitant ainsi la maintenance et respectant la confidentialité des données de l'entreprise."
* **🔄 Transition :** 
  > "Voyons l'évaluation quantitative de ces choix sur des projets réels." *(Suivant)*

---

### 🔹 17. 09 · Résultats réels sur projets (0:40)
* **Visuel :** *KPIs de performance (97% extraction, >75% vision, 87.5% chiffrage, 99% temps gagné).*
* **Script oral :**
  > "L'évaluation finale sur des projets réels fournis par BIM Pioneers valide les performances attendues :  
  > Nous atteignons **97 %** de détection des tableaux sur les PDF natifs, plus de **75 %** de précision en vision par ordinateur sans aucun entraînement, et **87,5 %** d'appariement automatique avec le catalogue.  
  > Au final, c'est **99 % de temps gagné sur le chiffrage**, qui passe de **2 heures à moins de 40 secondes**, sécurisant le calcul et augmentant la productivité des ingénieurs."
* **🔄 Transition :** 
  > "Forts de ces résultats d'évaluation, dressons maintenant le bilan final de ce travail et projetons ses perspectives d'évolution." *(Suivant)*

---

### 🔹 18. 10 · Conclusion & Perspectives (0:30)
* **Visuel :** *Ce qui a été réalisé et les axes d'évolution futurs.*
* **Script oral :**
  > "En conclusion, DigiKonstruct est une plateforme complète et opérationnelle, conteneurisée et prête au déploiement en production.  
  > Les perspectives futures s'orientent vers l'entraînement d'un modèle YOLO sur un dataset de plans électriques annotés pour améliorer la détection de vision, et la création de connecteurs directs sous forme de plugins pour les outils BIM comme Autodesk Revit."
* **🔄 Transition :** 
  > "Pour rendre ces travaux concrets, je vous propose maintenant de visionner une démonstration de 3 minutes de l'application en action." *(Suivant)*

---

## 🎬 Script de la Démonstration (3 minutes)

* **Visuel :** *Diapositive 20 ("Démonstration vidéo"). Lancement de la vidéo `demo00.webm` ou manipulation de l'application en direct.*
* **Durée :** 3:00  

#### ⏱️ Étape 1 : Interface React & Module 1 (Extraction) — [0:00 à 0:45]
> "Voici l'interface utilisateur de notre application DigiKonstruct. Nous allons commencer par importer notre note de calcul Caneco BT au format PDF.  
> En cliquant sur 'Importer', l'API FastAPI envoie le fichier à notre pipeline. Vous voyez à l'écran l'extraction s'effectuer en direct.  
> La table de calcul est analysée, nettoyée par TableCleaner, puis le LLM structure instantanément les données. Nous obtenons cette liste propre de circuits au format JSON avec leurs calibres, protections et désignations.  
> L'ingénieur peut à tout moment modifier ou valider ces données extraites directement dans le tableau."

#### ⏱️ Étape 2 : Vision & Module 2 (Quantification) — [0:45 à 1:45]
> "Passons maintenant au deuxième module : la quantification sur le plan d'implantation.  
> Nous chargeons le plan de l'étage au format image haute définition. Dans le panneau de configuration, nous sélectionnons le symbole du luminaire directement depuis la légende pour servir de gabarit.  
> En lançant la détection, l'algorithme de Template Matching parcourt le plan. Vous voyez apparaître en vert les boîtes de détection sur chaque luminaire identifié. L'algorithme NMS a correctement fusionné les détections pour éviter les doublons.  
> En quelques secondes, le compteur affiche 8 luminaires détectés, et nous exportons cette nomenclature directement vers notre base de données."

#### ⏱️ Étape 3 : Chiffrage automatique & Agent conversationnel — [1:45 à 2:45]
> "Le troisième module regroupe ces données pour le chiffrage.  
> En ouvrant l'onglet chiffrage, le système associe automatiquement nos circuits aux références correspondantes du catalogue Schneider dans PostgreSQL.  
> Pour affiner le devis, nous pouvons ouvrir le panneau de l'agent conversationnel. Je lui demande simplement en langage naturel : *'Remplace la référence du disjoncteur P02 par un équivalent chez ABB avec notre remise négociée'*.  
> L'agent comprend la consigne, effectue une recherche vectorielle cosinus via pgvector, applique la remise de la table discount_rates, et modifie la ligne du devis en temps réel. Le prix net total est mis à jour instantanément."

#### ⏱️ Étape 4 : Conclusion de la démo — [2:45 à 3:00]
> "Enfin, nous cliquons sur 'Exporter' pour télécharger le devis finalisé au format Excel.  
> Cette démonstration prouve le bon fonctionnement de notre chaîne de traitement de bout en bout, offrant une interface intuitive et rapide aux ingénieurs pour diviser leur temps de chiffrage par 100."
* **🔄 Transition :** 
  > "Pour clore cette démonstration, résumons la valeur ajoutée concrète de DigiKonstruct par rapport à la méthode manuelle traditionnelle." *(Suivant)*

---

### 🔹 20. 09b · Positionnement & Valeur Ajoutée (0:40)
* **Visuel :** *Comparaison côte à côte (2 colonnes) : le processus manuel traditionnel (à gauche, rouge) face à la solution DigiKonstruct (à droite, vert) sur 3 axes clés.*
* **Script oral :**
  > "Cette slide met directement en contraste l'approche traditionnelle avec notre solution DigiKonstruct sur trois dimensions clés.  
  > Premièrement, là où l'approche manuelle exigeait une saisie et un comptage visuel fastidieux sur plans, DigiKonstruct propose une automatisation complète de la chaîne d'extraction, de quantification et de chiffrage.  
  > Deuxièmement, le temps de traitement, qui demandait en moyenne 2 heures par dossier, est réduit à moins de 40 secondes.  
  > Enfin, nous éliminons les risques d'oublis de comptage ou d'erreurs humaines de ressaisie, fiabilisant le chiffrage final. C'est un gain de productivité et de rigueur immédiat pour le bureau d'études."
* **🔄 Transition :** 
  > "C'est sur cette synthèse de valeur ajoutée que je conclus ma présentation. Je vous remercie pour votre attention." *(Suivant)*

---

### 🔹 21. Merci pour votre attention (0:20)
* **Visuel :** *Diapositive de fin.*
* **Script oral :**
  > "Je vous remercie pour votre attention et je suis maintenant ravi de répondre à vos questions."
