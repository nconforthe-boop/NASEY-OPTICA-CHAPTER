# NASEY OPTICA CHAPTER - Site Web Officiel

Bienvenue sur le dépôt du site web officiel du **NASEY OPTICA CHAPTER**, le chapitre étudiant OPTICA de l'École Nationale Supérieure Polytechnique de Yaoundé (ENSPY).

## 📋 Vue d'ensemble

Ce projet est un site web moderne et professionnel dédié à la promotion de l'optique et de la photonique. Le site est construit avec les technologies web les plus récentes et est facilement maintenable par l'équipe du chapitre.

### Caractéristiques principales

- ✨ **Design moderne et réactif** : Fonctionne parfaitement sur tous les appareils (mobile, tablette, ordinateur)
- 🎨 **Interface professionnelle** : Utilise Tailwind CSS et shadcn/ui pour une apparence soignée
- ⚡ **Performance optimale** : Construit avec Vite pour un chargement rapide
- 📱 **Accessible** : Respecte les normes d'accessibilité web (WCAG)
- 🔧 **Facile à maintenir** : Code bien structuré et documenté
- 🚀 **Déploiement automatique** : GitHub Actions gère le déploiement automatiquement

## 🌐 Sections du Site

Le site comprend les sections suivantes :

1. **Accueil** : Présentation du chapitre avec un appel à l'action
2. **À propos** : Informations détaillées sur la mission et les objectifs
3. **Le Bureau** : Présentation des membres du bureau et leurs rôles
4. **Nous Rejoindre** : Critères d'adhésion et avantages de l'adhésion
5. **Activités** : Activités régulières, à venir et archives
6. **Contact** : Formulaire de contact et informations de localisation

## 🛠️ Stack Technologique

| Technologie | Utilisation |
|-------------|------------|
| **React 19** | Framework JavaScript pour l'interface utilisateur |
| **TypeScript** | Langage typé pour une meilleure qualité de code |
| **Tailwind CSS 4** | Framework CSS utilitaire pour le styling |
| **shadcn/ui** | Composants UI réutilisables et accessibles |
| **Vite** | Bundler et serveur de développement ultra-rapide |
| **Wouter** | Routeur léger pour la navigation côté client |
| **GitHub Pages** | Hébergement gratuit et automatique |

## 📦 Installation et Configuration

### Prérequis

- Node.js 18+ installé sur votre ordinateur
- npm ou pnpm (gestionnaire de paquets)
- Git pour le contrôle de version

### Étapes d'installation

1. **Cloner le dépôt** :
```bash
git clone https://github.com/votre-nom-utilisateur/optica-chapter-website.git
cd optica-chapter-website
```

2. **Installer les dépendances** :
```bash
pnpm install
# ou
npm install
```

3. **Lancer le serveur de développement** :
```bash
pnpm dev
# ou
npm run dev
```

4. **Ouvrir dans le navigateur** :
Accédez à `http://localhost:3000` pour voir le site en développement.

## 🚀 Déploiement

### Déploiement automatique avec GitHub Pages

Le site se déploie automatiquement chaque fois que vous poussez des changements vers la branche `main` :

```bash
git add .
git commit -m "Description de vos changements"
git push origin main
```

GitHub Actions va automatiquement :
1. Installer les dépendances
2. Compiler le site
3. Déployer les fichiers sur GitHub Pages

Votre site sera accessible à : `https://[votre-nom-utilisateur].github.io/optica-chapter-website/`

### Build pour la production

Pour générer une version optimisée pour la production :

```bash
pnpm build
# ou
npm run build
```

Les fichiers compilés se trouveront dans le dossier `dist/`.

## 📝 Modification du Contenu

### Modifier la page d'accueil

Le contenu principal se trouve dans `client/src/pages/Home.tsx`. Vous pouvez modifier :

- Les textes et descriptions
- Les images (en mettant à jour les URLs)
- Les informations de contact
- Les membres du bureau

### Ajouter de nouvelles sections

1. Créez un nouveau fichier dans `client/src/pages/`
2. Créez les composants correspondants dans `client/src/components/`
3. Ajoutez la route dans `client/src/App.tsx`
4. Mettez à jour la navigation

### Modifier le style

- **Couleurs et thème** : Modifiez `client/src/index.css`
- **Composants** : Modifiez les fichiers dans `client/src/components/`
- **Tailwind** : Utilisez les classes Tailwind CSS directement dans le JSX

## 👥 Gestion des Collaborateurs

Pour ajouter des responsables de l'organisation :

1. Allez dans **Settings** → **Collaborators**
2. Cliquez sur **Add people**
3. Entrez le nom d'utilisateur GitHub
4. Sélectionnez le niveau de permission approprié

Pour plus de détails, consultez le [Guide de Déploiement GitHub Pages](./GITHUB_DEPLOYMENT_GUIDE.md).

## 📚 Structure du Projet

```
optica-chapter-website/
├── client/
│   ├── public/              # Fichiers statiques (favicon, robots.txt)
│   ├── src/
│   │   ├── pages/          # Pages du site
│   │   ├── components/     # Composants réutilisables
│   │   ├── contexts/       # Contextes React
│   │   ├── hooks/          # Hooks personnalisés
│   │   ├── lib/            # Utilitaires
│   │   ├── App.tsx         # Composant principal
│   │   ├── main.tsx        # Point d'entrée
│   │   └── index.css       # Styles globaux
│   └── index.html          # Template HTML
├── server/                 # Code serveur (Express)
├── shared/                 # Code partagé
├── package.json            # Dépendances du projet
├── vite.config.ts          # Configuration Vite
├── tsconfig.json           # Configuration TypeScript
├── GITHUB_DEPLOYMENT_GUIDE.md  # Guide de déploiement
└── README.md               # Ce fichier
```

## 🔧 Commandes Utiles

```bash
# Développement
pnpm dev              # Lancer le serveur de développement

# Build
pnpm build            # Compiler pour la production

# Preview
pnpm preview          # Prévisualiser la version de production

# Vérification
pnpm check            # Vérifier les types TypeScript

# Formatage
pnpm format           # Formater le code avec Prettier
```

## 🐛 Dépannage

### Le site ne se met pas à jour après un push

1. Vérifiez que GitHub Actions a réussi dans l'onglet **Actions**
2. Attendez 5-10 minutes pour que GitHub Pages se rafraîchisse
3. Videz le cache de votre navigateur

### Erreur lors du build

1. Allez dans **Actions** et cliquez sur le workflow échoué
2. Lisez le message d'erreur
3. Corrigez le problème et poussez à nouveau

Pour plus d'aide, consultez le [Guide de Déploiement](./GITHUB_DEPLOYMENT_GUIDE.md).

## 📧 Contact et Support

Pour toute question ou suggestion concernant le site :

- **Email** : conforthengoumegne@gmail.com
- **WhatsApp** : +237 657 770 957
- **Superviseur** : Dr. Mandeng Mandeng Lucien

## 📄 Licence

Ce projet est sous licence MIT. Vous êtes libre de l'utiliser, le modifier et le distribuer.

## 🙏 Remerciements

Merci à tous les membres du NASEY OPTICA CHAPTER qui contribuent au succès de ce projet !
---

**Dernière mise à jour** : Mars 2026 
**Responsable** : NASEY OPTICA CHAPTER - ENSPY
