# Instructions de Déploiement - YouTools Platform

## 🚀 Push vers GitHub depuis votre machine locale

### Étape 1 : Cloner le repository GitHub vide

```bash
# Sur votre machine locale
git clone git@github.com:geoffroydemarquet-art/youtools-platform.git
cd youtools-platform
```

### Étape 2 : Copier tous les fichiers du projet

Téléchargez tous les fichiers de ce projet et copiez-les dans le dossier `youtools-platform` que vous venez de cloner.

**Fichiers à copier** :
- Tous les fichiers et dossiers du projet
- Y compris les fichiers cachés (.gitignore, etc.)

### Étape 3 : Vérifier le statut Git

```bash
git status
```

Vous devriez voir tous les fichiers prêts à être committés.

### Étape 4 : Commit et Push

```bash
# Si des fichiers ne sont pas stagés, les ajouter
git add -A

# Les commits sont déjà faits, mais si nécessaire :
git commit -m "Initial commit - YouTools formation platform

Complete React + Tailwind CSS application for design training with:
- Photoshop tutorials and shortcuts
- Illustrator training modules  
- Midjourney prompt design guides
- AI agents integration
- Responsive design with glassmorphism effects
- Page transition animations
- SEO optimization and analytics

Ready for Netlify deployment.

Co-Authored-By: Claude Sonnet 4.5 <noreply@anthropic.com>"

# Push vers GitHub
git push origin main
```

## 🌐 Déployer sur Netlify

Une fois le code sur GitHub :

1. **Allez sur [app.netlify.com](https://app.netlify.com)**
2. Cliquez **"Add new site"** > **"Import an existing project"**
3. Sélectionnez **"Deploy with GitHub"**
4. Autorisez Netlify à accéder à votre compte GitHub
5. Sélectionnez le repository **"youtools-platform"**
6. **Les paramètres sont déjà configurés dans netlify.toml** :
   - Build command: `pnpm install && pnpm run build`
   - Publish directory: `dist`
   - Node version: 20
7. Cliquez **"Deploy site"**

## ⚡ Alternative : Deploy direct via Netlify CLI

Si vous préférez déployer directement sans passer par GitHub :

```bash
# Installer Netlify CLI (sur votre machine)
npm install -g netlify-cli

# Login à Netlify
netlify login

# Deploy depuis le dossier du projet
cd youtools-platform
netlify deploy --prod
```

Suivez les instructions à l'écran pour :
- Créer un nouveau site ou sélectionner un site existant
- Confirmer le build directory (dist)

## 📋 Checklist avant déploiement

✅ Tous les fichiers sont copiés dans le repository local
✅ Le fichier `netlify.toml` est présent
✅ Le fichier `.gitignore` est présent
✅ Les dépendances sont listées dans `package.json`
✅ La police Bodoni Moda est importée dans `src/styles/fonts.css`

## 🔧 Après le déploiement

Une fois déployé sur Netlify, vous pouvez :
- Configurer un domaine personnalisé
- Activer les formulaires Netlify
- Ajouter des variables d'environnement si nécessaire
- Configurer les notifications de déploiement

## 💡 Besoin d'aide ?

Si vous rencontrez des problèmes :
1. Vérifiez que tous les fichiers sont bien présents
2. Assurez-vous que `pnpm-lock.yaml` est inclus
3. Consultez les logs de build sur Netlify
4. Le fichier `netlify.toml` contient toute la configuration nécessaire

---

🎨 **Youtools © Demarquet**
Développé avec Claude Sonnet 4.5
