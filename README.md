# PolitiCompare 2027

Application web React + Vite, responsive, sans backend, prête pour Vercel.

## Fonctionnalités

- Face-à-face de 13 personnalités sur 8 thématiques
- Exploration qualitative des 8 axes PolitiScales
- Fiches individuelles, recherche et filtre par famille politique
- URL partageable qui conserve les sélections
- Impression et export PDF via le navigateur
- Sources de vérification et méthodologie

## Démarrer en local

Installer Node.js 20.19+ ou 22.12+.

```bash
npm install
npm run dev
```

Ouvrir l'adresse affichée (généralement http://localhost:5173).

## Déployer sur Vercel

1. Créer un dépôt GitHub et y déposer le contenu de ce dossier.
2. Sur https://vercel.com/new, sélectionner « Import Git Repository ».
3. Vercel détecte Vite automatiquement. Paramètres : framework **Vite**, commande de build `npm run build`, dossier de sortie `dist`.
4. Cliquer sur **Deploy**. Un lien public `*.vercel.app` est créé.

Alternative : installer Vercel CLI, puis lancer `npx vercel` depuis ce dossier et suivre les instructions.

## Mettre à jour les contenus

Modifier `src/data.js` : tableaux `raw`, `axes`, `topics`, `updated`. Puis `npm run build` pour vérifier, et pousser les modifications sur GitHub (redéploiement automatique avec Vercel).

**Important** : les fiches sont des résumés éditoriaux indicatifs. Les sources proposées permettent un contrôle externe mais ne constituent pas des preuves individualisées pour chaque phrase. Avant une diffusion publique importante, ajouter des références primaires datées à chaque proposition, un historique des changements et un processus de vérification humaine. Ne pas présenter ces résumés comme des programmes officiels 2027.

## Technique

React 18, Vite 6, lucide-react. Pas de clé API, pas de base de données, pas de cookies analytiques. Google Fonts nécessite une connexion internet (polices de repli disponibles).
