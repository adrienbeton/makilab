# MakiLab Site — One-Pager

Site personnel one-page pour **Adrien Beton / makilab.io**. **Source de vérité : `index.html`** (single-file, all CSS+JS inline). Toute mise à jour de ce CLAUDE.md doit refléter le site, jamais l'inverse.

---

## Contexte projet

**Objectif** : Présenter Adrien (Sydney relocation) + MakiLab (lab de produits) en une page narrative. Cible : recruteurs Sydney + prospects consulting.

**Positionnement** : Strategy + data + sustainability — où ces trois champs se rencontrent vraiment.

**Stack** :
- HTML5 + vanilla CSS + vanilla JS, **single file** (`index.html`, ~1600 lignes, inline)
- GSAP 3.12.5 + ScrollTrigger + ScrollToPlugin (cdnjs)
- Pas de Lenis, pas de build, pas de framework
- Fonts (Google Fonts) : **Outfit** (400-800) + **JetBrains Mono** (400) + **Caveat** (400, 600)

---

## Structure (ordre des sections dans `index.html`)

1. `#hero` — split layout : identité (gauche) / rôles terracotta (droite)
2. `#conviction1` — Sustainability (chapter 01)
3. `#conviction2` — Transformation (chapter 02) — visuel 4 pétales (Vision / Steering / Tools / People autour de "Orchestration")
4. `#conviction3` — Technology (chapter 03) — visuel terminal timeline 2007 → 2025
5. `#pivot` — reveal du logo MakiLab
6. `#products` — Latest projects, carousel V-thumb (4 produits)
7. `#cta` — Contact
8. `<footer>` — "From Lyon to Sydney."

UI globale : tweaks panel (accent / grain / chapters / herotop swappers), progress dots, hamburger overlay nav, SVG zoom overlay.

---

## Design system

**Palette (`:root` — noms courts, pas `--color-*`) :**
```css
--cream: #f5f0eb;        --warm-white: #faf7f4;
--primary: #1a3a4a;      --secondary: #2d6a7a;
--accent: #d97757;       --accent-deep: #c45a3c;
--teal-light: #4a9aaa;   --muted: #8a9a9a;
```

**Typo :**
```css
--font-body: 'Outfit', sans-serif;
--font-mono: 'JetBrains Mono', monospace;
--font-hand: 'Caveat', cursive;   /* "Hey! I'm", radiant petal notes */
```

**Ton visuel :** sobre, data-forward, accents manuscrits Caveat ponctuels.

---

## Copy clé (verbatim depuis `index.html`)

**Hero**
- "Hey! I'm" (Caveat) → **Adrien Beton** → "Polytechnique · Imperial College London"
- Status pill : `AVAILABLE · SYDNEY · FULL RIGHTS · LINKEDIN`
- Lead : *"I've spent 17 years where three fields belong together."*
- Threads : 01 Sustainability / 02 Transformation / 03 Technology
- Coda : *"Trained as an engineer. Curious by nature. Hands-on by habit. Restless about the state of the world."*
- Sectors : Energy · Transport · Infrastructure · +12 more
- Right panel roles : Builder. / Operator. / Architect. / Explorer.
- Stats : 100+ Projects · 50+ Clients · 17 Years

**Convictions (statements)**
- C1 : *"Sustainability is not a cause. It is a business performance system."*
- C2 : *"Transformation is not a deliverable. It's an orchestration problem."*
- C3 : *"Technology is an accelerator. Not a shortcut, not an endgame."*

**Pivot**
- "meet" + logo MakiLab + *"where experience meets the itch to experiment · learn · ship"*

**CTA**
- Headline : *"Let's build something together"*
- Subtitle : *"Relocating to Sydney with my family with full working rights. Looking for a role where strategy, data and sustainability actually meet."*
- Bouton unique : "Connect on LinkedIn" → linkedin.com/in/abeton
- Caveat : *"Always up for a coffee :)"*

(Pas d'email affiché. Pas de triple framing Hiring/Tool/Curious.)

---

## Produits MakiLab (section `#products`)

| Produit | Tagline | Description |
|---|---|---|
| **Scope3 Trail** | From spreadsheet chaos to audit-ready | Portfolio supplier carbon emissions, AI agents |
| **PVision** | From hours in PVSyst to minutes on a map | Solar pre-study + financial model |
| **TRACE** | Where responsible AI should start | Diagnostic IA responsable, 5 piliers, 30 questions |
| **Food Impact Chatbot** | Turning a database into a conversation | RAG bilingue sur Agribalyse |

Pas de colonne statut dans le site. Assets : `assets/<product>{1,2,3}-{desktop,mobile}.png`.

---

## Fichiers du repo (post-cleanup)

```
index.html             # Source de vérité, single-file
assets/                # PNG produits (desktop + mobile) + logo wordmark + portrait
CLAUDE.md              # Ce fichier
.gitignore
```

Tout le reste (`explorations/`, `brand-guidelines/`, `docs/`, `archive/`, `.playwright-mcp/`) est **gitignored** — local only.

---

## Règles de travail

- `index.html` = source de vérité unique. Si CLAUDE.md diverge du site, **mettre CLAUDE.md à jour, pas le site**.
- Toute modification de copy = vérifier le rendu dans `index.html` avant de commit.
- Animations via GSAP uniquement (ScrollTrigger / ScrollToPlugin), pas de CSS transitions pour le scrollytelling.
- Confirmation requise avant tout push ou déploiement.
