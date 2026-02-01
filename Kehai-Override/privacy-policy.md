# Politique de Confidentialité - Kehai Override

**Dernière mise à jour** : 2024

## 🔒 Engagement en matière de confidentialité

**Kehai Override** est développé par **HellSoftware** avec un engagement fort envers la protection de votre vie privée. Cette extension est conçue pour fonctionner entièrement localement dans votre navigateur.

## 📊 Collecte de données

### ❌ Aucune collecte de données

**Kehai Override ne collecte, ne transmet, ni ne stocke aucune donnée personnelle ou de navigation en dehors de votre navigateur.**

- ✅ **Aucune télémétrie** : Aucune donnée d'utilisation n'est envoyée à des serveurs externes
- ✅ **Aucun tracking** : Aucun système de suivi ou d'analyse n'est intégré
- ✅ **Aucune connexion externe** : L'extension ne se connecte à aucun serveur distant
- ✅ **Traitement local uniquement** : Toutes les règles et configurations sont traitées localement

### 💾 Données stockées localement

L'extension stocke uniquement les données suivantes **localement dans votre navigateur** :

- **Règles de redirection** : Vos règles personnalisées
- **Règles de headers** : Vos configurations de modification d'en-têtes HTTP
- **Règles de mocks API** : Vos réponses API simulées
- **Règles d'injection** : Vos scripts JavaScript et CSS personnalisés
- **Profils et workspaces** : Vos organisations de règles
- **Paramètres de l'extension** : Vos préférences (activation/désactivation, etc.)

Ces données sont stockées via l'API `browser.storage` du navigateur :

- **Chrome** : `chrome.storage.sync` (avec fallback sur `chrome.storage.local`)
- **Firefox** : `browser.storage.sync` (avec fallback sur `browser.storage.local`)

Ces données restent **exclusivement sur votre machine** et ne sont jamais transmises à des tiers.

## 🔐 Permissions requises

L'extension demande les permissions suivantes pour fonctionner :

### `host_permissions: ['<all_urls>']`

**Pourquoi** : Nécessaire pour intercepter et modifier les requêtes HTTP/HTTPS sur tous les sites web selon vos règles.

**Ce que nous faisons** : Nous interceptons uniquement les requêtes que vous avez configurées dans vos règles. Aucune donnée n'est transmise en dehors de votre navigateur.

### `declarativeNetRequest`

**Pourquoi** : Utilisé pour les redirections et modifications de headers via l'API moderne Manifest V3.

**Ce que nous faisons** : Traitement local des règles sans transmission de données.

### `webRequest`

**Pourquoi** : Utilisé comme fallback pour les fonctionnalités avancées non supportées par Declarative Net Request.

**Ce que nous faisons** : Interception locale uniquement, aucune transmission.

### `storage`

**Pourquoi** : Nécessaire pour sauvegarder vos règles et configurations.

**Ce que nous faisons** : Stockage local uniquement dans votre navigateur.

### `scripting`

**Pourquoi** : Nécessaire pour injecter du code JavaScript/CSS personnalisé dans les pages selon vos règles.

**Ce que nous faisons** : Injection uniquement du code que vous avez défini, aucun code externe.

### `tabs` / `activeTab`

**Pourquoi** : Nécessaire pour ouvrir la page d'options depuis le popup.

**Ce que nous faisons** : Accès uniquement pour ouvrir l'interface de l'extension.

## 🌐 Synchronisation (Chrome uniquement)

Si vous utilisez Chrome et que la synchronisation Chrome est activée, vos règles peuvent être synchronisées entre vos appareils via `chrome.storage.sync`. Cette synchronisation est gérée par Chrome lui-même et suit la politique de confidentialité de Google.

## 🔄 Import/Export

L'extension permet d'exporter et d'importer vos configurations au format JSON. Ces fichiers sont gérés **uniquement par vous** et ne sont jamais transmis automatiquement.

## 📧 Contact

Si vous avez des questions concernant cette politique de confidentialité, vous pouvez nous contacter via :

- **Développeur** : Kehai Systems
- **Extension** : Kehai Override

## 📝 Modifications

Nous nous réservons le droit de modifier cette politique de confidentialité. Toute modification sera reflétée dans ce document avec une mise à jour de la date "Dernière mise à jour".

---

**En utilisant Kehai Override, vous acceptez cette politique de confidentialité.**

_"Le pouvoir d'altérer le Web"_ 😈
