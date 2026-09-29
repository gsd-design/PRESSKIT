# Presskit Nolan GSD 2027 — site one-page

Site statique : un seul fichier `index.html`, les médias dans `assets/`, le PDF `presskit.pdf` à la racine.
Aucune étape de build : ce qui est dans ce dossier se met en ligne tel quel.

## Mettre en ligne sur Netlify (le plus rapide)

1. Va sur https://app.netlify.com/drop
2. Glisse le fichier `nolan-gsd-presskit.zip` dans la zone.
3. Netlify te donne une adresse du type `https://xxxx.netlify.app`. Tu peux la renommer dans *Site configuration → Change site name*.

## GitHub puis Netlify (pour mettre à jour facilement ensuite)

1. Sur GitHub, crée un dépôt (ex. `presskit-2027`), puis *Add file → Upload files* et glisse le contenu du zip décompressé (`index.html`, `assets/`, `presskit.pdf`, `netlify.toml`, `.gitignore`, `README.md`). Commit.
2. Sur Netlify : *Add new site → Import an existing project → GitHub*, choisis le dépôt.
   - Build command : laisser vide
   - Publish directory : `.` (déjà indiqué dans `netlify.toml`)
3. Chaque modification envoyée sur GitHub remet le site à jour automatiquement.

## Après la mise en ligne

- Dans `index.html`, remplace `https://VOTRE-DOMAINE` (balises `og:url` et `og:image`, en haut du fichier) par l'adresse réelle du site, pour que l'aperçu s'affiche quand tu partages le lien.
- Pour changer un texte, une photo ou le PDF, ouvre `index.html` : les zones à modifier sont signalées par des commentaires `MODIFIER ICI`.
