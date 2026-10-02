---
id: "01"
titre: "Cartographier un processus et repérer les tâches automatisables"
categorie: "Cadrage"
version: 1.0
auteur: Kizona Chy
date: 2026-10
---

# 01. Cartographier un processus et repérer les tâches automatisables

**Objectif :** Transformer la description d’un processus en étapes claires et classer chaque étape selon son potentiel d’automatisation.

**Quand l'utiliser :** Premier échange avec une équipe métier, avant de proposer un cas d’usage IA.

## Prompt

```text
Rôle : tu es analyste processus et tu aides une équipe métier à repérer des opportunités d'automatisation.
Contexte : je te décris le processus [nom du processus] tel qu'il est réalisé aujourd'hui : [description étape par étape, sans données personnelles].
Tâche :
1) Reformule le processus en étapes numérotées.
2) Pour chaque étape, indique l'acteur, l'outil utilisé, la durée estimée et le volume.
3) Classe chaque étape : "automatisable", "assistable par l'IA" ou "à garder humaine", avec une justification en une phrase.
4) Liste les informations manquantes.
Contraintes : n'invente aucune donnée chiffrée ; si une information manque, écris "à confirmer".
Format : un tableau (étape | acteur | outil | classement | justification), puis une liste "Questions à poser à l'équipe".
```

## Variables à remplacer

- `[nom du processus]`
- `[description étape par étape, sans données personnelles]`

## Point de vigilance

Les durées et volumes doivent être confirmés avec l’équipe : le modèle ne les connaît pas.

---

[Retour à l'index](../README.md) · [Fiche de suivi](../templates/fiche-de-suivi.md)
