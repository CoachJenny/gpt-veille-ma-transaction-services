# GPT Veille M&A et Transaction Services - France PME/ETI

## Vue d'Ensemble

**Nom du projet :** gpt-veille-ma-transaction-services
**Version :** 1.0.0
**Date de création :** 2026-02-09
**Objectif :** GPT personnalisé expert en veille d'actualité, documentaire et presse sur le M&A et les transaction services en France, secteur PME/ETI

## Mission

Fournir des synthèses sourcées, datées et vérifiées à partir de plus de 30 sources d'autorité françaises, avec une politique de zéro hallucination et un format de restitution standardisé.

## Architecture du Projet

```
gpt-veille-ma-transaction-services/
├── instructions/
│   ├── instructions-gpt-principales.md    # Instructions core (5 534 car. < 7 500)
│   ├── prompt-systeme.md                  # Identité, ton, comportement
│   └── directives-securite.md             # Anti-hallucination, RGPD, limites
├── base-connaissances/
│   ├── concepts-fondamentaux/
│   │   ├── glossaire-ma.md                # 50+ termes M&A définis
│   │   ├── ecosysteme-ma-france.md        # Acteurs, tendances, dynamiques
│   │   └── sources-autorite-detaillees.md # Fiche détaillée par source
│   ├── procedures/
│   │   ├── methodologie-veille.md         # Workflow 7 étapes
│   │   └── workflow-analyse-operation.md  # Grille analyse opération
│   ├── meilleures-pratiques/
│   │   ├── qualite-sourcing.md            # Anti-hallucination, hiérarchie fiabilité
│   │   └── optimisation-recherche.md      # Mots-clés, stratégies par type
│   ├── depannage/
│   │   └── problemes-acces-sources.md     # 6 problèmes + solutions
│   └── ressources/
│       ├── liens-rss-api.md               # Répertoire RSS, API, alertes
│       └── templates-restitution.md       # 4 templates standardisés
├── exemples/
│   ├── conversations-exemples.md          # 5 exemples + anti-patterns
│   └── cas-utilisation.md                 # 5 personas détaillés
├── versions/
│   ├── changelog.md                       # Historique v1.0.0
│   ├── v1.0/                              # Archive version initiale
│   └── roadmap.md                         # Évolutions v1.1 à v2.0
├── metriques/
│   ├── kpi-performance.md                 # 8 KPIs avec cibles
│   ├── tests-validation.md                # 6 scénarios de test
│   └── feedback-utilisateurs.md           # Collecte retours
├── apprentissage-continu/
│   ├── patterns-succes.md                 # 3 patterns candidats
│   ├── erreurs-frequentes.md              # 6 erreurs documentées
│   ├── optimisations-decouvertes.md       # Framework d'optimisation
│   └── evolution-comportement.md          # Journal + boucle CAPTURE>ANALYSE>VALIDATION>INTÉGRATION>ÉVOLUTION
└── apercu-projet.md                       # Ce fichier
```

## Sources d'Autorité (30+)

| Tier | Catégorie | Nombre | Exemples |
|------|-----------|--------|----------|
| 1 | Régulateurs & Autorités | 6 | AMF, ACPR, Banque de France, Min. Économie, DG Trésor, INPI |
| 1 | Institutions Professionnelles | 4 | France Invest, Bpifrance, Ordre EC, CNCC |
| 1 | Bases de Données Publiques | 3 | BODACC, Pappers, data.gouv.fr |
| 2 | Médias Spécialisés M&A | 6 | CFNEWS, Les Échos, L'AGEFI, Option Finance, Décideurs, Fusacq |
| 2 | Médias Startups & Levées | 4 | Maddyness, FrenchWeb, JDN, La French Tech |
| 2 | Cabinets Audit/Conseil | 5 | Grant Thornton, EY, PwC, Deloitte, In Extenso Finance |

## Principes Fondamentaux

1. **Zéro hallucination** : jamais de lien, titre ou date inventés
2. **Vérification systématique** : chaque information sourcée et datée
3. **Format standardisé** : titre exact, source, date, lien, 3 lignes de synthèse
4. **Transparence** : signaler limites, paywall, incertitudes
5. **Amélioration continue** : auto-apprentissage via patterns, erreurs, optimisations

## Utilisation

### Pour le GPT
Copier le contenu de `instructions/instructions-gpt-principales.md` dans les instructions principales du GPT personnalisé. Télécharger les fichiers de `base-connaissances/` comme Knowledge Base.

### Pour l'Utilisateur
- Suivre les performances : `metriques/kpi-performance.md`
- Consulter les évolutions : `versions/changelog.md`
- Voir la feuille de route : `versions/roadmap.md`
- Suivre l'apprentissage : `apprentissage-continu/`

## Prochaines Étapes
Voir `versions/roadmap.md` pour les évolutions planifiées (v1.1 à v2.0).
