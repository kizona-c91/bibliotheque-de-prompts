---
id: "08"
titre: "Évaluer la réponse d’un assistant avec une grille"
categorie: "Assistants"
version: 1.0
auteur: Kizona Chy
date: 2026-10
---

# 08. Évaluer la réponse d’un assistant avec une grille

**Objectif :** Noter une réponse de façon cohérente et repérer les affirmations non appuyées par les sources.

**Quand l'utiliser :** Suivi d’un pilote : contrôle d’un échantillon de réponses.

## Prompt

```text
Rôle : tu es évaluateur qualité.
Contexte : question posée : [question]. Réponse de l'assistant : [réponse]. Documents de référence : [extraits].
Tâche : note la réponse de 1 à 5 sur l'exactitude, la complétude, la traçabilité des sources, la clarté et le respect des règles. Justifie chaque note en une phrase, cite l'élément précis de la réponse concerné et signale toute affirmation non appuyée par les documents.
Format : un tableau (critère | note | justification), puis un verdict (acceptable, à corriger ou à refuser) et la correction proposée.
```

## Variables à remplacer

- `[question]`
- `[réponse]`
- `[extraits]`

## Point de vigilance

Un évaluateur IA peut se tromper : relis un échantillon à la main avant de tirer des conclusions.

---

[Retour à l'index](../README.md) · [Fiche de suivi](../templates/fiche-de-suivi.md)
