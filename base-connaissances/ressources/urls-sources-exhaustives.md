---
titre: URLs Sources pour Veille Exhaustive
version: 1.0.0
derniere_maj: 2026-02-09
utilite: URLs directes pour exploration exhaustive via WebFetch
tags: [urls, sources, webfetch, exhaustivité]
---

# URLs Sources pour Veille Exhaustive M&A

## PHASE 1 - Exploration Exhaustive (WebFetch OBLIGATOIRE)

### Autorité de la Concurrence - Décisions DCC
- **URL directe** : https://www.autoritedelaconcurrence.fr/fr/les-decisions-de-controle-des-concentrations
- **Méthode** : WebFetch avec prompt "Extraire TOUTES les décisions de contrôle des concentrations (DCC) publiées entre [date début] et [date fin]. Pour chaque décision, donner : numéro décision, date, nom des entreprises concernées, secteur d'activité, type d'opération (acquisition, fusion, JV, etc.)"
- **Format attendu** : Liste exhaustive avec numéro décision, date, opération, secteur
- **Fréquence mise à jour** : Quotidienne
- **Avantages** : Source officielle, 0 paywall, exhaustivité garantie, granularité maximale

### Le Monde du Droit - Section Deals
- **URL directe** : https://www.lemondedudroit.fr/deals
- **Méthode** : WebFetch avec prompt "Extraire TOUS les deals publiés entre [date début] et [date fin]. Pour chaque deal, donner : titre, date publication, type opération (M&A, LBO, financement, JV), cabinets conseils mentionnés, lien URL"
- **Format attendu** : Liste exhaustive avec titre, date, cabinets, type, lien
- **Fréquence mise à jour** : Quotidienne
- **Avantages** : Angle cabinets conseils, valeur ajoutée TS (structuration juridique, earn-outs, garanties)

### Fusacq - Page Buzz
- **URL directe** : https://www.fusacq.com/buzz/fr
- **Méthode** : WebFetch avec prompt "Extraire TOUTES les opérations M&A publiées entre [date début] et [date fin]. Pour chaque opération, donner : titre, date publication, type opération, montant si divulgué (sinon indiquer 'non divulgué'), secteur, lien URL"
- **Format attendu** : Liste exhaustive avec titre, date, montant, secteur, lien
- **Fréquence mise à jour** : Quotidienne (plusieurs fois par jour)
- **Avantages** : Flux quotidien PME mid-market, marketplace cession-transmission, montants souvent divulgués

### CFNEWS
- **URL directe** : https://www.cfnews.net (section M&A)
- **Méthode** : WebSearch site:cfnews.net "[mois] 2026" M&A PME (paywall partiel, WebFetch si accessible)
- **Format attendu** : Titres + liens (contenu complet souvent derrière paywall)
- **Fréquence mise à jour** : Quotidienne
- **Avantages** : Base 57 000+ opérations, granularité M&A/LBO/venture/dette

## PHASE 2 - Recherche Ciblée (WebSearch + WebFetch sélectif)

### Maddyness - MaddyMoney
- **URL mensuelle** : https://www.maddyness.com/maddymoney (ex: /maddymoney-fevrier-2026)
- **Méthode** : WebSearch site:maddyness.com MaddyMoney "[mois] 2026" puis WebFetch de la page mensuelle
- **Format attendu** : Liste levées de fonds du mois avec montants, secteurs, investisseurs
- **Fréquence mise à jour** : Mensuelle (publiée entre le 5 et le 10 du mois suivant)
- **Avantages** : Exhaustivité levées start-up françaises, données structurées

### FrenchWeb
- **URL** : https://www.frenchweb.fr (section Levées de fonds)
- **Méthode** : WebSearch site:frenchweb.fr "levée de fonds" "[mois] 2026"
- **Format attendu** : Articles levées quotidiennes
- **Fréquence mise à jour** : Quotidienne
- **Avantages** : Couverture levées + mouvements investisseurs

### Les Échos
- **URL** : https://www.lesechos.fr (section Fusions-Acquisitions)
- **Méthode** : WebSearch site:lesechos.fr "fusion acquisition" France PME "[mois] 2026"
- **Format attendu** : Articles grandes opérations + décryptages
- **Fréquence mise à jour** : Quotidienne
- **Avantages** : Référence presse économique, contexte macro

### L'AGEFI
- **URL** : https://www.agefi.fr (section M&A / Private Equity)
- **Méthode** : WebSearch site:agefi.fr "private equity" "[mois] 2026"
- **Format attendu** : Articles M&A mid-market, PE, réglementaire
- **Fréquence mise à jour** : Quotidienne
- **Avantages** : Spécialisation finance, angle réglementaire

## PHASE 3 - Sources Additionnelles (Si Temps Disponible)

### Option Finance
- **URL** : https://www.optionfinance.fr
- **Méthode** : WebSearch site:optionfinance.fr "corporate finance" "[mois] 2026"
- **Fréquence mise à jour** : Hebdomadaire
- **Avantages** : Corporate finance, marchés capitaux

### Décideurs Magazine
- **URL** : https://www.magazine-decideurs.com
- **Méthode** : WebSearch site:magazine-decideurs.com M&A "[mois] 2026"
- **Fréquence mise à jour** : Hebdomadaire
- **Avantages** : Classements conseils M&A, palmarès fonds

### Journal du Net
- **URL** : https://www.journaldunet.com
- **Méthode** : WebSearch site:journaldunet.com start-up levée "[mois] 2026"
- **Fréquence mise à jour** : Quotidienne
- **Avantages** : Levées start-up, classements sectoriels

## Métriques d'Exhaustivité

### Objectifs Quantitatifs par Période
| Période | Opérations min. | Sources min. | Montants indiqués |
|---------|----------------|--------------|-------------------|
| 1 semaine | 30 | 8 | 100% |
| 2 semaines | 50 | 9 | 100% |
| 1 mois | 80 | 10 | 100% |

### Répartition Type par Source (ordre de grandeur)
| Source | Opérations attendues/semaine |
|--------|------------------------------|
| Autorité Concurrence | 5-10 décisions DCC |
| Le Monde du Droit | 8-15 deals |
| Fusacq | 15-25 opérations |
| CFNEWS | 5-10 opérations (accessibles) |
| Maddyness | 10-20 levées (mensuel) |
| Autres (FrenchWeb, Les Échos, L'AGEFI) | 5-10 |

### Contrôle Qualité
- **Avant restitution** : compter le nombre d'opérations extraites
- Si <30 pour une semaine → re-vérifier les pages sources (notamment Fusacq et Le Monde du Droit)
- Si montants manquants >10% → re-parcourir les sources pour compléter

## Notes d'Utilisation WebFetch

### Prompt Type pour WebFetch Exhaustif
```
Extraire TOUTES les opérations M&A/deals/décisions publiées entre le [JJ/MM/AAAA] et le [JJ/MM/AAAA].
Pour chaque opération, donner :
- Titre exact
- Date de publication
- Type d'opération (acquisition, cession, LBO, levée de fonds, JV, etc.)
- Montant (si divulgué, sinon indiquer "non divulgué")
- Secteur d'activité
- Lien URL vers l'article/décision

Présenter sous forme de liste exhaustive.
```

### Limites WebFetch
- Certaines pages avec pagination complexe peuvent nécessiter plusieurs appels
- Si WebFetch retourne "trop de résultats pour une seule page", segmenter par sous-période (ex: semaine 1, semaine 2)
- Paywall CFNEWS : extraire au minimum les titres + liens, indiquer [Abonnement requis] pour le contenu complet
