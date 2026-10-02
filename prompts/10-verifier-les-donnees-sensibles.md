---
id: "10"
titre: "Vérifier les données sensibles avant d’utiliser un outil IA"
categorie: "Sécurité et conformité"
version: 1.0
auteur: Kizona Chy
date: 2026-10
---

# 10. Vérifier les données sensibles avant d’utiliser un outil IA

**Objectif :** Repérer les données personnelles ou confidentielles et obtenir une version anonymisée.

**Quand l'utiliser :** Avant d’envoyer un texte réel à un outil d’IA générative.

## Prompt

```text
Rôle : tu es assistant de conformité (aide à la décision, pas décision finale).
Contexte : je veux envoyer le texte suivant à un outil d'IA générative : [texte].
Tâche : repère les données personnelles ou confidentielles (noms, adresses, numéros, données financières ou de santé, informations clients), propose une version anonymisée avec des balises ([NOM], [ADRESSE]...), et indique si le texte peut être envoyé après anonymisation.
Contraintes : en cas de doute, recommande de ne pas l'envoyer et de consulter la politique de l'entreprise.
Format : liste des éléments repérés, texte anonymisé, recommandation.
```

## Variables à remplacer

- `[texte]`

## Point de vigilance

Cet outil ne remplace ni la politique de sécurité de l’entreprise ni l’avis du responsable de la protection des données. N’utilise que les outils validés par l’entreprise.

---

[Retour à l'index](../README.md) · [Fiche de suivi](../templates/fiche-de-suivi.md)
