# Site Nolan GSD — nolangsd.fr

Site statique, sans étape de build : ce qui est dans ce dossier se met en ligne tel quel.

| Adresse | Fichier | Contenu |
|---|---|---|
| `nolangsd.fr` | `index.html` | Accueil : prochains concerts, vidéos, merch, contact |
| `nolangsd.fr/presskit` | `presskit/index.html` | Presskit 2027 pour les festivals et programmateurs |
| `nolangsd.fr/presskit.pdf` | `presskit.pdf` | Le presskit en PDF |

Les médias (photos, vidéo, police, bords déchirés) sont dans `assets/` et servent aux deux pages.

## Modifier le contenu

Ouvre le fichier de la page concernée : les zones à modifier sont signalées par des commentaires `MODIFIER ICI`.

- **Ajouter une date de concert** : dans `index.html`, section « PROCHAINS CONCERTS ». Le modèle d'une ligne de date est dans le commentaire juste au-dessus.
- **Ouvrir le merch** : dans `index.html`, section « MERCH », remplacer le bloc « Bientôt disponible » par les articles et le lien de la boutique.
- **Presskit** : `presskit/index.html` (bio, festivals, galerie, presse, contact).

## Mise en ligne

Le site est hébergé sur Netlify (`presskitnolangsd.netlify.app`), avec le domaine `nolangsd.fr` (zone DNS chez OVH).
Le code est sur GitHub : `gsd-design/PRESSKIT`. Chaque modification envoyée sur la branche `main` met le site à jour si Netlify est relié au dépôt.
