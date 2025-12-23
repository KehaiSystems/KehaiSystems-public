# 🔒 Politique de Confidentialité - Daemon Image Snatcher

**Dernière mise à jour** : 27 janvier 2025  
**Version de l'extension** : 1.0.0

---

## Collecte de Données

**Daemon Image Snatcher ne collecte, ne stocke, ni ne transmet aucune donnée personnelle.**

L'extension fonctionne entièrement en local dans votre navigateur. Aucune information n'est envoyée à des serveurs externes.

---

## Stockage Local

L'extension utilise le **stockage local du navigateur** uniquement pour :

- **Sauvegarder les images scannées** : Les URLs et métadonnées des images sont stockées localement pour améliorer les performances lors des scans répétés sur la même page
- **Limite de stockage** : Maximum 50 pages et 1000 images par page pour éviter le dépassement de quota
- **Nettoyage automatique** : Les anciennes entrées sont automatiquement supprimées (FIFO) lorsque la limite est atteinte

**Toutes les données restent sur votre appareil et ne sont jamais transmises.**

---

## Permissions Utilisées

Daemon Image Snatcher demande les permissions suivantes pour fonctionner :

### `activeTab`

**Utilisation** : Nécessaire pour scanner la page web actuellement active et extraire les images depuis le DOM.

**Données lues** : L'extension lit uniquement le contenu HTML/CSS de la page pour identifier les images. Aucune modification n'est apportée à la page.

### `downloads`

**Utilisation** : Nécessaire pour télécharger les images sélectionnées par l'utilisateur, individuellement ou en groupe (fichier ZIP).

**Action** : Aucun téléchargement automatique n'est effectué. Tous les téléchargements sont initiés explicitement par l'utilisateur.

### `storage`

**Utilisation** : Nécessaire pour sauvegarder localement les résultats des scans, améliorant les performances lors des scans répétés sur la même page.

**Données stockées** : URLs d'images, dimensions, formats, types. Aucune donnée personnelle n'est stockée.

**Toutes les données restent sur votre appareil. Aucune donnée n'est transmise à des serveurs externes.**

### `host_permissions: ['<all_urls>']`

**Utilisation** : Nécessaire pour permettre à l'utilisateur de scanner les images sur toutes les pages web qu'il visite.

**Action** : L'extension ne modifie pas les pages, elle lit uniquement le DOM pour extraire les URLs d'images.

**Important** : Cette permission est nécessaire pour que l'extension fonctionne sur tous les sites web. Aucune donnée n'est transmise à des serveurs externes.

---

## Cookies et Traçage

**Daemon Image Snatcher n'utilise aucun cookie et ne suit pas votre navigation.**

L'extension ne contient aucun code de suivi, analytics, ou publicité. Aucune information sur votre navigation n'est collectée ou transmise.

---

## Données Tiers

**L'extension ne communique avec aucun service tiers.**

Aucune API externe n'est appelée. Toutes les opérations (extraction, filtrage, téléchargement) sont effectuées localement dans votre navigateur.

---

## Sécurité

Daemon Image Snatcher prend la sécurité au sérieux :

- **Validation des URLs** : Toutes les URLs d'images sont validées avant traitement pour éviter les protocoles dangereux
- **Pas d'exécution de code** : L'extension ne télécharge ni n'exécute aucun code externe
- **Stockage sécurisé** : Les données sont stockées dans le stockage local sécurisé du navigateur
- **Content Security Policy** : L'extension utilise une CSP stricte pour prévenir les attaques XSS

---

## Modifications de cette Politique

Nous nous réservons le droit de modifier cette politique de confidentialité à tout moment. Toute modification sera reflétée par une mise à jour de la date "Dernière mise à jour" en haut de cette page.

En cas de modification substantielle, nous vous informerons via une mise à jour de l'extension ou une notification dans le Chrome Web Store / Firefox Add-ons.

---

## Vos Droits

Conformément au RGPD et aux lois sur la protection des données :

- **Droit d'accès** : Vous pouvez consulter toutes les données stockées localement via les outils de développement de votre navigateur
- **Droit de suppression** : Vous pouvez supprimer toutes les données en désinstallant l'extension ou en vidant le stockage local
- **Droit de portabilité** : Les données sont stockées localement et peuvent être exportées via les outils de développement

**Note** : Comme aucune donnée personnelle n'est collectée, ces droits s'appliquent uniquement aux données techniques stockées localement (URLs d'images, métadonnées).

---

## Contact

Pour toute question concernant cette politique de confidentialité ou le traitement de vos données, vous pouvez nous contacter :

- **Développeur** : HellTechnologies
- **Extension** : Daemon Image Snatcher
- **Version** : 1.0.0
- **Email** : HellTechnologies.dev@gmail.com

---

## Conformité

Cette politique de confidentialité est conforme aux exigences de :

- **RGPD** (Règlement Général sur la Protection des Données) - Union Européenne
- **CCPA** (California Consumer Privacy Act) - Californie, États-Unis
- **Chrome Web Store Policies** - Google
- **Firefox Add-on Policies** - Mozilla

---

© 2025 HellTechnologies - Daemon Image Snatcher

Cette politique de confidentialité est valable pour la version 1.0.0 et les versions ultérieures de l'extension.

