[README (15).md](https://github.com/user-attachments/files/29361058/README.15.md)
# 🦅 DIGIYLYFE — Clip terrain (45 s)

> **De Saly à Sarlat — le business local reprend la main.**
> Maquette HTML autonome du clip de présentation DIGIYLYFE. Auto-play, son embarqué, zéro dépendance.

---

## C'est quoi

Un clip de 45 secondes qui fait comprendre DIGIYLYFE sans expliquer toute la forêt : on montre le terrain, on montre le QR, on montre le contact direct, on frappe avec la doctrine.

Tout tient dans **un seul fichier** (`digiy-clip.html`). Pas de build, pas de serveur, pas de CDN. Tu ouvres, ça joue.

---

## Contenu du dossier

| Fichier | Rôle |
|---------|------|
| `digiy-clip.html` | Le clip complet (animation + musique générée + QR scannable) |
| `qr-digiylyfe.png` | Le QR DIGIY en image, réutilisable (affiche, flyer, fiche) |
| `voix-off-kit.md` | Script voix off calé sur les scènes + méthode d'enregistrement |
| `README.md` | Ce fichier |

> **Audio en option** — pose `voix.mp3` et/ou `musique.mp3` à côté du clip, ils sont détectés automatiquement (voir « Audio » plus bas).

---

## Lancer le clip

**En local** : double-clic sur `digiy-clip.html` → bouton **▶ LANCER LE CLIP**.

> Le clic est obligatoire pour débloquer le son (règle des navigateurs). Pour un screen-record propre, tu cliques, ça part avec la musique.

---

## Le déroulé — 6 séquences

| Temps | Scène |
|-------|-------|
| 0–7 s | De Saly à Sarlat — le terrain |
| 7–14 s | Le problème : « le lien est cassé » |
| 14–22 s | Scan QR → fiche pro qui s'ouvre |
| 22–34 s | Les 7 modules (LOC · DRIVER · MARKET · JOBS · RESA · PAY · EXPLORE) |
| 34–40 s | La doctrine : 0% commission, paiement direct, le terrain garde la main |
| 40–45 s | Signature 🦅 DIGIYLYFE + QR |

Le son suit l'image : groove sobre au début, montée sur les modules, **drop sec sur la doctrine** avec impacts calés sur chaque mot, puis résolution lumineuse sur l'aigle.

---

## Héberger sur GitHub Pages

C'est du statique pur, donc c'est direct :

```bash
git add digiy-clip.html qr-digiylyfe.png
git commit -m "Clip terrain DIGIYLYFE 45s"
git push
```

Active GitHub Pages sur le repo (Settings → Pages → branche `main`), et le clip est en ligne. Tu peux le pointer sur un sous-domaine type `clip.digiylyfe.com`.

---

## Partager le clip

Le clip a un bouton **🔗 Partager** (sous le cadre) :

- **Sur téléphone** → ouvre direct le partage natif (WhatsApp, SMS, etc.). Idéal pour le terrain.
- **Sur ordi** → copie le lien dans le presse-papier (ou ouvre WhatsApp Web en secours).

Pour que le lien partagé pointe au bon endroit, ouvre `digiy-clip.html` et règle la variable en haut du `<script>` :

```js
var SHARE_URL = "https://digiylyfe.com";  // mets ici l'adresse publique du clip
```

> Si le clip est déjà ouvert depuis une vraie page web (GitHub Pages), il partage **automatiquement** cette adresse — pas besoin de toucher à rien.

**Aperçu riche** : les balises Open Graph sont déjà en place. Quand quelqu'un colle le lien dans WhatsApp ou Facebook, ça affiche un joli aperçu (titre + doctrine + image) au lieu d'un lien tout nu.

---

## Personnaliser

**Le QR** → pointe vers `https://digiylyfe.com`. Pour le changer, modifie la variable `QR_URL` et la matrice `QR_MATRIX` dans le `<script>` (ou régénère un QR et remplace).

**La fiche pro** → cherche le bloc `class="fiche"` dans la scène `#s3`. Remplace `Ndiaye Auto` / `DIGIY DRIVER · Saly` par un vrai pro du Club.

---

## Audio (musique + voix)

Le clip a son propre **groove généré** par défaut (zéro fichier). Mais tu peux poser tes propres sons à côté du `.html` — ils sont détectés tout seuls :

| Fichier posé | Effet |
|--------------|-------|
| *(rien)* | Groove maison généré joue à plein volume |
| `musique.mp3` | **Remplace** le groove maison par ta piste |
| `voix.mp3` | Ajoute la voix off, la musique baisse toute seule (ducking) |
| les deux | Voix off + ta musique, mixées avec ducking |

**Musique perso** : pose `musique.mp3` dans le dossier. Pour démarrer la piste à un endroit précis (ex: tomber direct sur le drop), règle en haut du `<script>` :

```js
var MUSIC_START_AT = 0;  // seconde de départ dans la piste
```

> ⚠️ **Licence musique** — si tu utilises une piste **Epidemic Sound** (ex: *« All I Need » — DJ Mayson*), tu dois la télécharger **depuis ton compte Epidemic abonné** pour être couvert (YouTube, réseaux, etc.). Sans abonnement actif, ne la diffuse pas : claim/strike assuré. Renomme le fichier téléchargé en `musique.mp3`.

**Voix off** → renomme ton enregistrement en `voix.mp3`, pose-le dans le même dossier. Détails complets dans `voix-off-kit.md`.

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
