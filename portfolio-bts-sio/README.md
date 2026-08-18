# Portfolio BTS SIO — Guide simple

Site web en 2 fichiers seulement. Pas de JavaScript, pas d'installation.

## Les 2 fichiers à connaître

| Fichier | Rôle |
|---------|------|
| `index.html` | Le **contenu** : textes, titres, projets |
| `css/style.css` | L'**apparence** : couleurs, tailles, espacements |

## Voir ton site

Double-clique sur **`index.html`**. Il s'ouvre dans ton navigateur.

Tu peux aussi faire clic droit → **Ouvrir avec** → Chrome, Firefox, Edge...

## Modifier ton contenu

Ouvre `index.html` et cherche les commentaires **`MODIFIE ICI`**.

### Changer ton nom

```html
<h1>Bonjour, je suis Prénom Nom</h1>
```

Remplace `Prénom Nom` par ton nom.

### Ajouter un projet

1. Trouve la section `<!-- SECTION PROJETS -->`
2. Copie un bloc qui ressemble à ça :

```html
<article class="carte-projet">
  <p class="date-projet">Mars 2026</p>
  <h3>Titre du projet</h3>
  <p>Ce que tu as fait, en quelques phrases.</p>
  <p class="outils-projet">HTML · CSS</p>
</article>
```

3. Colle-le dans `<div class="liste-projets">`
4. Change la date, le titre, le texte et les outils

### Changer ton email

```html
<a href="mailto:ton.email@exemple.fr">ton.email@exemple.fr</a>
```

Les deux doivent être identiques (dans `href=` et entre les balises).

## Modifier les couleurs (optionnel)

Ouvre `css/style.css`. Les couleurs ressemblent à `#2563eb` (codes hexadécimaux).

Exemples dans le fichier :
- `#f5f7fa` → fond de la page
- `#2563eb` → bleu des liens et boutons
- `white` → fond blanc des blocs

## Structure du site

```
Accueil    → ton nom + phrase de présentation
À propos   → formation, lycée, option
Projets    → liste de tes travaux de l'année
Contact    → ton email
```

## En cas de problème

- **La page est toute blanche sans style** → vérifie que le dossier `css` est bien à côté de `index.html`
- **Un lien du menu ne marche pas** → vérifie que `href="#projets"` correspond bien à `id="projets"`
- **Tu as cassé quelque chose** → compare avec une carte-projet qui fonctionne encore
