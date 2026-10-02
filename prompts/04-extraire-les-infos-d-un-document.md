---
id: "04"
titre: "Extraire les informations d’un courrier ou d’un document"
categorie: "Traitement documentaire"
version: 1.0
auteur: Kizona Chy
date: 2026-10
---

# 04. Extraire les informations d’un courrier ou d’un document

**Objectif :** Obtenir une extraction structurée et vérifiable, sans que le modèle invente ce qui est absent.

**Quand l'utiliser :** Test d’automatisation du traitement documentaire, sur des documents anonymisés.

## Prompt

```text
Rôle : tu es assistant de traitement documentaire.
Contexte : le texte ci-dessous est un courrier dont les données personnelles ont été remplacées par des balises : [texte anonymisé].
Tâche : extrais le type de document, l'organisation expéditrice, la date, l'objet, l'action demandée, la date limite et les pièces à fournir.
Contraintes : n'utilise que ce qui figure dans le texte ; si une information est absente, écris "non trouvé" ; ne devine pas.
Format : un objet JSON avec les clés type, expediteur, date, objet, action, echeance, pieces, plus une clé confiance (haute, moyenne ou faible) accompagnée d'une phrase d'explication.
```

## Variables à remplacer

- `[texte anonymisé]`

## Point de vigilance

Anonymise toujours avant d’envoyer le texte (voir prompt 10) et contrôle un échantillon à la main : les dates sont une source d’erreur fréquente.

## Prompts liés

- [10. Vérifier les données sensibles avant d’utiliser un outil IA](10-verifier-les-donnees-sensibles.md)

---

[Retour à l'index](../README.md) · [Fiche de suivi](../templates/fiche-de-suivi.md)
