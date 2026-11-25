# Kink Jar

Site statique (un seul `index.html`), installable en PWA et utilisable hors-ligne.
Aucune donnée n'est envoyée : tout reste dans le navigateur (`localStorage`).

## Héberger sur GitHub Pages

1. Crée un dépôt GitHub (privé ou public) et envoie-y ces fichiers à la racine.
2. **Settings → Pages → Build and deployment → Source : Deploy from a branch**, branche `main`, dossier `/ (root)`.
3. Après ~1 min, le site est sur `https://<ton-user>.github.io/<nom-du-depot>/`.

> Un dépôt **privé** avec Pages nécessite un compte GitHub payant (Pro/Team). Sinon, le dépôt est public,
> mais le site contient `noindex` + `robots.txt` pour ne pas être référencé. L'URL reste accessible à qui la connaît.

## Mettre à jour
Modifie `index.html`, puis incrémente `CACHE` dans `sw.js` (ex. `kink-jar-v5-2`) pour que les appareils récupèrent la nouvelle version.
