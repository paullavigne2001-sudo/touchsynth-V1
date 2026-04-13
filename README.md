# TouchSynth 🎵✨

Une application web interactive qui génère du son et des effets visuels au toucher.

## Demo

Ouvre `index.html` dans ton navigateur — aucun serveur requis.  
Ou déploie sur GitHub Pages en 2 minutes (voir ci-dessous).

## Fonctionnalités

- 🎹 **Son au toucher** — chaque position X joue une note d'une gamme pentatonique sur 2 octaves
- 🎛️ **Son modulé par le glissement** — l'axe Y contrôle le filtre passe-bas et le détunage
- 🌈 **Traces lumineuses** — particules colorées qui s'estompent progressivement
- 💡 **Halos persistants** — taches de lumière qui disparaissent lentement
- 🔁 **Multi-touch** — plusieurs doigts = plusieurs notes simultanées
- 🎸 **Changement de timbre** — double-tape (ou clic droit) pour cycler entre Sine / Triangle / Sawtooth / Square
- 🔊 **Réverbération** — convolution légère pour un son ambiant
- 📊 **Visualiseur de forme d'onde** — barre animée en bas de l'écran

## Déploiement sur GitHub Pages

### Méthode 1 — Interface GitHub (la plus simple)

1. Crée un nouveau dépôt sur [github.com/new](https://github.com/new)
2. Nomme-le `touchsynth` (ou ce que tu veux)
3. Laisse-le **public**
4. Clique **"Add file" → "Upload files"** et dépose `index.html`
5. Va dans **Settings → Pages**
6. Sous *Source*, sélectionne **"Deploy from a branch"** → branche `main` → dossier `/ (root)`
7. Clique **Save** — ton app sera dispo à `https://TON_USERNAME.github.io/touchsynth/`

### Méthode 2 — Git en ligne de commande

```bash
git init
git add index.html README.md
git commit -m "feat: initial TouchSynth"
git branch -M main
git remote add origin https://github.com/TON_USERNAME/touchsynth.git
git push -u origin main
```

Puis active GitHub Pages dans Settings → Pages.

## Utilisation

| Action | Effet |
|---|---|
| Toucher / Cliquer | Joue une note, crée une explosion de particules |
| Glisser horizontalement | Change la note (gamme pentatonique) |
| Glisser verticalement | Modifie le filtre et le détunage |
| Double-tap / Clic droit | Cycle le timbre (Sine → Triangle → Sawtooth → Square) |
| Plusieurs doigts | Polyphonie — plusieurs notes simultanées |

## Structure

```
touchsynth/
└── index.html   # Application complète (HTML + CSS + JS en un seul fichier)
└── README.md
```

Tout est dans un seul fichier — pas de dépendances, pas de build step.

## Compatibilité

- ✅ Chrome / Edge (desktop & mobile)
- ✅ Safari iOS (avec geste initial requis pour l'audio — comportement normal du navigateur)
- ✅ Firefox
- ✅ Android Chrome

## Licence

MIT — libre de modifier, distribuer, utiliser.
