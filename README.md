# Birdie ⛳ — version web (jouable sur iPhone, hors ligne)

Même jeu que l'app iOS, en HTML/JS pur (aucune dépendance) : vue 3D ou 2D, clubs, vent, éditeur de parcours, partage par lien.

## Héberger sur GitHub Pages
1. Créez un dépôt GitHub et déposez-y ces 5 fichiers **à la racine** : `index.html`, `sw.js`, `manifest.webmanifest`, `icon-192.png`, `icon-512.png`.
2. Dépôt ▸ **Settings ▸ Pages** ▸ *Deploy from a branch* ▸ `main` / `/ (root)` ▸ Save.
3. Après ~1 minute, ouvrez `https://<votre-compte>.github.io/<depot>/` dans **Safari** sur l'iPhone.
4. Bouton Partager ▸ **Sur l'écran d'accueil** : le jeu s'ouvre en plein écran comme une app et fonctionne **hors ligne** après la première visite.

## Partager un parcours
Bouton ⇪ : envoie un lien `…/#c=<code>`. En l'ouvrant, le destinataire reçoit le parcours dans sa liste (il peut aussi coller le lien via « Importer »).

## Notes
- Les parcours et records sont enregistrés sur l'appareil (localStorage).
- Après une mise à jour du code, changez `V='birdie-v1'` dans `sw.js` pour forcer le rafraîchissement du cache.
