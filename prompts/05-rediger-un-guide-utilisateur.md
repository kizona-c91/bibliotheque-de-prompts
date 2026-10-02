---
id: "05"
titre: "Rédiger un guide utilisateur"
categorie: "Documentation"
version: 1.0
auteur: Kizona Chy
date: 2026-10
---

# 05. Rédiger un guide utilisateur

**Objectif :** Produire un guide d’une page, compréhensible par des utilisateurs non techniques.

**Quand l'utiliser :** Déploiement d’un outil ou d’un assistant auprès d’une équipe.

## Prompt

```text
Rôle : tu es rédacteur technique pour des utilisateurs non techniques.
Contexte : l'outil [nom] sert à [objectif]. Voici les étapes réelles d'utilisation : [étapes].
Tâche : rédige un guide d'une page : à quoi sert l'outil, prérequis, procédure pas à pas, erreurs fréquentes et solutions, bonnes pratiques de sécurité.
Contraintes : phrases courtes ; un verbe d'action par étape ; aucun jargon sans explication ; ne décris aucune fonction qui ne figure pas dans les étapes fournies.
Format : titres, étapes numérotées, encadré "À ne pas faire".
```

## Variables à remplacer

- `[nom]`
- `[objectif]`
- `[étapes]`

## Point de vigilance

Fais tester le guide par un utilisateur réel : c’est le seul moyen de repérer les étapes confuses.

---

[Retour à l'index](../README.md) · [Fiche de suivi](../templates/fiche-de-suivi.md)
