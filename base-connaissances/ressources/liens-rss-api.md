---
titre: Répertoire des Flux RSS et API Disponibles
version: 1.0.0
derniere_maj: 2026-02-09
utilisations: 0
efficacite: N/A
tags: [ressources, RSS, API, flux, automatisation, veille]
---

# Répertoire des Flux RSS et API

## Flux RSS Disponibles

### Régulateurs
| Source | URL RSS | Fréquence | Statut |
|--------|---------|-----------|--------|
| AMF - Communiqués | amf-france.org/rss | Quotidien | Actif |
| AMF - Doctrine | amf-france.org/rss (catégorie) | Variable | Actif |
| ACPR | acpr.banque-france.fr/rss | Variable | Actif |
| Min. Économie | economie.gouv.fr/rss | Quotidien | Actif |

### Médias Spécialisés
| Source | Flux | Fréquence | Accès |
|--------|------|-----------|-------|
| CFNEWS - M&A | Par rubrique | Quotidien | Abonnés |
| CFNEWS - PE | Par rubrique | Quotidien | Abonnés |
| CFNEWS - VC | Par rubrique | Quotidien | Abonnés |
| CFNEWS - Dette | Par rubrique | Quotidien | Abonnés |
| Maddyness | maddyness.com/feed | Quotidien | Gratuit |
| FrenchWeb | frenchweb.fr/feed | Quotidien | Gratuit |
| Bpifrance Le Hub | lehub.bpifrance.fr/feed | Variable | Gratuit |

## API Publiques

### BODACC
- **Endpoint** : API REST publique
- **Authentification** : Aucune requise
- **Données** : Annonces légales (cessions, modifications capital, procédures collectives)
- **Format** : JSON
- **Limite** : Pas de limite documentée
- **Documentation** : bodacc.fr/pages/api

### Pappers
- **Endpoint** : api.pappers.fr
- **Authentification** : Clé API (inscription gratuite)
- **Données** : Entreprises, dirigeants, comptes annuels, bénéficiaires effectifs
- **Format** : JSON
- **Limite gratuite** : 100 crédits/mois
- **Plans payants** : À partir de 30€/mois
- **Documentation** : pappers.fr/api

### INPI - Données Entreprises
- **Endpoint** : API données INPI
- **Authentification** : Inscription requise
- **Données** : Registre RBE, marques, brevets
- **Format** : JSON
- **Documentation** : data.inpi.fr

### data.gouv.fr - SIRENE
- **Endpoint** : API SIRENE (INSEE)
- **Authentification** : Token gratuit
- **Données** : Base SIRENE complète (établissements, entreprises)
- **Format** : JSON
- **Documentation** : api.insee.fr/catalogue

## Alertes Email Configurables

| Source | Type d'alerte | Configuration |
|--------|--------------|---------------|
| BODACC | Annonces par critère (secteur, zone, type) | bodacc.fr → Créer une alerte |
| AMF | Communiqués par catégorie | amf-france.org → Newsletter |
| Pappers | Surveillance entreprise | pappers.fr → Alertes (payant) |
| Google Alerts | Mots-clés M&A | google.com/alerts |
| CFNEWS | Newsletter quotidienne | cfnews.net (abonnés) |

## Calendrier des Publications Récurrentes

| Publication | Éditeur | Fréquence | Période couverte | Mois publication |
|------------|---------|-----------|------------------|-----------------|
| Baromètre Capital-Investissement | France Invest + Grant Thornton | Semestriel | S1/S2 | Mars / Septembre |
| Baromètre Transactions | EY | Trimestriel | T1-T4 | Après chaque trimestre |
| MoneyTree | PwC + France Invest | Trimestriel | T1-T4 | Après chaque trimestre |
| MaddyMoney | Maddyness | Mensuel | Mois M | M+1 |
| Panorama PME | In Extenso + Epsilon | Semestriel | S1/S2 | Variable |
| Rapport annuel marché | AMF | Annuel | Année N | Avril N+1 |
