# Vitrine publique — dossier isolé

**Mission :** afficher images + GIF + texte marketing (problème, solution, technologies).

**Pas de code.** Pas de backend. Pas de lien vers l'app admin.

---

## Ouvrir la vitrine

Double-cliquez :

```text
public/OPEN_VITRINE.bat
```

Ou ouvrez `public/index.html` dans le navigateur.

Aucun serveur requis.

---

## Médias actuels

| Fichier                    | Dossier               |
| -------------------------- | --------------------- |
| `demo-1.gif`               | `assets/gifs/`        |
| `v1-gateway-dashboard.svg` | `assets/screenshots/` |
| `v2-gateway-openai.svg`    | `assets/screenshots/` |
| `v2-hardware-monitor.svg`  | `assets/screenshots/` |
| `v2-model-inspector.svg`   | `assets/screenshots/` |

Pour ajouter un GIF : déposez-le dans `assets/gifs/` puis mettez à jour `index.html`.

---

## Publier sur GitHub Pages (CV / LinkedIn)

Publiez **uniquement** le contenu de `public/` — jamais `back/` ni `front/`.

```powershell
# 1. Connexion (une fois)
gh auth login

# 2. Repo vitrine dédié (recommandé)
cd AI_INFRA_CENTER\public
gh repo create snorbik-ai-vitrine --public --source=. --remote=origin
git add -A
git commit -m "feat: vitrine publique avec demo GIF"
git push -u origin main
```

Puis GitHub → **Settings → Pages → Deploy from branch `main` / root**.

**Attention :** `demo-1.gif` fait ~123 Mo. GitHub refuse les fichiers > 100 Mo.
Options : compresser le GIF (ezgif.com) ou utiliser Git LFS avant le push.

Lien CV : `https://<votre-user>.github.io/snorbik-ai-vitrine/`
