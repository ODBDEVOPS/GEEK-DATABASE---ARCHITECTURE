# GEEK-DATABASE---ARCHITECTURE
repository complet pour un site "Geek Database" qui servira de base pour un projet de gestion de collections (films, séries, jeux, livres, mangas, etc.).
# 📁 STRUCTURE DU REPOSITORY
```
GeekDatabase/
├── 📁 .github/
│   ├── 📁 workflows/
│   │   ├── deploy.yml           # Déploiement GitHub Pages
│   │   ├── preview.yml          # Prévisualisation PR
│   │   ├── audit.yml            # Audit hebdomadaire
│   │   └── data-sync.yml        # Synchronisation données externes
│   │
│   ├── 📁 ISSUE_TEMPLATE/
│   │   ├── bug_report.md
│   │   ├── feature_request.md
│   │   └── database_entry.md
│   │
│   └── 📁 dependabot/
│       └── config.yml
│
├── 📁 src/
│   ├── 📁 assets/
│   │   ├── 📁 fonts/
│   │   ├── 📁 icons/
│   │   ├── 📁 images/
│   │   │   ├── 📁 covers/
│   │   │   ├── 📁 posters/
│   │   │   └── 📁 avatars/
│   │   └── 📁 logos/
│   │
│   ├── 📁 components/
│   │   ├── 📁 ui/
│   │   │   ├── Card/
│   │   │   ├── Modal/
│   │   │   ├── SearchBar/
│   │   │   ├── Pagination/
│   │   │   └── FilterPanel/
│   │   │
│   │   ├── 📁 layout/
│   │   │   ├── Header/
│   │   │   ├── Footer/
│   │   │   ├── Sidebar/
│   │   │   └── Grid/
│   │   │
│   │   └── 📁 features/
│   │       ├── MediaCard/
│   │       ├── CollectionGrid/
│   │       ├── RatingStars/
│   │       └── WishlistButton/
│   │
│   ├── 📁 data/
│   │   ├── 📁 schemas/
│   │   │   ├── movie.json
│   │   │   ├── game.json
│   │   │   ├── book.json
│   │   │   └── series.json
│   │   │
│   │   ├── 📁 collections/
│   │   │   ├── movies.json
│   │   │   ├── games.json
│   │   │   ├── books.json
│   │   │   └── series.json
│   │   │
│   │   └── 📁 users/
│   │       ├── sample_user.json
│   │       └── collections/
│   │
│   ├── 📁 pages/
│   │   ├── index.html
│   │   ├── dashboard.html
│   │   ├── catalog/
│   │   │   ├── movies.html
│   │   │   ├── games.html
│   │   │   ├── books.html
│   │   │   └── series.html
│   │   │
│   │   ├── collection/
│   │   │   ├── my-collection.html
│   │   │   ├── wishlist.html
│   │   │   └── statistics.html
│   │   │
│   │   ├── community/
│   │   │   ├── users.html
│   │   │   ├── reviews.html
│   │   │   └── rankings.html
│   │   │
│   │   ├── about.html
│   │   ├── api.html
│   │   └── 404.html
│   │
│   ├── 📁 styles/
│   │   ├── 📁 base/
│   │   │   ├── _variables.css
│   │   │   ├── _reset.css
│   │   │   ├── _typography.css
│   │   │   └── _animations.css
│   │   │
│   │   ├── 📁 layouts/
│   │   │   ├── _grid.css
│   │   │   ├── _header.css
│   │   │   └── _footer.css
│   │   │
│   │   ├── 📁 components/
│   │   │   ├── _cards.css
│   │   │   ├── _buttons.css
│   │   │   └── _forms.css
│   │   │
│   │   ├── 📁 pages/
│   │   │   ├── _home.css
│   │   │   ├── _catalog.css
│   │   │   └── _dashboard.css
│   │   │
│   │   ├── main.css
│   │   └── themes/
│   │       ├── light.css
│   │       ├── dark.css
│   │       └── cyberpunk.css
│   │
│   ├── 📁 scripts/
│   │   ├── 📁 modules/
│   │   │   ├── database.js
│   │   │   ├── search.js
│   │   │   ├── filters.js
│   │   │   ├── api.js
│   │   │   └── auth.js
│   │   │
│   │   ├── 📁 utils/
│   │   │   ├── helpers.js
│   │   │   ├── validators.js
│   │   │   └── formatters.js
│   │   │
│   │   ├── app.js
│   │   └── service-worker.js
│   │
│   └── 📁 templates/
│       ├── base.html
│       ├── media-card.html
│       ├── user-card.html
│       └── review-card.html
│
├── 📁 docs/
│   ├── 📁 api/
│   │   ├── REST.md
│   │   └── examples.md
│   │
│   ├── 📁 architecture/
│   │   ├── database-schema.md
│   │   └── component-structure.md
│   │
│   ├── 📁 deployment/
│   │   ├── GITHUB_PAGES.md
│   │   └── CUSTOM_DOMAINS.md
│   │
│   ├── CONTRIBUTING.md
│   ├── CODE_OF_CONDUCT.md
│   └── DATA_FORMAT.md
│
├── 📁 tools/
│   ├── build-gh-pages.js
│   ├── data-generator.js
│   ├── image-optimizer.js
│   └── sitemap-generator.js
│
├── 📁 tests/
│   ├── 📁 unit/
│   │   ├── database.test.js
│   │   └── search.test.js
│   │
│   ├── 📁 e2e/
│   │   └── basic-navigation.test.js
│   │
│   └── jest.config.js
│
├── 📁 public/
│   ├── robots.txt
│   ├── manifest.json
│   ├── browserconfig.xml
│   └── favicon/
│
├── _config.yml
├── .nojekyll
├── CNAME
├── .gitignore
├── package.json
├── README.md
├── LICENSE
├── lighthouserc.json
├── netlify.toml
└── vercel.json
```
# 🎮 Geek Database

![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Deployed-brightgreen)
![GitHub Actions](https://img.shields.io/github/actions/workflow/status/votrenom/geek-database/deploy.yml)
![Website](https://img.shields.io/website?url=https%3A%2F%2Fvotrenom.github.io%2Fgeek-database)
![License](https://img.shields.io/badge/License-MIT-blue)
![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen)

> Base de données collaborative pour collectionneurs geeks - Films, Séries, Jeux, Livres, Mangas

🌐 **Live Demo :** [https://votrenom.github.io/geek-database](https://votrenom.github.io/geek-database)

## ✨ Fonctionnalités

- 📚 **Catalogue complet** : Films, séries, jeux vidéo, livres, mangas
- 🏷️ **Système de tags** : Catégorisation avancée par genre, plateforme, etc.
- 🔍 **Recherche avancée** : Filtres multiples et recherche en temps réel
- 📊 **Statistiques** : Visualisations de vos collections
- 👥 **Communauté** : Partage et découverte des collections des autres
- 📱 **Responsive** : Design adapté mobile, tablette et desktop
- 🔄 **Offline-first** : Fonctionne hors connexion (PWA)
- 🎨 **Multi-themes** : Light, Dark, Cyberpunk

## 🚀 Démarrage Rapide

### Prérequis
- Node.js 18+
- npm 9+

### Installation
```bash
# 1. Cloner le projet
git clone https://github.com/votrenom/geek-database.git
cd geek-database

# 2. Installer les dépendances
npm install

# 3. Démarrer le serveur de développement
npm run dev

# 4. (Optionnel) Démarrer le mock API
npm run dev:data
