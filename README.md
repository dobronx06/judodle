# Judodle

Jeu de devinette quotidien des techniques de judo du Kodokan.
Construit avec Astro, deployable sur Cloudflare Pages, Vercel, Netlify ou tout hebergeur de sites statiques.

## Demarrage rapide

```bash
npm install
npm run dev      # Serveur de dev sur localhost:4321
npm run build    # Build statique dans dist/
npm run preview  # Previsualisation du build
```

## Description

Judodle est un jeu quotidien inspire de Wordle ou le joueur doit deviner la technique de judo du jour parmi les 100 techniques officielles du Kodokan. Chaque tentative revele des indices sur les attributs de la technique (categorie, groupe, traduction, premiere apparition, etc.).

## Contenu

- **100 techniques** du repertoire officiel du Kodokan
- **6 attributs** d'indices : traduction, categorie, groupe, premiere apparition, debout/sol, lettre initiale
- **1 mode de jeu** : Classique (comparaison d'attributs)
- **Theme visuel** inspire du tatami, du judogi blanc, et des couleurs officielles IJF (blanc/bleu/rouge/or)

## Structure du projet

```
src/
  data/
    data.json     <-- 100 techniques de judo
    theme.json    <-- Theme visuel Kodokan
  components/
    Header.astro
    Footer.astro  <-- Mention "Non affilie au Kodokan ni a l'IJF"
    AdSlot.astro
  layouts/
    Layout.astro  <-- Injecte le theme en CSS vars
  pages/
    index.astro   <-- Logique du jeu
  styles/
    global.css
public/
  favicon.svg
```

## Theme

Le theme s'inspire de l'esthetique traditionnelle du judo :
- **Couleurs** : beige tatami, blanc judogi, bleu IJF, rouge ippon, or medaille
- **Typographie** : Noto Sans JP (respecte l'origine japonaise) + Inter
- **Ambiance** : traditionnelle mais accessible, pedagogique et respectueuse

## Deploiement

1. Pousser le repo sur GitHub
2. Connecter a Cloudflare Pages (ou Vercel/Netlify)
3. Build command : `npm run build`
4. Output directory : `dist`

## Mentions legales

Non affilie au Kodokan Institute ni a l'International Judo Federation (IJF).
Les techniques de judo mentionnees appartiennent au patrimoine du judo et sont
repertoriees selon la nomenclature officielle du Kodokan.

## Licence

Prive. Dataset et theme propres a ce projet.
