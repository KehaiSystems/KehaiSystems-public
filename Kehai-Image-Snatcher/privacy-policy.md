# 🔒 Privacy Policy - Kehai Image Snatcher

**Last updated** : January 27, 2025  
**Extension version** : 1.3.0

---

## Data Collection

**Kehai Image Snatcher does not collect, store, or transmit any personal data.**

The extension operates entirely locally in your browser. No information is sent to external servers.

---

## Local Storage

The extension uses **browser local storage** only for:

- **Saving scanned images** : Image URLs and metadata are stored locally to improve performance during repeated scans on the same page
- **Storage limit** : Maximum 50 pages and 1000 images per page to avoid quota overflow
- **Automatic cleanup** : Old entries are automatically deleted (FIFO) when the limit is reached

**All data remains on your device and is never transmitted.**

---

## Permissions Used

Kehai Image Snatcher requests the following permissions to function:

### `activeTab`

**Usage** : Required to scan the currently active web page and extract images from the DOM.

**Data read** : The extension only reads the HTML/CSS content of the page to identify images. No modifications are made to the page.

### `downloads`

**Usage** : Required to download images selected by the user, individually or in groups (ZIP file).

**Action** : No automatic downloads are performed. All downloads are explicitly initiated by the user.

### `storage`

**Usage** : Required to locally save scan results, improving performance during repeated scans on the same page.

**Data stored** : Image URLs, dimensions, formats, types. No personal data is stored.

**All data remains on your device. No data is transmitted to external servers.**

### `host_permissions: ['<all_urls>']`

**Usage** : Required to allow the user to scan images on all web pages they visit.

**Action** : The extension does not modify pages, it only reads the DOM to extract image URLs.

**Important** : This permission is necessary for the extension to work on all websites. No data is transmitted to external servers.

---

## Cookies and Tracking

**Kehai Image Snatcher does not use any cookies and does not track your browsing.**

The extension contains no tracking code, analytics, or advertising. No information about your browsing is collected or transmitted.

---

## Third-Party Data

**The extension does not communicate with any third-party services.**

No external APIs are called. All operations (extraction, filtering, downloading) are performed locally in your browser.

---

## Security

Kehai Image Snatcher takes security seriously:

- **URL validation** : All image URLs are validated before processing to avoid dangerous protocols
- **No code execution** : The extension does not download or execute any external code
- **Secure storage** : Data is stored in the browser's secure local storage
- **Content Security Policy** : The extension uses a strict CSP to prevent XSS attacks

---

## Changes to this Policy

We reserve the right to modify this privacy policy at any time. Any changes will be reflected by updating the "Last updated" date at the top of this page.

In case of substantial changes, we will inform you via an extension update or a notification in the Chrome Web Store / Firefox Add-ons.

---

## Your Rights

In accordance with GDPR and data protection laws:

- **Right of access** : You can view all locally stored data via your browser's developer tools
- **Right to deletion** : You can delete all data by uninstalling the extension or clearing local storage
- **Right to portability** : Data is stored locally and can be exported via developer tools

**Note** : Since no personal data is collected, these rights apply only to technical data stored locally (image URLs, metadata).

---

## Contact

For any questions regarding this privacy policy or the processing of your data, you can contact us:

- **Developer** : Kehai Systems
- **Extension** : Kehai Image Snatcher
- **Version** : 1.3.0

---

## Compliance

This privacy policy complies with the requirements of:

- **GDPR** (General Data Protection Regulation) - European Union
- **CCPA** (California Consumer Privacy Act) - California, United States
- **Chrome Web Store Policies** - Google
- **Firefox Add-on Policies** - Mozilla

---

© 2025 Kehai Systems - Kehai Image Snatcher

This privacy policy is valid for version 1.3.0 and subsequent versions of the extension.
