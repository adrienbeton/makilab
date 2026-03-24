# MakiLab Site — Manifeste Scrollytelling

Site personnel one-page pour **Adrien Beton / makilab.io**. Scrollytelling GSAP, HTML statique, aucun framework.

---

## Contexte projet

**Objectif** : Site manifeste qui raconte le parcours d'Adrien → ses convictions → MakiLab. Cible double : recruteurs (Sydney) + prospects consulting.

**Positionnement** : "Data intelligence for positive impact." Pas une landing corporate — un manifeste authentique, sobre, technique.

**Stack** : HTML5 + vanilla CSS3 + vanilla JS + GSAP 3.12.5 (CDN). Fonts : Outfit + JetBrains Mono (Google Fonts). Pas de build, pas de framework.

---

## Structure narrative (immuable)

1. **Hero** — Adrien, statement, portrait
2. **Constat** — Le monde est cassé (brittle, anxious, non-linear)
3. **Conviction 1** — Sustainability as Operating System
4. **Conviction 2** — Transformation as Orchestration Problem
5. **Conviction 3** — Technology with Responsibility
6. **Pivot** — "I didn't stop at thinking. I build." → transition vers MakiLab
7. **MakiLab** — Le lab + les produits
8. **CTA** — Sydney relocation, hiring / tool / curious

---

## Design system

**Palette Deep Ocean :**
- `--color-primary: #1a3a4a` (navy)
- `--color-secondary: #2d6a7a` (teal)
- `--color-accent: #d97757` (terracotta)
- `--color-accent-deep: #c45a3c`
- `--color-teal-light: #4a9aaa`
- `--color-bg-light: #f5f0eb` (off-white)
- `--color-bg-dark: #0a0a0c` (near-black)

**Typo :** Outfit (body/titres) + JetBrains Mono (markers, code, chiffres clés)

**Ton visuel :** sobre, fonctionnel, data-forward. Pas décoratif.

---

## Copy clé (source of truth)

**Hero :**
```
Adrien Beton
17 years turning climate strategy into operations.
Now building the tools I wish I'd had.
```

**Constat :**
```
Brittle. Anxious. Non-linear. Incomprehensible.
Supply chains snap. Regulations multiply faster than organisations can absorb them.
Climate targets are set in boardrooms and forgotten in spreadsheets.
The old playbook doesn't hold.
```

**Conviction 1 :**
```
17 years inside the machine.
Sustainability is not a cost centre. It's an operating system.
Climate, resources, supply chains, social performance, governance, digital responsibility
— these aren't separate problems. They're one system.
```
Markers : net-zero roadmaps (40 pays), LCA multi-critères (15+ secteurs), SBTi, CSRD, 1 000 ktCO₂ sur un programme.

**Conviction 2 :**
```
17 years watching brilliant strategies die on slide 47.
Transformation is not a deliverable. It's an orchestration problem.
Vision. Measurement. Tools. Change. Four levers.
Most organisations activate one and call it strategy.
```
Markers : 15+ cycles design thinking, strategic foresight, frameworks adoptés à l'échelle orga.

**Conviction 3 :**
```
17 years building tools — from automated LCA spreadsheets to AI agents.
But technology without domain expertise produces beautiful interfaces on top of garbage data.
And technology without responsibility creates new problems while solving old ones.
```
Markers : AI climate workflows, responsible AI maturity, green IT, infra self-hosted.

**Pivot :**
```
That's 17 years of thinking about these problems.
But I didn't stop at thinking. I build.

Polytechnique × Imperial College. 15 years across EMEA. 81 projects. 15+ sectors.
I've spent my career at this intersection — thinking strategy and shipping tools.
And I got tired of building them for someone else's PowerPoint.
```

**CTA :**
```
I'm relocating to Sydney. Looking for where climate, tech, and execution actually meet.

Hiring? 17 years of building inside consulting. Ready to build inside your team.
Need a tool? AI workflows for climate and ESG teams. Let's scope it.
Curious? Always up for a real conversation.

adrien@makilab.io · LinkedIn
```

---

## Produits MakiLab

| Produit | Statut | Problème résolu |
|---|---|---|
| Scope3 Analyzer | MVP actif | Calcul automatisé émissions Scope 3 fournisseurs (Python + Claude API) |
| Food Impact Chatbot | MVP actif | LCA alimentaire conversationnel (RAG + Agribalyse, bilingue) |
| Climate Framework Translator | Concept | Équivalences CSRD/EU ↔ ASRS/australien |
| Responsible AI Maturity Mapper | Concept | Assessment gouvernance IA responsable |
| MakiPV / PV Business Case | En dev | Modélisation projets photovoltaïques |

---

## Fichiers clés

```
explorations/          # 14 prototypes HTML (v1 → v10b) — ne pas modifier
brand-guidelines/      # Assets visuels, palette, logo
docs/superpowers/
  plans/               # Plan d'implémentation détaillé
  specs/               # Specs design v1 → v4
```

**Prototype de référence :** `explorations/v4-manifeste.html` (direction retenue).
**Plan actif :** `docs/superpowers/plans/2026-03-24-manifeste-scrollytelling.md`

---

## Règles de travail

- **Jamais modifier les fichiers dans `explorations/`** — ce sont des archives de référence
- Nouvelles itérations → nouveau fichier ou dossier dédié
- Le copy ci-dessus est la source de vérité — ne pas improviser les textes
- Animations GSAP uniquement (pas de CSS transitions pour les effets scrollytelling)
- Confirmation requise avant tout push ou déploiement
