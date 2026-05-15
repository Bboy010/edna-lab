# eDNA Research UNA — Site Web

## Contexte du projet

Site vitrine moderne et épuré pour le **eDNA Laboratory** de l'Université Nangui-Abrogoua (UNA), Abidjan, Côte d'Ivoire. Le laboratoire offre des services de séquençage et de bioinformatique basés sur l'ADN environnemental (eDNA).

Déploiement cible : **Netlify via GitHub** (site statique, HTML/CSS/JS vanilla).

---

## Structure du projet

```
Bioinformatic-training-2026/
├── index.html              # Page principale du site
├── CLAUDE.md               # Ce fichier
├── netlify.toml            # Config Netlify
├── .gitignore
├── assets/
│   ├── css/
│   │   └── style.css
│   ├── js/
│   │   └── main.js
│   └── images/             # Copier les logos ici
├── logo-bio-info/          # Logos source
│   ├── eDNA-lab.jpg        # Logo principal eDNA Laboratory
│   ├── Logo Lw.png         # Partenaire 1 : LearnerWorld
│   ├── nf-core.png         # Partenaire : nf-core
│   ├── nextflow.jpg        # Partenaire : Nextflow
│   └── cabinet-lewis.jpg   # Partenaire : Cabinet Lewis
└── brochure_v3.html        # Brochure formations (existant)
```

---

## Identité visuelle

- **Logo principal** : `logo-bio-info/eDNA-lab.jpg`
- **Palette de couleurs** :
  - Primaire navy : `#0D1B2A`
  - Teal accent : `#0E7C7B` / `#0AAFA0`
  - Or accent : `#F0A500`
  - Fond clair : `#F4F9FC`
- **Typographies** : Space Grotesk (corps) + DM Serif Display (titres)
- **Style** : Moderne, épuré, scientifique, dark mode avec accents lumineux

---

## Organisation du laboratoire

### Direction
- **Head** : Dr. Ouattara Koffi Nouho

### Équipes
| Pôle | Membres | Responsabilités |
|------|---------|-----------------|
| **Field Activities** | Owo Nicolas, Yao Koffi Olivier | Stratégie d'échantillonnage |
| **Dry Lab (Bioinformatique)** | Hongo Koffi Anderson, Kouadio Ines | Formation, bourses, gestion des données |
| **Wet Lab** | Kouame N'Guessan, Adous Carine | Extraction, amplification, séquençage |

---

## Services offerts

### 3 axes principaux
1. **Barcoding** — Single Species & Multiplex → Phylogénétique & Phylogénomique → Écologie/Conservation/Biodiversité
2. **Metabarcoding** — Bulk DNA & Environmental DNA → Analyses communautaires
3. **Métagénomique** — WGS, Shotgun, Amplicon sequencing → Taxonomie & Génomique fonctionnelle → Biotechnologie

### Applications
- Écologie & Conservation de la biodiversité
- Biotechnologie
- Pangnomique & Épigénomique
- Meta-omique (Métabolomique, Protéomique, Transcriptomique)

---

## Équipements

| Équipement | Description |
|-----------|-------------|
| **BENTOLAB** | 3 équipements en 1 bloc (Gel Électrophorèse, Transilluminateur, Centrifugeuse, Thermocycleur PCR) |
| **miniPCR BIO** | 2 équipements en 1 bloc |
| **MinION mk1b** | Oxford Nanopore Technology — NGS 3ème génération (Long Read) |
| **Curiosty** | Microscope portable terrain — Caméra 4K, grossissements ×2 à ×20 |

---

## Partenaires

### Dans le dossier `logo-bio-info/`
1. `Logo Lw.png` — **LearnerWorld** (partenaire principal formations)
2. `nf-core.png` — **nf-core**
3. `nextflow.jpg` — **Nextflow**
4. `cabinet-lewis.jpg` — **Cabinet Lewis** (FDFP)

### Autres partenaires (logos à ajouter)
- Public Health Alliance for Genomic Epidemiology
- Zymo Research
- ZMT Academy
- Critical Ecosystem Partnership Fund
- Wellcome Connecting Science
- VALIDATE
- WAMBA.net
- POGO (Partnership for Observation of the Global Ocean)
- eDNA Collaborative
- Oxford Nanopore
- PacBio

---

## Stratégie eDNA

- **Recherche** : Projets financés (Azagny, Fonsti, Cocody Bay, Firca) + Collaborations (WCS, eDNA Collaborative, Anvi'O, Umea, PacBio)
- **Vision eDNA** : Capacity Building → GitHub / Protocol IO
- **Consulting** : Sessions de formation + Services (Barcoding, Metabarcoding, Métagénomique)

---

## Pages du site

1. **Accueil (Hero)** — Mission, accroche, CTA contact
2. **À propos** — Histoire du labo, UNA, vision
3. **Services** — Barcoding, Metabarcoding, Métagénomique + Bioinformatique
4. **Équipe** — Dr. Ouattara + membres par pôle
5. **Équipements** — BENTOLAB, miniPCR, MinION, Curiosty
6. **Formations** — Lien vers brochure, ateliers NGS
7. **Partenaires** — Grille de logos
8. **Contact** — Formulaire + coordonnées

---

## Déploiement

### Stack technique
- HTML5 / CSS3 / JavaScript vanilla (pas de framework — compatibilité Netlify optimale)
- Google Fonts (Space Grotesk + DM Serif Display)
- Site **100% statique**

### Workflow Git → Netlify
```bash
git init
git remote add origin <repo-github>
git push origin main
# Connecter le repo GitHub à Netlify
# Build command: (vide)
# Publish directory: . (racine)
```

### netlify.toml
```toml
[build]
  publish = "."

[[headers]]
  for = "/*"
  [headers.values]
    X-Frame-Options = "DENY"
    X-Content-Type-Options = "nosniff"
```

---

## Contacts

- **Email** : learnerworld22@gmail.com
- **Site partenaire** : www.learner-world.com
- **Localisation** : Abidjan, Côte d'Ivoire
- **Institution** : Université Nangui-Abrogoua (UNA)
