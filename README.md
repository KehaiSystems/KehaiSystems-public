# Kehai-Systems-public

Ce dépôt contient tous les documents publics des produits Kehai Systems, notamment les politiques de confidentialité et autres informations légales.

## 🌐 Accès en ligne

Les documents sont accessibles via la page d'index principale : **`index.html`**

Cette page liste tous les produits Kehai Systems et leurs documents disponibles, avec un design moderne et responsive.

## 📁 Structure du projet

```
Kehai-Systems-public/
├── index.html              # Page d'index principale
├── products.json           # Configuration des produits et documents
├── README.md              # Ce fichier
└── [Nom-du-Produit]/      # Dossier pour chaque produit
    ├── privacy-policy.html
    ├── privacy-policy.md
    └── ... (autres documents)
```

## ➕ Ajouter un nouveau produit

Pour ajouter un nouveau produit et ses documents :

### 1. Créer le dossier du produit

Créez un nouveau dossier à la racine avec le nom de votre produit :
```
[Nom-du-Produit]/
```

### 2. Ajouter les documents

Placez vos documents (HTML, Markdown, PDF, etc.) dans ce dossier :
```
[Nom-du-Produit]/
├── privacy-policy.html
├── privacy-policy.md
└── autres-documents.pdf
```

### 3. Mettre à jour `products.json`

Ajoutez votre produit dans le fichier `products.json` :

```json
{
  "products": [
    {
      "name": "Nom du Produit",
      "description": "Description courte du produit",
      "documents": [
        {
          "name": "Nom affiché du document",
          "url": "Nom-du-Produit/privacy-policy.html",
          "type": "privacy-policy"
        },
        {
          "name": "Autre document",
          "url": "Nom-du-Produit/autre-document.md",
          "type": "other"
        }
      ]
    }
  ]
}
```

### Exemple complet

```json
{
  "products": [
    {
      "name": "Mon Nouveau Produit",
      "description": "Description de mon nouveau produit",
      "documents": [
        {
          "name": "Politique de Confidentialité",
          "url": "Mon-Nouveau-Produit/privacy-policy.html",
          "type": "privacy-policy"
        },
        {
          "name": "Conditions d'utilisation",
          "url": "Mon-Nouveau-Produit/terms.html",
          "type": "terms"
        }
      ]
    }
  ]
}
```

## 🎨 Personnalisation

Le design de `index.html` utilise un thème sombre avec les couleurs Kehai Systems :
- **Cyan** (`#00ced1`) : Couleur principale
- **Rouge** (`#dc143c`) : Couleur d'accent
- **Fond sombre** : Pour un look moderne

Vous pouvez modifier les styles CSS dans `index.html` pour personnaliser l'apparence.

## 📝 Types de documents supportés

- **HTML** (`.html`) : Documents formatés avec style
- **Markdown** (`.md`) : Documents en format Markdown
- **PDF** (`.pdf`) : Documents PDF
- Tout autre format de fichier accessible via le navigateur

## 🔗 Liens relatifs

Tous les liens dans `products.json` doivent être **relatifs** à la racine du projet. Par exemple :
- ✅ `Kehai-Image-Snatcher/privacy-policy.html`
- ❌ `/Kehai-Image-Snatcher/privacy-policy.html`
- ❌ `https://example.com/privacy-policy.html`

## 🚀 Déploiement sur GitHub Pages

### Méthode 1 : Via l'interface GitHub (Recommandé)

1. **Pousser votre code sur GitHub**
   ```bash
   git add .
   git commit -m "Initial commit - Site Kehai Systems"
   git push origin main
   ```

2. **Activer GitHub Pages**
   - Allez sur votre dépôt GitHub
   - Cliquez sur **Settings** (Paramètres)
   - Dans le menu de gauche, cliquez sur **Pages**
   - Sous **Source**, sélectionnez :
     - **Branch** : `main` (ou `master`)
     - **Folder** : `/ (root)`
   - Cliquez sur **Save** (Enregistrer)

3. **Attendre le déploiement**
   - GitHub va déployer votre site (cela peut prendre 1-2 minutes)
   - Une fois prêt, vous verrez l'URL de votre site : `https://[votre-username].github.io/Kehai-Systems-public/`
   - Vous pouvez aussi utiliser un domaine personnalisé si vous en avez un

### Méthode 2 : Via GitHub Actions (Automatique)

Si vous voulez un déploiement automatique à chaque push, créez le fichier `.github/workflows/deploy.yml` :

```yaml
name: Deploy to GitHub Pages

on:
  push:
    branches:
      - main

permissions:
  contents: read
  pages: write
  id-token: write

jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - name: Setup Pages
        uses: actions/configure-pages@v3
      - name: Upload artifact
        uses: actions/upload-pages-artifact@v2
        with:
          path: '.'
      - name: Deploy to GitHub Pages
        id: deployment
        uses: actions/deploy-pages@v2
```

### Vérification

Une fois déployé, votre site sera accessible à :
- `https://[votre-username].github.io/Kehai-Systems-public/`
- Ou avec un domaine personnalisé si configuré

### ⚠️ Notes importantes

- Le fichier `.nojekyll` est déjà présent pour désactiver Jekyll (nécessaire pour servir les fichiers HTML statiques)
- Assurez-vous que `index.html` est à la racine du dépôt
- Les liens dans `products.json` doivent être relatifs (sans `/` au début)
- Les modifications peuvent prendre quelques minutes à apparaître en ligne

## 🌐 Autres options de déploiement

Ce dépôt peut aussi être déployé sur :
- **Netlify** : Déployez directement depuis GitHub (drag & drop ou Git)
- **Vercel** : Déployez avec un simple `git push`
- **Cloudflare Pages** : Importez depuis GitHub
- Tout autre service d'hébergement statique

## 📄 Produits actuels

- **Kehai Image Snatcher** : Extension Chrome et Firefox pour scanner et télécharger des images

---

© 2026 Kehai Systems - Tous droits réservés
