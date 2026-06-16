# Skavyoy — link

Bio-link minimaliste : un pseudonyme au centre, les liens en orbite autour,
le tout flottant sur un shader animé. Une seule couleur d'accent sombre (bleu),
aucun texte superflu.

**➜ https://skavyoy8.github.io/link/**

## Concept

Fusion de deux idées :
- **Radial orbital timeline** — les liens (nœuds) tournent autour du noyau central avec
  profondeur (échelle / opacité / z-index), pause au survol, clic = ouverture du lien.
- **Shader lines** — fond WebGL ([Three.js](https://threejs.org/)) de lignes radiantes,
  passé en monochrome teinté sur l'accent et atténué pour rester sombre.

Le pseudo central est aussi le bouton « partager » (clic = copie du lien).

## Tech

- Un seul fichier (`index.html`), zéro build, Three.js via CDN.
- Accent = une seule variable CSS `--accent` (change-la pour changer toute l'ambiance).
- Accessible : liens réels (fonctionnent sans JS), `prefers-reduced-motion` respecté,
  navigation clavier, titre lisible par lecteur d'écran.

## Lancer en local

```bash
npx serve .
```
