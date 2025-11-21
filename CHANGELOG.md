# Changelog

All notable changes to this project are documented in this file.

## 2025-11-21

### Added
- Solutions chimiques
  - New listing page: pages/solutions-chimiques.html
  - Dynamic PDP for solutions: pages/products/pdp.html (query: ?slug=...)
  - Individual acetone PDP template: pages/products/acetone.html (later superseded by dynamic PDP)
  - Linked category card on pages/produits.html to the listing page

- Tubes sous vide
  - New category listing: pages/tubes-sous-vide.html (marques: VACUETTE, MEDIPLUS, VACUTEST)
  - Brand pages:
    - pages/tubes-sous-vide/vacuette.html
    - pages/tubes-sous-vide/mediplus.html
    - pages/tubes-sous-vide/vacutest.html
  - Dynamic PDP for tubes: pages/products/pdp_tube.html (query: ?marque=...&slug=...)

- Colorants
  - Category listing: pages/colorants.html (marques: RAL, SOLVAPUR)
  - Brand pages:
    - pages/colorants/ral.html
    - pages/colorants/solvapur.html
  - Dynamic PDP for colorants: pages/products/pdp_colorant.html (query: ?marque=...&slug=...)

- Micropipettes
  - Category listing: pages/micropipettes.html (marques: ACCUMAX, DRAGONLAB, ONILAB)
  - Brand pages:
    - pages/micropipettes/accumax.html
    - pages/micropipettes/dragonlab.html
    - pages/micropipettes/onilab.html
  - Dynamic PDP for micropipettes: pages/products/pdp_micropipette.html (query: ?marque=...&slug=...)

- Tests rapides & réactifs
  - Category listing: pages/tests-rapides.html (marques: BIOTEST, SD BIOSENSOR, Autres marques)
  - Brand pages:
    - pages/tests-rapides/biotest.html
    - pages/tests-rapides/sd-biosensor.html
    - pages/tests-rapides/autres.html
  - Dynamic PDP for tests rapides: pages/products/pdp_test_rapide.html (query: ?marque=...&slug=...)

### Changed
- pages/produits.html
  - Fixed stray character in navigation
  - Added new "Solutions chimiques" chip and card
  - Linked "Solutions chimiques" to pages/solutions-chimiques.html
  - Linked "Tubes sous vide" to pages/tubes-sous-vide.html
  - Linked "Coloration" to pages/colorants.html
  - Linked "Micropipettes" to pages/micropipettes.html
  - Linked "Tests rapides & réactifs" to pages/tests-rapides.html

### Fixed
- Image path issues
  - Standardized on assets/tube_sous_vide/... for tubes, with fallbacks to legacy assets/TUBES SOUS VIDE/... in dynamic PDP
  - URL-encoded spaces in file and folder names across pages to ensure images load reliably in browsers
  - Corrected file extensions (.jpeg, .jpg, .png, .jfif) where applicable

### Notes
- Slugging convention: lowercase, accents removed, spaces replaced by hyphens, punctuation simplified
- All dynamic PDP pages include informational notes and back links to their respective listing pages
- Listings and PDPs are intentionally image-driven; office document contents are not parsed
