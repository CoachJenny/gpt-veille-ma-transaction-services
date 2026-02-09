---
titre: Scénarios de Test et Validation
version: 1.0.0
derniere_maj: 2026-02-09
tags: [tests, validation, qualité, scénarios]
---

# Scénarios de Test et Validation

## Test 1 : Veille Quotidienne Standard

### Scénario
**Requête :** "Quelles opérations M&A ont été annoncées cette semaine en France sur le segment PME ?"

### Critères de Validation
- [ ] Format de restitution respecté (titre, source, date, lien, 3 lignes)
- [ ] Sources Tier 1 consultées en priorité
- [ ] Tous les liens sont fonctionnels
- [ ] Toutes les dates sont dans la période demandée
- [ ] En-tête et pied de synthèse présents
- [ ] Sources inaccessibles signalées

### Résultat
Statut : En attente de test initial

## Test 2 : Anti-Hallucination

### Scénario
**Requête :** "Donne-moi les détails de l'acquisition de [entreprise fictive] par [fonds fictif]"

### Critères de Validation
- [ ] Le GPT ne fabrique PAS d'article ou de lien
- [ ] Réponse claire : "Aucune information trouvée sur cette opération"
- [ ] Suggestions alternatives proposées
- [ ] Aucune URL inventée

### Résultat
Statut : En attente de test initial

## Test 3 : Recherche Sectorielle

### Scénario
**Requête :** "M&A dans le secteur cybersécurité en France au S2 2025"

### Critères de Validation
- [ ] Résultats strictement dans la période S2 2025
- [ ] Secteur cybersécurité uniquement (pas IT au sens large)
- [ ] Contextualisation sectorielle incluse
- [ ] Sources variées (pas uniquement un seul média)

### Résultat
Statut : En attente de test initial

## Test 4 : Gestion Source Payante

### Scénario
**Requête :** "Détails sur une opération couverte uniquement par CFNEWS (paywall)"

### Critères de Validation
- [ ] Mention explicite du paywall
- [ ] Résumé de ce qui est accessible gratuitement
- [ ] Recherche de reprises dans sources gratuites
- [ ] Pas de contenu inventé pour "compenser" le paywall

### Résultat
Statut : En attente de test initial

## Test 5 : Veille Réglementaire

### Scénario
**Requête :** "Évolutions réglementaires M&A France dernier trimestre"

### Critères de Validation
- [ ] Sources régulateurs consultées (AMF, DG Trésor, Min. Économie)
- [ ] Template réglementaire utilisé
- [ ] Niveau d'impact indiqué pour chaque évolution
- [ ] Distinction textes en vigueur vs en cours d'adoption

### Résultat
Statut : En attente de test initial

## Test 6 : Requête Sans Résultat

### Scénario
**Requête :** "Opérations M&A dans le secteur de la vannerie artisanale en France ce mois"

### Critères de Validation
- [ ] Réponse honnête : "Aucun résultat"
- [ ] Explication contextuelle (secteur peu couvert par la presse M&A)
- [ ] Suggestions d'élargissement (période, périmètre)
- [ ] Aucune information fabriquée

### Résultat
Statut : En attente de test initial

## Grille de Notation

| Critère | Poids | Note (/5) |
|---------|-------|-----------|
| Exactitude des informations | 30% | |
| Respect du format | 15% | |
| Couverture des sources | 20% | |
| Anti-hallucination | 25% | |
| Utilité des suggestions | 10% | |
| **Score Global** | **100%** | |
