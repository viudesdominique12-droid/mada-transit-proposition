# Conception MADA Transit

Site de présentation client — proposition de conception du système de gestion
des opérations de transport, de la facturation et du suivi des créances
clients pour **MADA Transit SARL**.

Référence : **MT-CONC-01** · Version 1.0 · 19 octobre 2026
Stack cible : PostgreSQL + Django

## Contenu du site

Six pages statiques en HTML/CSS, pas de dépendances serveur, pas de JavaScript
externe. Fonctionne hors ligne (double-clic sur `index.html`).

| Fichier | Rôle |
|---|---|
| `index.html` | Page d'accueil — vue d'ensemble de la proposition |
| `comprendre.html` | Compréhension du métier — les trois réalités, les trois pièges |
| `design.html` | Architecture — les trois domaines bornés et le flux d'utilisation |
| `maquettes.html` | Maquettes des quatre écrans clés |
| `feuille-de-route.html` | Règles de gestion, rapports et étapes jusqu'à la mise en production |
| `contact.html` | Hypothèses à lever, équipe, formulaire de prise de rendez-vous |
| `styles.css` | Design system partagé |
| `presentation.html` | Redirection historique vers `index.html` |

## Déployer sur GitHub Pages (en 5 minutes)

### 1. Créer le dépôt
1. Allez sur <https://github.com/new>.
2. Nom suggéré : `mada-transit-proposition`.
3. Visibilité : **Public** (indispensable pour GitHub Pages gratuit).
4. Ne cochez rien d'autre, cliquez **Create repository**.

### 2. Importer les fichiers
1. Sur la nouvelle page du dépôt, cliquez sur **« uploading an existing file »**
   (lien dans le texte au centre).
2. Depuis l'explorateur Windows, ouvrez le dossier
   `C:\Users\…\Desktop\GMT Mada transit\`.
3. Sélectionnez tous les fichiers (`Ctrl+A`), glissez-déposez sur la zone
   d'import.
4. En bas, cliquez **Commit changes**.

### 3. Activer GitHub Pages
1. Dans le dépôt, allez dans **Settings → Pages** (menu latéral).
2. Section **Source** : choisissez **Deploy from a branch**.
3. **Branch** : `main`, dossier `/ (root)` → cliquez **Save**.
4. Patientez une à deux minutes. L'URL publique apparaît en haut de la page :

   ```
   https://<votre-pseudo>.github.io/mada-transit-proposition/
   ```

5. Testez l'URL dans votre navigateur. La page d'accueil s'affiche.

### 4. Partager
Envoyez simplement l'URL au client, par courriel ou messagerie. Le site est
public, pas besoin de compte, pas d'installation.

## Alternative rapide : Netlify Drop

Si vous préférez éviter GitHub, <https://app.netlify.com/drop> accepte un
glisser-déposer direct du dossier et fournit une URL en 30 secondes.
Pratique mais le lien est en `*.netlify.app`, moins personnalisable.

## Modifier le site plus tard

Toutes les pages sont du HTML modifiable à la main. Pour un changement rapide :
1. Modifiez le fichier concerné localement.
2. Sur GitHub, ouvrez le dépôt, cliquez sur le fichier à mettre à jour, cliquez
   sur l'icône crayon, collez le nouveau contenu, **Commit changes**.
3. GitHub Pages redéploie automatiquement en une minute.

## Notes importantes

- **Formulaire de contact** : visuel uniquement. Les données saisies ne sont
  envoyées nulle part. Pour recevoir réellement les demandes, intégrez un
  service comme [Formspree](https://formspree.io) (ligne à ajouter dans
  `contact.html`).
- **Mode sombre** : automatique selon le réglage du système du visiteur.
- **Responsive** : testé sur mobile (380 px), tablette et bureau.
