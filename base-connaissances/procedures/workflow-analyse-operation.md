---
titre: Workflow d'Analyse d'une Opération M&A
version: 1.0.0
derniere_maj: 2026-02-09
utilisations: 0
efficacite: N/A
tags: [procédure, analyse, opération, M&A, due-diligence]
---

# Workflow d'Analyse d'une Opération M&A

## Grille d'Analyse Standard

Lorsqu'un utilisateur demande des détails sur une opération spécifique, collecter et structurer les informations suivantes :

### 1. Identification de l'Opération
- **Type** : acquisition, cession, LBO, MBO, MBI, build-up, carve-out, fusion
- **Cible** : nom, secteur, taille (CA, effectif, EBITDA si disponible)
- **Acquéreur** : nom, type (industriel, fonds PE, family office, management)
- **Vendeur** : nom, type, raison de la cession si connue
- **Date d'annonce** : JJ/MM/AAAA
- **Date de closing** : si disponible

### 2. Paramètres Financiers
- **Valorisation (EV)** : montant si public
- **Multiple implicite** : EV/EBITDA, EV/CA si calculable
- **Structure de financement** : equity/dette, type de dette
- **Complément de prix** : earn-out, conditions

### 3. Contexte Stratégique
- **Rationale acquéreur** : croissance externe, consolidation, diversification, intégration verticale
- **Positionnement dans le secteur** : part de marché, synergies identifiées
- **Historique** : opérations précédentes des parties prenantes

### 4. Conseils et Intermédiaires
- **Conseil M&A sell-side** : banque d'affaires
- **Conseil M&A buy-side** : banque d'affaires
- **Transaction services** : cabinet(s) de DD
- **Conseil juridique** : cabinet(s) d'avocats
- **Financement** : banque(s) arrangeur(s)

### 5. Aspects Réglementaires
- **Notification concentration** : oui/non, autorité compétente
- **Contrôle IEF** : si acquéreur étranger
- **Approbation sectorielle** : si secteur régulé (santé, finance, défense)

## Sources par Type d'Information

| Information | Source primaire | Source secondaire |
|-------------|---------------|-------------------|
| Annonce opération | CFNEWS, Les Échos | L'AGEFI, Décideurs |
| Données financières cible | Pappers, BODACC | Comptes déposés au greffe |
| Valorisation | CFNEWS (si publiée) | Communiqué de presse |
| Conseils mandatés | CFNEWS, Décideurs | LinkedIn (vérification) |
| Réglementaire | AMF, Autorité Concurrence | DG Trésor (IEF) |
| Contexte stratégique | Les Échos, L'AGEFI | Études France Invest |

## Template de Restitution Opération

```markdown
## [Nom Cible] - [Type Opération]

**Annonce :** [Date] | **Closing :** [Date ou "en cours"]
**Acquéreur :** [Nom] ([Type]) | **Vendeur :** [Nom] ([Type])
**Secteur :** [Secteur] | **Valorisation :** [Montant ou "non divulguée"]

### Synthèse
[3-5 lignes décrivant l'opération, son contexte et ses enjeux]

### Conseils Mandatés
- Sell-side : [Cabinet]
- Buy-side : [Cabinet]
- Transaction services : [Cabinet]
- Juridique : [Cabinet(s)]

### Sources
- [Source 1 - Titre - Date - Lien]
- [Source 2 - Titre - Date - Lien]
```
