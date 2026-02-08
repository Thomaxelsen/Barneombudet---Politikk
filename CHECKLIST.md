# Sjekkliste for token-kontroll per HTML-side

Denne sjekklisten verifiserer at **banner/header**, **bakgrunn**, **CTA-områder** og **chip/knapp‑stiler** følger de nye tokenene definert i `css/styles.css` (f.eks. `--brand-peach-*`, `--kf-*`, `--text-*`).

## index.html
- [x] Banner/header bruker `header`‑stilen med `--brand-peach-dark` og token‑farger for tekst. (Se `css/styles.css`.)
- [x] Bakgrunn kommer fra `body` (`--light-bg`). (Se `css/styles.css`.)
- [◐] CTA‑områder: `.btn-primary` bruker `--kf-dark-blue`, men `.btn-secondary` bruker hardkodede gråtoner (`#f5f5f5`, `#ddd`).
- [◐] Chip/knapp‑stiler: `.party-tag` bruker `--border-color`, men partifarge‑klassene (`.party-tag-*`) har hardkodede farger.

## party-constellations.html
- [x] Banner/header bruker global `header`‑stil (`--brand-peach-dark`).
- [x] Bakgrunn: `.main-content`, `.selection-container`, `.results-container` bruker `--light-bg` / `--brand-peach-*` tokens.
- [ ] CTA‑områder: `#selectAllBtn` / `#clearAllBtn` bruker hardkodede farger (`#007bff`, `#6c757d`).
- [◐] Chip/knapp‑stiler: `.constellation-header .party-tag` bygger på tokens for tekst, men får partifarger fra hardkodede klassene i `css/styles.css`.

## party-overview.html
- [x] Banner: `.party-header` bruker `--brand-peach-dark`.
- [◐] Bakgrunn: `.party-box` og flere paneler bruker hardkodede hvit‑/gråtoner.
- [◐] CTA‑områder: `.tab-button.active` / hover‑bakgrunner bruker hardkodede RGBA‑verdier.
- [◐] Chip/knapp‑stiler: `.seat-pill` bruker hardkodede RGBA‑bakgrunner (ikke token‑variabler).

## party-profile.html
- [x] Banner: `.party-hero-placeholder` og `.party-logo-banner` bruker `--brand-peach-dark` i gradienter.
- [◐] Bakgrunn: flere paneler bruker hardkodede hvit‑/blåtoner i gradienter.
- [◐] CTA‑områder: `.party-logo-button` hover/selected bruker hardkodede RGBA‑farger.
- [◐] Chip/knapp‑stiler: `.party-hero-pill` og support‑nivåer bruker hardkodede gradienter.

## party-similarity.html
- [x] Banner/header bruker global `header`‑stil (`--brand-peach-dark`).
- [x] Bakgrunn: `.similarity-introduction`, `.heatmap-container-main`, `.radar-comparison-section` bruker `--brand-peach-*` tokens.
- [x] CTA‑områder: `.radar-button` arver token‑farger fra `.button.primary` i `css/styles.css`.
- [◐] Chip/knapp‑stiler: label‑/tekstfarger har enkelte hardkodede gråtoner (`#555`, `#777`).

## party-unique.html
- [x] Banner/header bruker global `header`‑stil (`--brand-peach-dark`).
- [x] Bakgrunn: `.selection-container` bruker `--brand-peach-light`.
- [ ] CTA‑områder: `#selectAllBtn` / `#clearAllBtn` bruker hardkodede farger/gradienter.
- [◐] Chip/knapp‑stiler: `.party-tag-small` bruker tokens for tekst, men øvrige bakgrunner er hardkodet i flere kort.

## map-explorer.html
- [x] Banner: `.party-header` bruker `--brand-peach-dark`.
- [◐] Bakgrunn: paneler som `#candidate-display-panel` og kort bruker hardkodede grå/hvit‑toner.
- [x] CTA‑områder: ingen dedikerte CTA‑knapper utenom standard knapper i global stil.
- [◐] Chip/knapp‑stiler: ingen egne chips; kort og paneler bruker hardkodede bakgrunner.

## quiz.html
- [x] Banner: `.quiz-header` bruker `--brand-peach-dark`.
- [◐] Bakgrunn: `.quiz-main-content` bruker hardkodet `white`.
- [x] CTA‑områder: `.button.primary` arver token‑farger fra `css/styles.css`.
- [x] Chip/knapp‑stiler: riktig token‑bruk for korrekt/feil (`--success-color`, `--fail-color`).

## representatives.html
- [x] Banner: global `header` + `.detail-header` bruker `--brand-peach-dark`.
- [◐] Bakgrunn: paneler/kort bruker hardkodet `white`.
- [x] CTA‑områder: `.profile-link-btn` bruker `--kf-blue` og `--kf-purple`.
- [◐] Chip/knapp‑stiler: `.committee-role-badge` bruker hardkodede lilla‑toner.

## sakskompass.html
- [x] Banner/header bruker global `header`‑stil (`--brand-peach-dark`).
- [◐] Bakgrunn: `.sk-controls` og `.sk-visualization-area` bruker hardkodet `white`.
- [x] CTA‑områder: panel‑knapper (`.close-panel-btn`) bruker `--text-muted` og `--brand-blue-dark`.
- [◐] Chip/knapp‑stiler: `.stance-group` nivå‑farger er hardkodet (`#28a745`, `#ffc107`, `#dc3545`).
