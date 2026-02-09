---
derniere_maj: 2026-02-09
nombre_erreurs_documentees: 8
---

# Erreurs Fréquentes à Éviter

## Format d'Entrée

```markdown
### Erreur #[N] : [Nom Court]
- **Description** : [Ce qui se passe]
- **Cause racine** : [Pourquoi ça arrive]
- **Impact** : [Conséquence pour l'utilisateur]
- **Prévention** : [Comment l'éviter]
- **Détection** : [Comment la repérer]
- **Fréquence observée** : [Rare / Occasionnel / Fréquent]
- **Date identification** : [DATE]
```

## Erreurs Documentées

### Erreur #1 : Hallucination de Liens URL
- **Description** : Générer un lien URL par déduction ou construction logique au lieu de le vérifier
- **Cause racine** : Inférence du pattern d'URL d'un site sans vérification
- **Impact** : Critique - lien mort, perte de confiance utilisateur
- **Prévention** : Ne JAMAIS construire une URL. Toujours la vérifier avant restitution
- **Détection** : URL qui semble "trop propre" ou trop logiquement construite
- **Fréquence observée** : Fréquent (risque permanent)
- **Date identification** : 2026-02-09

### Erreur #2 : Confusion Date Publication vs Date Opération
- **Description** : Confondre la date de l'article avec la date réelle de l'opération M&A
- **Cause racine** : L'article peut être publié des jours/semaines après l'annonce réelle
- **Impact** : Élevé - chronologie incorrecte, confusion utilisateur
- **Prévention** : Toujours distinguer "date de publication de l'article" vs "date d'annonce de l'opération" vs "date de closing"
- **Détection** : Vérifier si l'article mentionne "annoncé le [date antérieure]"
- **Fréquence observée** : Fréquent
- **Date identification** : 2026-02-09

### Erreur #3 : Confusion Annonce vs Closing
- **Description** : Présenter une opération annoncée comme finalisée (ou inversement)
- **Cause racine** : Les médias annoncent souvent l'opération avant le closing effectif
- **Impact** : Modéré - information trompeuse sur le statut réel
- **Prévention** : Vérifier explicitement le statut (signing, approbation réglementaire, closing)
- **Détection** : Chercher les termes "sous réserve", "en cours", "signing", "closing attendu"
- **Fréquence observée** : Occasionnel
- **Date identification** : 2026-02-09

### Erreur #4 : Extrapolation de Montants
- **Description** : Estimer ou déduire un montant d'opération non divulgué
- **Cause racine** : Tentation de calculer via multiples sectoriels moyens
- **Impact** : Élevé - fausse information financière
- **Prévention** : Si le montant n'est pas publié, indiquer "non divulgué"
- **Détection** : Vérifier que chaque montant cité a une source explicite
- **Fréquence observée** : Occasionnel
- **Date identification** : 2026-02-09

### Erreur #5 : Mélange de Données Multi-Périodes
- **Description** : Mélanger des données de périodes différentes sans le signaler
- **Cause racine** : Études/baromètres avec des dates de couverture différentes de la date de publication
- **Impact** : Modéré - analyse biaisée, comparaisons invalides
- **Prévention** : Toujours indiquer la période couverte par chaque source, pas seulement la date de publication
- **Détection** : Vérifier les mentions "données à fin [date]" dans les études
- **Fréquence observée** : Occasionnel
- **Date identification** : 2026-02-09

### Erreur #6 : Omission de Limite d'Accès Paywall
- **Description** : Ne pas signaler qu'une source est derrière un paywall
- **Cause racine** : Oubli de mentionner la restriction d'accès
- **Impact** : Modéré - utilisateur clique et ne peut pas accéder au contenu
- **Prévention** : Systématiquement marquer les sources payantes avec [Abonnement requis]
- **Détection** : Vérifier si chaque source citée est en accès libre ou payant
- **Fréquence observée** : Fréquent (risque permanent)
- **Date identification** : 2026-02-09

### Erreur #7 : Encodage Unicode dans les TodoWrite
- **Description** : Les caractères accentués français (É, è, ê, etc.) s'affichent comme séquences d'échappement Unicode (\u00c9, \u00e8) dans les labels de tâches TodoWrite
- **Cause racine** : Passage de chaînes JSON avec échappement Unicode au lieu de texte UTF-8 natif dans les appels TodoWrite
- **Impact** : Faible fonctionnellement, mais donne une impression de manque de rigueur auprès de l'utilisateur
- **Prévention** : Toujours écrire les labels TodoWrite en texte brut sans accents problématiques, ou vérifier que les caractères accentués passent correctement
- **Détection** : Relire les labels de tâches affichés à l'utilisateur
- **Fréquence observée** : Observé 1 fois (session du 09/02/2026)
- **Date identification** : 2026-02-09

### Erreur #8 : Privilégier les Baromètres aux Opérations Concrètes
- **Description** : Répondre à une demande de veille périodique (ex: "veille du 1 au 5 février") avec des baromètres trimestriels/annuels (EY, Grant Thornton, France Invest) au lieu d'opérations PME concrètes quotidiennes
- **Cause racine** : Recherche web qui privilégie les contenus "informationnels" bien référencés SEO au lieu des flux d'actualité transactionnelle quotidienne (Fusacq, CFNEWS, Le Monde du Droit, Autorité Concurrence)
- **Impact** : Élevé - l'utilisateur attend des transactions opérationnelles exploitables, pas des tendances macro génériques
- **Prévention** : (1) Toujours commencer par Autorité Concurrence (DCC) + Le Monde du Droit + Fusacq + CFNEWS pour opérations concrètes, (2) Ajouter baromètres/études seulement si publiés dans ou proche de la période demandée (contexte macro complémentaire), (3) Mentionner en pied de synthèse les baromètres attendus dans les 4 semaines (consulter calendrier-publications-barometres.md)
- **Détection** : Comparer le ratio opérations concrètes vs baromètres. Si <50% d'opérations, revoir la stratégie de recherche
- **Fréquence observée** : Identifié 1 fois (comparaison ChatGPT session 09/02/2026)
- **Date identification** : 2026-02-09

---

*Section auto-alimentée. Chaque nouvelle erreur rencontrée en session est documentée ici pour prévention future.*
