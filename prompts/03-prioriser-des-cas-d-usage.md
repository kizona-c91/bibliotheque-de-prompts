---
id: "03"
titre: "Transformer des besoins en cas d’usage priorisés"
categorie: "Cadrage"
version: 1.0
auteur: Kizona Chy
date: 2026-10
---

# 03. Transformer des besoins en cas d’usage priorisés

**Objectif :** Passer de notes brutes à des fiches de cas d’usage comparables et à un ordre de priorité argumenté.

**Quand l'utiliser :** Après plusieurs entretiens, pour préparer un arbitrage avec le responsable du projet.

## Prompt

```text
Rôle : tu es chef de projet IA.
Contexte : voici les besoins recueillis : [notes brutes, sans données personnelles].
Tâche : transforme-les en cas d'usage. Pour chacun : titre, problème métier, solution IA envisagée, utilisateurs, données nécessaires, risques, indicateur de succès. Note ensuite chaque cas de 1 à 5 sur la valeur métier, la faisabilité et le risque (5 = risque faible), puis propose un ordre de priorité justifié.
Contraintes : n'invente aucun gain chiffré ; écris "hypothèse" quand tu estimes.
Format : une fiche par cas d'usage, puis un tableau (cas | valeur | faisabilité | risque | score).
```

## Variables à remplacer

- `[notes brutes, sans données personnelles]`

## Point de vigilance

Les scores servent à lancer la discussion, pas à décider seuls : fais valider par les métiers.

---

[Retour à l'index](../README.md) · [Fiche de suivi](../templates/fiche-de-suivi.md)
