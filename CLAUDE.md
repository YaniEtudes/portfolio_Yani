# Portfolio de Yani Nait Chabane

Site perso en un seul fichier `index.html` (HTML, CSS et JS vanilla, Three.js r128 via cdnjs).
Pas de build, pas de npm. Déployé par GitHub Pages depuis `main` (racine).
Repo : github.com/YaniEtudes/portfolio_Yani

## Règles
- Tout le texte est en français, ton direct d'étudiant, pas de tirets cadratins.
- Formulations neutres en genre (pas de "étudiant / étudiante" ni d'accords sur le sujet).
- Confidentialité du stage FCN : aucun nom de collaborateur, aucun nom de logiciel interne, aucun chiffre d'audit, aucune capture. Seuls les outils génériques (Microsoft 365, Entra ID, PIM, MFA) sont cités.
- Les infos perso (email, LinkedIn) se règlent dans l'objet `CONFIG` au début du `<script>`. Ne rien coder en dur ailleurs.
- Ne jamais inventer une compétence ou un projet : si une info manque, poser la question.

## Design (thème "Night Session")
- Tokens dans `:root` : fond #0C0F16, accent ambre #E0743C, teal #3ABFB0.
- Polices : Cormorant Garamond italique (titres), Outfit (texte), JetBrains Mono (labels).
- Chaque projet a sa couleur (`--c` en RGB sur la carte) et un petit motif animé dans la vignette.
- Pas d'emoji, pas de lib en plus sans vraie raison.
- Respecter `prefers-reduced-motion`. Mobile d'abord : tester à 375 px de large.
- Three.js : la boucle de rendu doit se mettre en pause hors écran et onglet caché.

## Avant chaque commit
1. `python -m http.server 8000` puis ouvrir http://localhost:8000
2. Console du navigateur sans erreur, test mobile 375 px, menu burger OK.
3. Commit court en français, push sur `main`.

## Idées d'amélioration (backlog)
1. Vraies captures ou GIF des projets dans `assets/` (webp, moins de 200 Ko chacun).
2. Vidéo démo de la Salle des Armes (intégration en lazy loading).
3. Page ou modale de détail par projet.
4. CV en PDF téléchargeable.
5. Image Open Graph pour les aperçus de lien, score Lighthouse supérieur à 90.
6. Photo de profil (portrait, fond neutre) dans la section À propos.
