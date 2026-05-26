# MAbeautyplus CRM Dashboard

Dashboard CRM live connecté à Airtable — 5 centres, données en temps réel.

## 🚀 Déploiement

Ce projet est un fichier HTML unique (`index.html`) sans dépendances serveur.  
Il se déploie directement sur Netlify depuis GitHub.

## 📋 Prérequis

Un token Airtable avec accès à la base **CRM 2026** :
1. Aller sur [airtable.com/create/tokens](https://airtable.com/create/tokens)
2. Créer un token → Scope : `data.records:read` → Access : base `CRM 2026`
3. Coller le token dans l'interface au premier lancement

Le token est sauvegardé dans le `localStorage` du navigateur — aucun serveur ne le stocke.

## 🏗️ Structure

```
mabeautyplus-crm/
├── index.html      # Application complète (HTML + CSS + JS)
├── netlify.toml    # Config Netlify (headers sécurité, cache)
└── README.md       # Ce fichier
```

## 📊 Fonctionnalités

- **Dashboard** — KPIs globaux, 6 graphiques, filtres combinables
- **Prospects** — Tableau complet trié/filtré, pagination 50/page
- **Centres** — Performance par centre (conversion, bilans, sources)
- **Commerciaux** — Taux de conversion et bilans par commercial(e)
- **Sources & Annonces** — Croisement Meta Ads × CRM

## 🔄 Mise à jour des données

Cliquer sur **↻ Actualiser** dans la topbar pour resynchroniser avec Airtable.  
Les données se rechargent aussi automatiquement à chaque ouverture de l'app.

## 🛠️ Configuration Airtable

- Base ID : `appNML7rJEKiWkuVg`
- Table ID : `tblgCdNITlPy74Z5G` (Prospects Master)
