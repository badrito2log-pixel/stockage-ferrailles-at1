# Stockage ferrailles, zone AT1 – flux amont

Maquette 3D du stockage des aciers de la zone AT1 (SNCF Réseau, EIV de Saulon) : plan du site, cantilevers, stockage au sol sous le portique, plan de rangement et indicateurs.

## Les deux pages

| Page | Pour qui | Ce qu'on peut faire |
|---|---|---|
| `index.html` (lien à communiquer) | Les personnes qui consultent | Voir la maquette, les chiffres et le tableau, filtrer, exporter le rapport PDF. Lecture seule. |
| `edition.html` | Les éditeurs | Ajouter, modifier, déplacer ou supprimer des références, retirer ou remettre un cantilever, puis publier le plan. |

## Mettre le site en ligne (une seule fois)

1. Créez un compte sur github.com (ou utilisez le vôtre).
2. Cliquez sur **New repository**, nommez-le `stockage-ferrailles-at1`, puis **Create repository**.
3. Sur la page du dépôt, cliquez sur **uploading an existing file** et glissez **tout le contenu de ce dossier** (y compris le dossier `img` et le fichier `.nojekyll`), puis **Commit changes**.
4. Allez dans **Settings > Pages**. Dans « Build and deployment », choisissez **Deploy from a branch**, branche **main**, dossier **/ (root)**, puis **Save**.
5. Après une à deux minutes, le site est en ligne à l'adresse :
   `https://VOTRE-NOM-GITHUB.github.io/stockage-ferrailles-at1/`
   C'est ce lien que vous communiquez aux personnes qui consultent.
   La page d'édition est à la même adresse suivie de `edition.html`.

## Donner les droits d'édition

Publier un nouveau plan revient à modifier le fichier `plan.js` du dépôt. Seules les personnes qui ont le droit d'écrire dans le dépôt peuvent le faire :

- **Settings > Collaborators > Add people** : invitez un éditeur avec son compte GitHub (rôle **Write**).
- Les personnes qui ne sont pas collaboratrices peuvent ouvrir le site, mais ne peuvent rien publier.

## Publier un nouveau plan (éditeurs)

1. Ouvrez `edition.html` (en ligne ou sur votre PC).
2. Faites vos changements : ils sont gardés comme brouillon dans votre navigateur.
3. Cliquez sur **Exporter plan.js pour publication** (carte « Modifications »).
4. Sur GitHub, dans le dépôt : **Add file > Upload files**, déposez le nouveau `plan.js` (il remplace l'ancien), puis **Commit changes**.
5. Le site se met à jour en une à deux minutes. Les personnes qui ont déjà la page ouverte doivent la recharger (le navigateur peut garder l'ancien plan jusqu'à 10 minutes).

Boutons utiles dans la page d'édition :
- **Revenir au plan publié** : efface votre brouillon et repart du plan en ligne.
- **Revenir au plan du classeur** : repart du plan de rangement du classeur Excel.

## Contenu du dossier

| Fichier | Rôle |
|---|---|
| `index.html`, `edition.html` | Les deux pages |
| `style.css` | La mise en forme |
| `app.js` | Le fonctionnement (3D, filtres, tableau, export) |
| `data.js` | Le plan de rangement du classeur et le plan du site |
| `plan.js` | Le plan publié (remplacé à chaque publication) |
| `vehicules.js` | Les modèles 3D des véhicules |
| `img/` | Photo de fond, logo, icône |

Une connexion Internet est nécessaire pour charger le moteur 3D, la police et le module PDF.

## Crédits des modèles 3D

- Pick-up et moto : Innerscene Corp (innerscene.com), domaine public CC0 1.0.
- Semi-remorque bâchée : modèle fourni par l'utilisateur (licence à vérifier auprès de sa source).
