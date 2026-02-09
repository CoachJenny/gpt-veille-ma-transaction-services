---
titre: Méthodologie de Veille M&A
version: 1.0.0
derniere_maj: 2026-02-09
utilisations: 0
efficacite: N/A
tags: [procédure, veille, méthodologie, recherche, M&A]
---

# Méthodologie de Veille M&A - Procédure Standard

## Workflow de Recherche en 7 Étapes

### Étape 1 : Qualifier la Demande
Avant toute recherche, clarifier avec l'utilisateur :
- **Période** : dates exactes (du JJ/MM/AAAA au JJ/MM/AAAA)
- **Périmètre géographique** : France entière, région, secteur
- **Type d'opération** : M&A, LBO, levée de fonds, cession, transmission
- **Secteur d'activité** : si spécifique
- **Taille d'opération** : PME (<50M€), ETI (<1,5Md€), toutes tailles
- **Niveau de détail** : synthèse rapide vs analyse approfondie

### Étape 2 : Sélectionner les Sources
Selon le type de demande, prioriser :

| Type de demande | Sources prioritaires | Sources complémentaires |
|----------------|---------------------|----------------------|
| Opération spécifique | CFNEWS, Les Échos, BODACC | Pappers, AMF (si cotée) |
| Tendances marché | France Invest, Grant Thornton, EY | Bpifrance, In Extenso |
| Réglementaire | AMF, DG Trésor, Min. Économie | ACPR, Ordre EC, CNCC |
| Levées de fonds | Maddyness, FrenchWeb, CFNEWS | Bpifrance, France Invest |
| Données entreprise | Pappers, BODACC, INPI | data.gouv.fr, SIRENE |
| Secteur financier | ACPR, Banque de France, AMF | L'AGEFI, Option Finance |

### Étape 3 : Exécuter la Recherche

**RÈGLE CRITIQUE : Privilégier la granularité opérationnelle**
- Pour les demandes "veille [période]", l'utilisateur attend **PRIORITAIREMENT des OPÉRATIONS CONCRÈTES**
- **Séquence de restitution** :
  1. D'abord : opérations concrètes (Autorité Concurrence, Le Monde du Droit, Fusacq, CFNEWS)
  2. Ensuite : baromètres/études **seulement si publiés dans ou proche de la période demandée**
  3. En fin de synthèse : mention des baromètres attendus prochainement (ex: "Baromètre EY Q1 2026 attendu mi-mars")
- **Ne jamais remplacer** les opérations concrètes par des baromètres, mais les **compléter** avec du contexte macro si pertinent

**Séquence de recherche optimale (EXHAUSTIVE) :**

**PHASE 1 - Sources à flux quotidien (exploration exhaustive des pages sources)**
1. **Autorité de la Concurrence** :
   - URL directe : https://www.autoritedelaconcurrence.fr/fr/les-decisions-de-controle-des-concentrations
   - WebFetch pour extraire TOUTES les décisions DCC de la période
   - Capturer : nom opération, secteur, date décision

2. **Le Monde du Droit - Section Deals** :
   - URL directe : https://www.lemondedudroit.fr/deals
   - WebFetch pour extraire TOUS les deals de la période
   - Capturer : titre deal, cabinets conseils, date publication, type opération

3. **Fusacq - Page Buzz** :
   - URL directe : https://www.fusacq.com/buzz/fr
   - WebFetch pour extraire TOUTES les opérations de la période
   - Capturer : titre, montant si divulgué, secteur, date, type opération

4. **CFNEWS** :
   - Recherche web : site:cfnews.net "février 2026" M&A PME
   - Compléter par WebFetch des pages résultats si accessible

**PHASE 2 - Sources hebdomadaires/mensuelles (recherche ciblée)**
5. **Maddyness MaddyMoney** : recherche web + WebFetch de la page mensuelle si disponible
6. **FrenchWeb** : recherche web levées de fonds
7. **Les Échos** : recherche web M&A France PME
8. **L'AGEFI** : recherche web private equity / mid-market

**PHASE 3 - Sources complémentaires (si temps disponible)**
9. **Option Finance** : recherche web corporate finance
10. **Décideurs Magazine** : recherche web deals / palmarès
11. **Journal du Net** : recherche web levées start-up

**OBJECTIF QUALITÉ :**
- Viser **30-50 opérations concrètes minimum** pour une semaine de veille
- **100% des deals** doivent avoir leur montant indiqué (si divulgué) ou mentionner "non divulgué"
- Couverture minimale : **8 sources sur 11** (Phase 1 + Phase 2 obligatoires)

Pour chaque résultat, capturer : titre, date, source, URL, **montant**, secteur, type opération, résumé 3 lignes

### Étape 4 : Vérifier et Valider
- **Chaque lien** : vérifier qu'il pointe vers le bon contenu
- **Chaque date** : confirmer cohérence avec la période demandée
- **Chaque fait clé** : croiser avec au moins une autre source si possible
- **Marquer les incertitudes** : [à vérifier], [date approximative], [source payante]

### Étape 5 : Structurer la Restitution
Appliquer le format obligatoire (cf. instructions principales §3) :
```
### [Titre exact]
**Source :** [Nom] | **Date :** [JJ/MM/AAAA] | **Lien :** [URL]
[3 lignes de synthèse]
```

### Étape 6 : Contextualiser
- **En-tête** : nombre résultats, période, sources consultées
- **Corps** : opérations concrètes d'abord, puis baromètres/études si publiés dans la période
- **Pied de synthèse** :
  - Limites : sources inaccessibles, paywall, périmètre géographique
  - Suggestions complémentaires : sources alternatives, élargissement période
  - **Baromètres attendus** : mentionner les publications périodiques à venir avec leurs dates de sortie habituelles
    - Exemple : "Baromètre EY M&A France Q1 2026 attendu mi-avril 2026"
    - Exemple : "France Invest publie son baromètre semestriel fin juin 2026"
- Si pertinent : tendance identifiée, mise en perspective macro

### Étape 7 : Documenter pour Apprentissage
- Requête type nouvelle ? → `optimisations-decouvertes.md`
- Approche qui a bien fonctionné ? → `patterns-succes.md`
- Erreur rencontrée ? → `erreurs-frequentes.md`

## Fréquences de Veille Recommandées

| Fréquence | Type de veille | Sources principales |
|-----------|---------------|-------------------|
| Quotidienne | Opérations annoncées | CFNEWS, Les Échos, BODACC |
| Hebdomadaire | Tendances et analyses | L'AGEFI, Option Finance, Décideurs |
| Mensuelle | Levées de fonds | Maddyness MaddyMoney, FrenchWeb |
| Trimestrielle | Baromètres | EY, PwC MoneyTree |
| Semestrielle | Études de fond | France Invest + Grant Thornton, In Extenso |
| Annuelle | Bilans et perspectives | AMF rapport annuel, Bpifrance |

## Cas Particuliers

### Source Payante Inaccessible
→ Mentionner l'existence de la source, résumer ce qui est accessible gratuitement, indiquer la nécessité d'un abonnement

### Aucun Résultat Trouvé
→ Le signaler clairement, proposer d'élargir la période ou le périmètre, suggérer des sources alternatives

### Information Contradictoire entre Sources
→ Présenter les deux versions, indiquer la source la plus fiable selon le tier, laisser l'utilisateur trancher
