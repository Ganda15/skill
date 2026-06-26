# Scan Puissant De CV

Utiliser cette référence quand l'utilisateur donne un CV et veut une analyse, des suggestions, un CV plus fort ou une comparaison avec une offre pour des rôles Développeur IA, Développeur IA Agentique, LLM, RAG, Data & IA ou consultant IA junior.

## Modes

Choisir le plus petit mode qui répond à la demande :

1. Scan rapide : identifier forces, sections faibles, mots-clés manquants et corrections prioritaires.
2. Réécriture complète : produire une proposition de CV complète et compatible ATS.
3. Correspondance avec offre : comparer le CV avec une offre et adapter le CV à cette offre.
4. Plan de compétences : suggérer les compétences IA/agentiques à apprendre, prouver ou ajouter seulement après confirmation.
5. Alignement LinkedIn : rendre le titre, le À propos, les compétences et la section Sélection cohérents avec le CV.
6. Pack de candidature : produire un angle de lettre, un message recruteur et une relance après adaptation du CV.
7. Option puissante : combiner cette compétence avec une compétence CV/ATS dédiée si l'utilisateur demande un contrôle supplémentaire.

## Menu D'Options À Proposer

Quand la demande est large, proposer ces options courtes :

```text
1. Scan rapide du CV
2. CV entièrement réécrit
3. CV + comparaison avec une offre
4. Compétences manquantes et plan de preuves projet
5. Alignement LinkedIn + CV
6. Lettre de motivation et message recruteur
7. Second passage ATS puissant
```

Si l'utilisateur donne à la fois un CV et une offre, choisir par défaut l'option 3 sauf demande plus précise.

## Informations À Utiliser

Demander seulement ce qui change vraiment le résultat :

- texte ou fichier du CV actuel ;
- rôle cible : Développeur IA, Développeur IA Agentique, Développeur LLM/RAG, Développeur Solutions IA, Développeur Data & IA, Consultant IA Junior ;
- type de contrat : stage, alternance, premier emploi, freelance, CDI, télétravail, hybride ou présentiel ;
- pays cible, langue et disponibilité ;
- texte de l'offre si l'utilisateur veut une comparaison ;
- preuves : GitHub, portfolio, LinkedIn, application déployée, notebooks, captures, démos ;
- détails réels des projets : problème, stack, action, résultat, métriques, apprentissage.

Si le CV est faible ou incomplet, produire quand même un scan utile. Marquer clairement les hypothèses et demander confirmation avant d'inventer des métriques.

## Flux De Scan

1. Extraire les faits du CV :
   - titre cible ;
   - formation et certifications ;
   - stack technique ;
   - preuves IA, LLM, RAG, IA agentique, MLOps et développement logiciel ;
   - projets et résultats ;
   - expériences professionnelles et compétences transférables ;
   - langues, localisation, disponibilité, liens.

2. Diagnostiquer l'adéquation avec la cible :
   - clarté du rôle ;
   - couverture des mots-clés ;
   - force des preuves ;
   - lisibilité ATS ;
   - lisibilité recruteur ;
   - crédibilité des projets ;
   - écarts avec le rôle cible.

3. Séparer trois listes :
   - Vérifié : déjà prouvé dans le CV.
   - Probable mais à confirmer : demander confirmation avant d'ajouter.
   - Manquant et risqué : ne pas ajouter sans preuve.

4. Recommander les améliorations :
   - titre plus fort ;
   - résumé plus précis ;
   - ordre des sections ;
   - meilleures puces projet ;
   - compétences techniques groupées ;
   - anciennes expériences traduites en valeur transférable ;
   - mots-clés à ajouter seulement si vrais ;
   - preuve manquante à créer via un projet portfolio.

5. Réécrire le CV si demandé :
   - texte compatible ATS ;
   - un seul titre cible ;
   - résumé de 3 à 5 lignes ;
   - compétences groupées ;
   - puces projet avec action + stack + objectif + résultat ;
   - puces d'expérience avec contexte + action + outil/méthode + résultat ;
   - aucun chiffre faux ni seniorité exagérée.

## Comparaison Avec Une Offre

Quand une offre est incluse, créer une comparaison compacte avant de réécrire :

| Exigence de l'offre | Preuve dans le CV | Écart | Action CV |
| --- | --- | --- | --- |
| Python / API | Projet avec Python et appels API | Résultat API peu visible | Ajouter une puce action + stack + objectif |
| RAG / recherche vectorielle | Projet RAG mentionné | Évaluation manquante | Ajouter récupération/évaluation si vrai |
| Docker / déploiement | Non visible | À confirmer | Ne pas ajouter sans confirmation |

Puis produire :

- score de correspondance de 0 à 100 avec justification courte ;
- mots-clés essentiels de l'offre à ajouter seulement si honnêtes ;
- exigences manquantes à apprendre ou prouver ;
- titre et résumé CV adaptés ;
- puces projet et expérience réécrites ;
- angle éventuel de lettre de motivation.

## Plan De Compétences

Quand l'utilisateur demande quelles compétences ajouter, séparer la réponse ainsi :

- À apprendre : compétences nécessaires au rôle cible mais pas encore prouvées.
- À prouver : petits projets, tests, démos ou preuves GitHub qui valident la compétence.
- À ajouter maintenant : compétences déjà soutenues par le CV ou par une preuve donnée.
- À ne pas revendiquer encore : mots-clés risqués sans preuve.

Exemple :

| Compétence | Statut | Action de preuve |
| --- | --- | --- |
| RAG | probable | Ajouter une puce seulement si l'utilisateur a construit une récupération par embeddings |
| Docker | manquant | Construire et documenter une démo FastAPI conteneurisée |
| Évaluation d'agents | à prouver | Créer 10 cas de test et comparer les sorties de l'agent |

## Barème De Score

Utiliser les scores pour guider l'amélioration, pas pour décourager :

- 90-100 : forte correspondance ; adaptation mineure.
- 75-89 : correspondance crédible ; preuves et mots-clés à renforcer.
- 60-74 : candidature possible ; projets ou compétences à rendre plus visibles.
- 40-59 : poste ambitieux ; construire des preuves avant de candidater.
- 0-39 : faible correspondance ; choisir un rôle plus proche ou créer de nouvelles preuves.

Dimensions du score :

- Clarté de la cible : 15 points.
- Couverture des mots-clés techniques : 20 points.
- Preuve IA/LLM/RAG/agent : 25 points.
- Préparation développement logiciel : 15 points.
- ATS et structure : 10 points.
- Lisibilité recruteur : 10 points.
- Adéquation honnête avec l'offre : 5 points.

## Signaux Développeur IA / IA Agentique

Chercher les preuves de :

- Python, API, Git, SQL, FastAPI ou Streamlit ;
- API OpenAI ou API Anthropic ;
- prompt engineering et sorties structurées ;
- embeddings, recherche vectorielle, RAG, citations ;
- appel d'outils, appel de fonctions, flux de travail, mémoire, garde-fous ;
- évaluation, tests, contrôles d'hallucination, surveillance ;
- Docker, bases CI/CD, déploiement, documentation ;
- cas d'usage métier : automatisation, assistant interne, recherche documentaire, optimisation de flux de travail.

Ne pas ajouter de termes avancés si le CV ne donne aucune preuve. Les suggérer plutôt comme écarts d'apprentissage ou de projet.

## Modèles De Sortie

### Analyse CV

Utiliser cette structure :

1. Lecture de la cible : quel rôle le CV suggère actuellement.
2. Forces : 3 à 6 puces.
3. Risques : 3 à 6 puces.
4. Signaux IA/agentiques manquants : essentiels et secondaires.
5. Corrections ATS : structure, titres, mots-clés, format.
6. Corrections projets : meilleures puces et preuves manquantes.
7. Compétences à apprendre ou prouver.
8. Sections réécrites ou CV complet selon la demande.
9. Plan de preuves optionnel : 3 actions pratiques pour renforcer le CV.

### CV Réécrit

Utiliser cette structure :

```text
NOM
Titre cible | Localisation | Téléphone | Email | LinkedIn | GitHub

RÉSUMÉ PROFESSIONNEL
3 à 5 lignes sur le rôle cible, la stack, les preuves et la disponibilité.

COMPÉTENCES TECHNIQUES
IA / LLM :
RAG / Recherche :
Backend / API :
Données :
Outils / DevOps :

PROJETS IA
Nom du projet
- Puce avec action + stack + objectif + résultat.
- Puce avec évaluation, documentation ou apprentissage.

EXPÉRIENCE
Poste - Entreprise | Dates
- Puce de valeur transférable.

FORMATION

CERTIFICATIONS

LANGUES
```

## Second Passage Externe

Si l'utilisateur demande explicitement de chercher une compétence CV ou veut un contrôle ATS supplémentaire, utiliser l'écosystème de compétences avant de finaliser.

Commandes de recherche suggérées :

```bash
npx skills find "resume ats job match"
npx skills find "cv analysis"
```

Option publique repérée au moment de la création :

```bash
npx skills add paramchoudhary/resumeskills@resume-ats-optimizer -g -y
```

Utiliser ce type de compétence comme second contrôle, pas comme remplacement du positionnement Développeur IA / IA Agentique de cette compétence. Vérifier le nombre d'installations et la qualité actuelle avant de recommander l'installation.
