# FX Immobilier — version de démonstration (V1)

Application mobile-first de suivi des mandats, visites, offres, compromis et relances.

## Démarrage rapide

Ouvrir `index.html` dans un navigateur, ou publier les fichiers sur GitHub Pages.

## Publication sur GitHub Pages

1. Créer un nouveau dépôt GitHub nommé `fx-immobilier-demo`, sans fichiers clients.
2. Ajouter tous les fichiers de ce dossier à la racine du dépôt (dont `index.html`).
3. Dans **Settings → Pages**, choisir **Deploy from a branch**, **main**, **/(root)** puis enregistrer.
4. Visiter le lien fourni par GitHub Pages depuis Chrome Android. Dans le menu Chrome, choisir **Installer l'application** ou **Ajouter à l'écran d'accueil**, selon l'affichage.

## Fonctionnalités

- Tableau de bord (mandats, visites à venir, offres à suivre, compromis signés, relances proches)
- Ajouter, modifier, supprimer des mandats, visites, offres, compromis, relances
- Rechercher, filtrer, marquer une relance comme terminée
- Exporter/importer une sauvegarde JSON manuelle
- Interface pensée pour smartphone et installation comme raccourci/application PWA depuis un site HTTPS
- Application statique sans service distant, avec cache hors ligne après première ouverture sur HTTPS

## IMPORTANT — confidentialité et limites

**Ceci est un prototype, pas un CRM de production.** Les informations sont stockées en clair dans `localStorage` sur le navigateur/appareil utilisé. Elles ne sont ni chiffrées, ni authentifiées, ni synchronisées. Elles peuvent disparaître si les données du navigateur sont effacées ou si le téléphone change.

N'entrer **aucune donnée personnelle réelle** (noms complets, numéros, emails de clients, données sensibles, pièces notariales ou d'identité). Utiliser des codes anonymisés lors des tests.

Une publication sur GitHub Pages donne accès publiquement à l'application et à son code, mais **pas au contenu de `localStorage` de chaque utilisateur**, qui reste dans son navigateur. Il ne faut jamais publier les sauvegardes JSON ni les dossiers réels dans le dépôt GitHub. Tout fichier ajouté au dépôt peut être accessible publiquement.

Pour un usage métier réel : prévoir authentification, stockage chiffré et sauvegardé côté serveur, contrôle d'accès, suppression/archivage, sécurité, conformité RGPD, rôles, droits, et une politique de traitement des données.

Les exemples préchargés, leurs montants, contacts et dates sont fictifs. Il n'y a **aucune connexion aux systèmes iad, WhatsApp, Gmail ou Google Calendar**. Les relances sont affichées à l'ouverture de l'application, sans notifications automatiques.

## Évolution recommandée

- V2 : authentification sécurisée + base PostgreSQL/Supabase avec politiques d'accès RLS, backups
- V3 : synchronisation calendrier autorisée, alertes, fiches prospects et droits d'accès

© Prototype personnel FX Immobilier. Aucun logo ou endorsement officiel iad.
