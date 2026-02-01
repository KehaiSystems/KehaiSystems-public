# 📖 Guide complet : Mettre en ligne sur GitHub Pages

Ce guide vous explique étape par étape comment mettre en ligne votre site Kehai Systems sur GitHub Pages.

## 📋 Prérequis

- Un compte GitHub
- Le dépôt `Kehai-Systems-public` créé sur GitHub
- Git installé sur votre machine

## 🚀 Étapes de déploiement

### Étape 1 : Préparer votre dépôt local

Assurez-vous que tous vos fichiers sont prêts :

```bash
# Vérifier les fichiers présents
ls -la

# Vous devriez voir :
# - index.html
# - products.json
# - README.md
# - .nojekyll
# - Kehai-Image-Snatcher/
```

### Étape 2 : Initialiser Git (si pas déjà fait)

```bash
# Si le dépôt n'est pas encore un dépôt Git
git init
git add .
git commit -m "Initial commit - Site Kehai Systems public"
```

### Étape 3 : Connecter à GitHub

```bash
# Ajouter le dépôt distant (remplacez par votre URL)
git remote add origin https://github.com/[votre-username]/Kehai-Systems-public.git

# Pousser le code
git branch -M main
git push -u origin main
```

### Étape 4 : Activer GitHub Pages

1. **Ouvrez votre navigateur** et allez sur votre dépôt GitHub :
   `https://github.com/[votre-username]/Kehai-Systems-public`

2. **Cliquez sur "Settings"** (Paramètres) en haut du dépôt

3. **Dans le menu de gauche**, cliquez sur **"Pages"**

4. **Configurez la source** :
   - **Source** : Sélectionnez `Deploy from a branch`
   - **Branch** : Choisissez `main` (ou `master`)
   - **Folder** : Sélectionnez `/ (root)`
   - Cliquez sur **"Save"** (Enregistrer)

5. **Attendez le déploiement** :
   - GitHub va afficher un message "Your site is being built"
   - Après 1-2 minutes, vous verrez : "Your site is live at..."
   - L'URL sera : `https://[votre-username].github.io/Kehai-Systems-public/`

### Étape 5 : Vérifier votre site

1. Cliquez sur l'URL fournie par GitHub
2. Vérifiez que la page d'index s'affiche correctement
3. Testez les liens vers les documents

## 🔄 Mettre à jour le site

Chaque fois que vous modifiez des fichiers :

```bash
git add .
git commit -m "Description de vos modifications"
git push origin main
```

GitHub Pages se mettra à jour automatiquement en quelques minutes.

## 🌍 Utiliser un domaine personnalisé (Optionnel)

Si vous avez un domaine (ex: `kehaisystems.com`) :

1. Dans **Settings > Pages**, ajoutez votre domaine dans **Custom domain**
2. Configurez un enregistrement DNS CNAME pointant vers `[votre-username].github.io`
3. GitHub générera un fichier `CNAME` automatiquement

## ✅ Checklist de vérification

- [ ] Tous les fichiers sont poussés sur GitHub
- [ ] GitHub Pages est activé dans les paramètres
- [ ] La branche `main` est sélectionnée comme source
- [ ] Le dossier racine `/` est sélectionné
- [ ] Le site est accessible via l'URL GitHub Pages
- [ ] Les liens vers les documents fonctionnent
- [ ] Le fichier `.nojekyll` est présent (déjà créé)

## 🐛 Résolution de problèmes

### Le site ne s'affiche pas

- Vérifiez que GitHub Pages est bien activé
- Attendez 5-10 minutes (le premier déploiement peut prendre du temps)
- Vérifiez l'onglet **Actions** pour voir s'il y a des erreurs de build

### Les liens ne fonctionnent pas

- Vérifiez que les chemins dans `products.json` sont relatifs (sans `/` au début)
- Vérifiez que les fichiers existent bien dans les dossiers

### Erreur 404

- Assurez-vous que `index.html` est bien à la racine
- Vérifiez que le fichier `.nojekyll` est présent

## 📞 Support

Si vous rencontrez des problèmes, consultez la [documentation officielle de GitHub Pages](https://docs.github.com/en/pages).

---

**Votre site sera accessible à :**
`https://[votre-username].github.io/Kehai-Systems-public/`






