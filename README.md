# YouTools - Plateforme de Formation Design Graphique

Plateforme complète de formation professionnelle pour le design graphique, incluant des tutoriels pour Photoshop, Illustrator et Midjourney avec intégration d'agents IA.

## 🚀 Technologies

- **React 18.3.1** - Interface utilisateur moderne
- **Tailwind CSS v4** - Styling avec design glassmorphism
- **Vite 6.3.5** - Build tool ultra-rapide
- **TypeScript** - Type safety
- **Motion (Framer Motion)** - Animations fluides
- **Radix UI** - Composants accessibles

## 📦 Installation

```bash
# Installer pnpm si nécessaire
npm install -g pnpm

# Installer les dépendances
pnpm install

# Démarrer en développement
pnpm run dev

# Build pour production
pnpm run build
```

## 🌐 Déploiement sur Netlify

### Option 1: Via GitHub (Recommandé)

1. **Créer un repository GitHub:**
   - Allez sur [github.com](https://github.com) et créez un nouveau repository
   - Ne cochez PAS "Initialize with README"

2. **Pusher le code:**
   ```bash
   git remote add origin https://github.com/VOTRE-USERNAME/VOTRE-REPO.git
   git push -u origin main
   ```

3. **Connecter à Netlify:**
   - Allez sur [netlify.com](https://netlify.com) et connectez-vous
   - Cliquez "Add new site" > "Import an existing project"
   - Sélectionnez GitHub et autorisez l'accès
   - Choisissez votre repository
   - Les paramètres de build sont déjà configurés dans `netlify.toml`
   - Cliquez "Deploy site"

### Option 2: Via Netlify CLI

```bash
# Installer Netlify CLI
npm install -g netlify-cli

# Login
netlify login

# Déployer
netlify deploy --prod
```

## ✨ Fonctionnalités

- 📚 **Modules de Formation**
  - Photoshop: 50+ raccourcis Mac, glossaire, 11 tutoriels vidéo
  - Illustrator: 40+ raccourcis, techniques avancées
  - Midjourney: 230+ astuces de prompt design

- 🤖 **Agents IA**
  - PROF - Expert design graphique
  - TENDANCES GRAPHIQUES - Veille créative
  - MARKETING - Stratégies créatives
  - NANO BANANA - Assistant créatif
  - NAMING - Génération de noms

- 🎨 **Design**
  - Effets glassmorphism
  - Transitions de page avec flou
  - Animations staggered pour les éléments
  - Design responsive mobile-first
  - Vidéos de fond dynamiques

- 🔐 **Authentification**
  - Système de login sécurisé
  - Protection des pages

- 📊 **SEO & Analytics**
  - Google Analytics intégré
  - Web Vitals tracking
  - Sitemap XML
  - Meta tags optimisés

## 📁 Structure du Projet

```
src/
├── app/
│   ├── App.tsx                 # Application principale
│   ├── components/
│   │   ├── HomePage.tsx        # Page d'accueil
│   │   ├── PhotoshopPage.tsx   # Module Photoshop
│   │   ├── IllustratorPage.tsx # Module Illustrator
│   │   ├── MidjourneyPage.tsx  # Module Midjourney
│   │   ├── AIAssistantPage.tsx # Agents IA
│   │   ├── ProgrammePage.tsx   # Programme de formation
│   │   └── ui/                 # Composants UI réutilisables
│   └── public/                 # Assets statiques
└── styles/
    ├── globals.css             # Styles globaux & animations
    ├── fonts.css               # Import fonts (Bodoni Moda)
    └── index.css               # Point d'entrée Tailwind
```

## 🎯 Configuration

### Variables d'environnement (optionnel)

Créez un fichier `.env` pour les variables d'environnement:

```env
VITE_GA_TRACKING_ID=your-google-analytics-id
```

### Build Configuration

Le fichier `netlify.toml` contient:
- Command de build: `pnpm install && pnpm run build`
- Répertoire de publication: `dist`
- Redirections SPA configurées
- Node version: 20

## 🔧 Scripts Disponibles

```bash
pnpm run dev      # Développement local
pnpm run build    # Build production
pnpm run preview  # Prévisualiser le build
```

## 📝 Notes de Développement

- **Framework**: Application React SPA (Single Page Application)
- **Router**: Navigation interne sans React Router
- **Styling**: Tailwind CSS v4 avec thème personnalisé
- **Animations**: CSS animations + Motion pour les interactions
- **Fonts**: Bodoni Moda (Google Fonts)

## 🌟 Crédits

Développé avec l'assistance de Claude Sonnet 4.5

© Youtools - Demarquet
