# 🦅 DIGIYLYFE — Clip terrain (20 s)

> **De Saly à Sarlat — le business local reprend la main.**
> Maquette HTML autonome du clip de présentation DIGIYLYFE. Auto-play, son embarqué, zéro dépendance.

---

## C'est quoi

Un clip de 20 secondes qui fait comprendre DIGIYLYFE sans expliquer toute la forêt : on montre le terrain, on montre le QR, on montre le contact direct, on frappe avec la doctrine.

Tout tient dans **un seul fichier** (`digiy-clip.html`). Pas de build, pas de serveur, pas de CDN. Tu ouvres, ça joue.

---

## Contenu du dossier

| Fichier | Rôle |
|---------|------|
| `digiy-clip.html` | Le clip complet (animation + musique générée + QR scannable) |
| `qr-digiylyfe.png` | Le QR DIGIY en image, réutilisable (affiche, flyer, fiche) |
| `voix-off-kit.md` | Script voix off calé sur les scènes + méthode d'enregistrement |
| `README.md` | Ce fichier |

---

## Lancer le clip

**En local** : double-clic sur `digiy-clip.html` → bouton **▶ LANCER LE CLIP**.

> Le clic est obligatoire pour débloquer le son (règle des navigateurs). Pour un screen-record propre, tu cliques, ça part avec la musique.

---

## Le déroulé — 6 séquences

| Temps | Scène |
|-------|-------|
| 0–3 s | De Saly à Sarlat — le terrain |
| 3–6 s | Le problème : « le lien est cassé » |
| 6–10 s | Scan QR → fiche pro qui s'ouvre |
| 10–14 s | Les 7 modules (LOC · DRIVER · MARKET · JOBS · RESA · PAY · EXPLORE) |
| 14–17 s | La doctrine : 0% commission, paiement direct, le terrain garde la main |
| 17–20 s | Signature 🦅 DIGIYLYFE + QR |

Le son suit l'image : groove sobre au début, montée sur les modules, **drop sec sur la doctrine** avec impacts calés sur chaque mot, puis résolution lumineuse sur l'aigle.

---

## Héberger sur GitHub Pages

C'est du statique pur, donc c'est direct :

```bash
git add digiy-clip.html qr-digiylyfe.png
git commit -m "Clip terrain DIGIYLYFE 20s"
git push
```

Active GitHub Pages sur le repo (Settings → Pages → branche `main`), et le clip est en ligne. Tu peux le pointer sur un sous-domaine type `clip.digiylyfe.com`.

---

## Personnaliser

**Le QR** → pointe vers `https://digiylyfe.com`. Pour le changer, modifie la variable `QR_URL` et la matrice `QR_MATRIX` dans le `<script>` (ou régénère un QR et remplace).

**La fiche pro** → cherche le bloc `class="fiche"` dans la scène `#s3`. Remplace `Ndiaye Auto` / `DIGIY DRIVER · Saly` par un vrai pro du Club.

**La voix off** → renomme ton enregistrement en **`voix.mp3`**, pose-le dans le même dossier. Le clip le détecte, lance la voix, et **baisse la musique automatiquement** (ducking). Détails complets dans `voix-off-kit.md`.

---

## Faire le MP4

Screen-record le cadre 16:9 pendant que le clip joue (OBS, ou enregistrement d'écran natif). La barre de progression et les boutons sont **hors** du cadre vidéo → ton enregistrement reste propre.

---

## Doctrine

```
0% COMMISSION
PAIEMENT DIRECT AU PRO
CONTACT DIRECT
LE TERRAIN GARDE LA MAIN
```

DIGIYLYFE ne capture pas le terrain. **DIGIYLYFE équipe le terrain.**

---

## Identité

- **Couleurs** : vert terrain `#1A5C38` · or `#C49A22`
- **Territoire** : Saly / Petite Côte (Sénégal) + Sarlat (France)
- **Marque** : Club des Métiers du Terrain

---

*Sobre devant. Redoutable derrière.*

🦅♾️ **Aigle Royal** — pierre par pierre.
