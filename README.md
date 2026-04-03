# Portfolio Ouraga — BTS SIO

Portfolio personnel réalisé dans le cadre du BTS SIO.

## Déploiement sur GitHub Pages

1. **Créer un repo GitHub** : va sur [github.com/new](https://github.com/new) et crée un repo (ex: `portfolio`)
2. **Push le code** :
   ```bash
   cd portfolio
   git init
   git add .
   git commit -m "Portfolio BTS SIO"
   git branch -M main
   git remote add origin https://github.com/SOUSY94/portfolio.git
   git push -u origin main
   ```
3. **Activer GitHub Pages** :
   - Va dans **Settings → Pages**
   - Source : **Deploy from a branch**
   - Branch : **main** / dossier **(root)**
   - Clique **Save**
4. Ton site sera accessible à : `https://SOUSY94.github.io/portfolio/`

## Ce qu'il te reste à faire

### 1. Remplacer ton adresse email
Dans `index.html`, cherche `ton.email@gmail.com` et remplace-le par ta vraie adresse (2 endroits dans la section Contact).

### 2. Ajouter ta photo de profil
- Place ta photo dans `images/profile.jpg`
- Dans `index.html`, décommente la ligne `<img src="images/profile.jpg" ...>` et supprime le div placeholder

### 3. Ajouter tes captures d'écran
Place tes captures dans `images/` avec ces noms :

| Projet | Fichiers attendus |
|---|---|
| Site Vitrine | `images/vitrine1.png`, `vitrine2.png`, `vitrine3.png` |
| WordPress | `images/wordpress1.png`, `wordpress2.png`, `wordpress3.png` |
| Gest Travaux | `images/gest1.png`, `gest2.png`, `gest3.png` |
| Stage SIO1 | `images/stage1.png` |
| Stage SIO2 | `images/stage2.png` |

Puis remplace les `<div class="img-placeholder">` par des `<img src="images/fichier.png" alt="...">` dans le HTML.

### 4. Ajouter tes attestations de stage
Place tes PDF dans `assets/` :
- `assets/attestation-sio1.pdf`
- `assets/attestation-sio2.pdf`

## Structure du projet

```
portfolio/
├── index.html          ← Page principale (GitHub Pages entry)
├── stage.html          ← Page détail du stage
├── veille.html         ← Page veille technologique
├── .nojekyll           ← Désactive le processing Jekyll
├── README.md
├── images/
│   ├── profile.jpg     ← Ta photo (à ajouter)
│   ├── jeu1.gif        ← Memory Game (déjà présent)
│   ├── jeu2.gif
│   ├── jeu3.png
│   ├── vitrine1.png    ← Captures site vitrine (à ajouter)
│   ├── ...
│   ├── stage1.png      ← Captures stage (à ajouter)
│   └── stage2.png
└── assets/
    ├── CV_Ouraga.pdf           ← Ton CV (déjà présent)
    ├── attestation-sio1.pdf    ← Attestation 1 (à ajouter)
    └── attestation-sio2.pdf    ← Attestation 2 (à ajouter)
```

## Technologies

- HTML5 / CSS3 (Flexbox, Grid, animations)
- JavaScript (thème, lightbox, menu mobile, smooth scroll)
- Hébergé sur GitHub Pages
