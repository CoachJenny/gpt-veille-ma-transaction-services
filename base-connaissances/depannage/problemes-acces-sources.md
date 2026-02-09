---
titre: Dépannage - Problèmes d'Accès aux Sources
version: 1.0.0
derniere_maj: 2026-02-09
utilisations: 0
efficacite: N/A
tags: [dépannage, accès, sources, paywall, erreurs]
---

# Dépannage - Problèmes d'Accès aux Sources

## Problème 1 : Source Derrière Paywall

### Symptôme
Impossible d'accéder au contenu complet (CFNEWS, Les Échos, L'AGEFI, Option Finance)

### Solutions
1. **Chercher le résumé gratuit** : la plupart des sites offrent un extrait/chapô
2. **Rechercher des reprises** : l'info a peut-être été reprise par une source gratuite
3. **Communiqué de presse** : chercher le CP de l'entreprise ou du fonds
4. **Cache moteur de recherche** : vérifier les snippets Google pour extraire des détails
5. **Signaler à l'utilisateur** : indiquer clairement la limite et suggérer l'abonnement

### Formulation
> "Cette information est publiée par [Source] (abonnement requis). Voici ce qui est accessible gratuitement : [extrait]. Pour l'article complet : [URL]"

## Problème 2 : Lien Mort ou Expiré

### Symptôme
URL retournant une erreur 404 ou redirigeant vers la page d'accueil

### Solutions
1. **Ne pas inventer de lien alternatif**
2. Chercher le même contenu via le titre exact dans un moteur de recherche
3. Vérifier si le contenu a été déplacé (changement de structure du site)
4. Utiliser la Wayback Machine (archive.org) si besoin historique
5. Signaler avec `[Lien potentiellement expiré - vérifier]`

## Problème 3 : Date Incohérente

### Symptôme
La date affichée ne correspond pas au contenu (article ancien mis à jour, ou date erronée)

### Solutions
1. Chercher la date dans le corps de l'article (souvent plus fiable que l'URL)
2. Croiser avec d'autres sources pour confirmer la chronologie
3. Vérifier la date du communiqué de presse original
4. Signaler avec `[Date à confirmer - vérification croisée recommandée]`

## Problème 4 : RSS/API Indisponible

### Symptôme
Le flux RSS ou l'API d'une source référencée ne répond pas

### Solutions
1. Vérifier si le flux a changé d'URL (fréquent lors de refontes de sites)
2. Consulter directement la page d'actualité du site
3. Utiliser la recherche par date sur le site
4. Documenter dans `erreurs-frequentes.md` pour suivi

## Problème 5 : Résultats Non Pertinents

### Symptôme
Les résultats retournés ne correspondent pas à la demande (mauvais secteur, mauvaise période, hors périmètre PME)

### Solutions
1. Affiner les mots-clés (cf. `meilleures-pratiques/optimisation-recherche.md`)
2. Ajouter des filtres de date explicites
3. Exclure les résultats hors périmètre dans la restitution
4. Reformuler la recherche avec des termes plus spécifiques
5. Demander clarification à l'utilisateur si l'ambiguïté persiste

## Problème 6 : Contradiction entre Sources

### Symptôme
Deux sources fiables donnent des informations contradictoires (montant, date, parties prenantes)

### Solutions
1. Identifier la source la plus proche de l'information primaire (CP vs article)
2. Vérifier les dates de publication (la plus récente peut avoir une correction)
3. Présenter les deux versions avec niveau de fiabilité respectif
4. Indiquer clairement la contradiction à l'utilisateur
5. Suggérer la source à privilégier avec justification
