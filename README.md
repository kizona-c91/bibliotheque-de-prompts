# Bibliothèque de prompts

Collection de modèles de prompts réutilisables pour l'IA générative appliquée aux métiers. Les prompts servent à identifier des cas d'usage, concevoir et tester des assistants, rédiger des guides, former les utilisateurs et suivre des pilotes. Ils fonctionnent avec tout outil de chat basé sur un modèle de langage.

Auteur : Kizona Chy. Version initiale : 1.0, octobre 2026.

## Utilisation

1. Choisis un prompt dans l'index ci-dessous.
2. Copie le bloc `Prompt` du fichier.
3. Remplace chaque partie entre crochets, par exemple `[nom du processus]`. La section `Variables à remplacer` de chaque fichier liste ces parties.
4. Lis le `Point de vigilance` avant d'utiliser la réponse.
5. Note le résultat dans la [fiche de suivi](templates/fiche-de-suivi.md).

Les balises en majuscules, comme `[NOM]` ou `[ADRESSE]`, ne sont pas des variables. Ce sont des balises d'anonymisation à laisser telles quelles.

## Index

| N° | Prompt | Catégorie | Quand l'utiliser |
|----|--------|-----------|------------------|
| 01 | [Cartographier un processus et repérer les tâches automatisables](prompts/01-cartographier-un-processus.md) | Cadrage | Premier échange avec une équipe métier, avant de proposer un cas d’usage IA. |
| 02 | [Préparer un entretien de recueil de besoins](prompts/02-preparer-un-entretien-de-besoins.md) | Cadrage | Avant un entretien avec un responsable ou un utilisateur métier. |
| 03 | [Transformer des besoins en cas d’usage priorisés](prompts/03-prioriser-des-cas-d-usage.md) | Cadrage | Après plusieurs entretiens, pour préparer un arbitrage avec le responsable du projet. |
| 04 | [Extraire les informations d’un courrier ou d’un document](prompts/04-extraire-les-infos-d-un-document.md) | Traitement documentaire | Test d’automatisation du traitement documentaire, sur des documents anonymisés. |
| 05 | [Rédiger un guide utilisateur](prompts/05-rediger-un-guide-utilisateur.md) | Documentation | Déploiement d’un outil ou d’un assistant auprès d’une équipe. |
| 06 | [Définir les consignes d’un assistant interne (prompt système)](prompts/06-prompt-systeme-assistant-interne.md) | Assistants | Paramétrage d’un assistant documentaire ou d’un agent métier. |
| 07 | [Générer des cas de test pour un assistant IA](prompts/07-generer-des-cas-de-test.md) | Assistants | Avant un pilote, et après chaque modification des consignes. |
| 08 | [Évaluer la réponse d’un assistant avec une grille](prompts/08-evaluer-une-reponse-avec-une-grille.md) | Assistants | Suivi d’un pilote : contrôle d’un échantillon de réponses. |
| 09 | [Préparer un atelier de sensibilisation à l’IA](prompts/09-preparer-un-atelier-de-sensibilisation.md) | Formation | Acculturation d’une équipe métier aux usages de l’IA générative. |
| 10 | [Vérifier les données sensibles avant d’utiliser un outil IA](prompts/10-verifier-les-donnees-sensibles.md) | Sécurité et conformité | Avant d’envoyer un texte réel à un outil d’IA générative. |
| 11 | [Synthétiser une veille sur l’IA générative](prompts/11-synthetiser-une-veille-ia.md) | Veille | Veille régulière, à partager sous forme de note interne. |

## Méthode commune

Chaque prompt est construit avec six éléments. Cette structure rend les résultats plus fiables et permet de comparer deux versions d'un même prompt.

| Élément | Contenu |
|---------|---------|
| Rôle | Qui le modèle doit incarner. |
| Contexte | La situation et les informations utiles, sans donnée personnelle. |
| Tâche | Ce qui est attendu, en étapes numérotées. |
| Contraintes | Ce qui est interdit (inventer, deviner) et la conduite à tenir quand une information manque. |
| Format | La forme de la réponse (tableau, JSON, plan) pour qu'elle soit directement exploitable. |
| Vérification | Ce que l'humain contrôle avant d'utiliser la réponse. |

## Règles d'usage responsable

- Ne jamais coller de données personnelles, confidentielles ou clients dans un outil non validé par l'entreprise. Anonymiser d'abord avec le [prompt 10](prompts/10-verifier-les-donnees-sensibles.md).
- Considérer toute réponse comme un brouillon : relire et vérifier avant diffusion.
- Exiger les sources et signaler l'incertitude plutôt que de laisser le modèle deviner.
- Tester chaque prompt sur plusieurs cas, dont des cas difficiles, avant de le partager.
- Versionner les prompts : date, auteur, changement, résultat des tests.
- Garder l'humain responsable de la décision finale.

## Structure du dépôt

| Chemin | Contenu |
|--------|---------|
| `prompts/` | Un fichier par prompt, nommé `NN-titre-court.md`. |
| `templates/modele-de-prompt.md` | Modèle vide pour ajouter un prompt à la collection. |
| `templates/fiche-de-suivi.md` | Fiche à remplir à chaque test d'un prompt. |

Chaque fichier de prompt commence par un en-tête YAML : `id`, `titre`, `categorie`, `version`, `auteur`, `date`.

## Ajouter un prompt

1. Copie `templates/modele-de-prompt.md` dans `prompts/` avec le numéro suivant, par exemple `prompts/12-titre-court.md`.
2. Remplis les six éléments de la méthode commune.
3. Teste le prompt sur plusieurs cas, dont des cas difficiles, et remplis une fiche de suivi.
4. Ajoute une ligne dans l'index de ce README.

Pour modifier un prompt existant, augmente le champ `version` de son en-tête et décris le changement dans le message de commit.
