# Portfolio Epitech — Melda ASLAN

Après un Master en Ressources Humaines et des expériences chez Castorama et American Vintage, je me reconvertis dans l’informatique à Epitech Paris. Étudiante en Pré-MSc, je m’intéresse au développement logiciel, au Cloud et au DevOps. Ce portfolio présente mon parcours, mes projets et mes apprentissages. Je recherche une alternance en développement Full Stack à partir de janvier 2027.

## Technologies

Site statique en **HTML5 et CSS3**, sans JavaScript, framework, PHP, backend applicatif ni compilation. Flexbox, Grid et les media queries adaptent la mise en page. Le formulaire utilise le service externe FormSubmit.

## Lancement local

Depuis le dossier du projet :

```bash
cd /home/zeldaketur/epitech/Portfolio
python3 -m http.server 5500
```

Ouvrir http://localhost:5500/ ; arrêter le serveur avec `Ctrl+C`. Python sert uniquement à la prévisualisation. Utiliser HTTP plutôt que `file://` pour le formulaire ; FormSubmit et les liens externes nécessitent une connexion Internet.

## Structure du projet

| Fichier ou dossier | Contenu |
| --- | --- |
| `index.html` | One Page : Accueil, À propos, Parcours, Projets et Contact. |
| `about.html` | Présentation, compétences, langues et mise en pratique. |
| `parcours.html` | Formations, expériences et missions RH détaillées. |
| `projets.html` | Projets, contribution personnelle et apprentissages. |
| `contact.html` | Formulaire, coordonnées, CV et informations pratiques. |
| `assets/css/style.css` | Styles communs, responsive et accessibilité. |
| `assets/documents/Melda_Aslan_CV.pdf` | CV téléchargeable. |
| `assets/images/` | Portrait, capture du Job Board, illustrations, logos et icônes. |

Le menu mène aux ancres `#accueil`, `#about`, `#parcours`, `#projets` et `#contact` de l’accueil. Depuis les pages distinctes, les liens utilisent `index.html#…`. Les boutons « En savoir plus » ouvrent les détails des projets ; les autres pages restent accessibles directement par leur nom de fichier.

Le header sticky et le défilement fluide gardent les titres visibles. Les préférences de réduction des mouvements sont respectées. Pour maintenir le site, répercuter les changements communs dans l’accueil et la page détaillée concernée.

## Projets

| Projet | État | Présentation |
| --- | --- | --- |
| Job Board — M&A Corporation | Réalisé en binôme | Plateforme de recrutement avec React, FastAPI et SQLite. |
| NFL Big Data Bowl | Réalisé en équipe | Exploration de données sportives et visualisations avec Python, pandas et matplotlib. |
| Hospital DevOps Platform | En développement | Backend FastAPI/PostgreSQL, conteneurisation Docker et mise en place progressive de CI/CD avec GitHub Actions. |
| Cloud Cost Monitoring & Alerting | Terminé | Détection d’anomalies sur des coûts simulés, alertes e-mail et sécurisation des secrets. |
| Docker Mini App | Terminé | Application web à trois tiers avec Flask, PostgreSQL et Nginx, orchestrée avec Docker Compose. |
| DevOps Cloud CI/CD | Envisagé | Exploration de l’automatisation de la construction et du déploiement d’une application. |

Sur le Job Board, ma contribution concerne **AdCard, AdList, l’intégration des données API, Header/Footer et le CSS**. La page détaillée explique l’affichage des données dans React et distingue mon travail des fonctionnalités collectives.

Dépôt : [Job Board](https://github.com/Aure-0411/Job_Board). Les technologies citées décrivent les projets, sans présumer un niveau d’expertise. DevOps Cloud CI/CD reste une piste distincte du travail déjà engagé sur Hospital.

## CV et contact

Le CV est téléchargeable depuis l’accueil et les coordonnées Contact grâce à des liens HTML avec `download`.

Les formulaires de `index.html` et `contact.html` fonctionnent via **FormSubmit** : envoi POST vers `https://formsubmit.co/meldaaslan@outlook.fr`, avec prénom, nom, email, sujet et message obligatoires. L’email du visiteur fournit le Reply-To ; `_subject` définit le titre du courriel. reCAPTCHA est activé par défaut.

**L’envoi a été testé avec succès : j’ai reçu le message dans Outlook.** Après un changement d’hébergement, refaire un test de réception et contrôler l’adresse proposée par Répondre. Si FormSubmit demande une activation, suivre le lien reçu par email puis renouveler l’envoi.

Les données sont traitées par FormSubmit, qui affiche sa page de confirmation. [Documentation](https://formsubmit.co/documentation) · [Aide](https://formsubmit.co/help).

## Accessibilité et tests

HTML sémantique, un H1 par page, textes alternatifs, lien d’évitement, labels et focus clavier visible. Les détails utilisent `details` et `summary` natifs. Le CSS prend en compte la réduction des mouvements et les couleurs forcées.

Contrôles effectués :

- **Navigation** : liens locaux et ancres présents, aucun identifiant dupliqué ; défilement vers Projets sous le header et ouverture des détails vérifiés.
- **Responsive** : cinq pages contrôlées à 360, 768 et 1280 px, sans débordement horizontal détecté.
- **CV** : trois liens de téléchargement vérifiés, transfert HTTP réussi et PDF lisible, identique au fichier original.
- **Formulaire** : champs requis, labels et validation d’email contrôlés ; réception du message de test confirmée dans Outlook.

Ces tests ciblés ne constituent pas une certification d’accessibilité et ne garantissent pas la disponibilité future des services externes.

## Dépôt et publication

Dépôt Epitech : `T-ENT-500-PAR-5-1-portfolio-26`.

Le site est compatible avec GitHub Pages ou tout hébergement statique, sans compilation. Il n’est pas encore publié ; aucune URL GitHub Pages n’est définie. Le premier push et le déploiement restent à effectuer.

Pour la remise Epitech, le portfolio conserve cinq pages et les apprentissages dans les projets. Le cahier des charges PDF n’est pas inclus : les exigences d’accès aux pages distinctes, de progression, de crédits visibles et de publication restent à comparer au document officiel.

## Crédits et ressources

Maquettes, portrait, capture du Job Board et CV fournis par **Melda ASLAN**. Portrait sans retouche dans `assets/images/melda-portrait-bureau.png` ; capture réelle dans `assets/images/job-board.png`. Logo MA en texte et dégradé CSS, police système Arial. © 2026 Melda ASLAN.

Les visuels NFL et Cloud/DevOps sont des **illustrations conceptuelles créées avec ImageGen**, légendées sur le site, et non des captures d’applications. Fichiers : `assets/images/projects/{nfl,hospital,cloud-cost,docker}-maquette-v2.png` et `cicd.png`. Prompts conservés dans `assets/images/projects/PROMPTS-MAQUETTE-V2.txt` et `PROMPTS.txt`.

### Icônes et drapeaux

| Ressource | Auteur et licence | Fichiers locaux |
| --- | --- | --- |
| [Devicon](https://github.com/devicons/devicon) | konpa et contributeurs — MIT | `assets/images/devicon/` : `LICENSE.txt`, `SOURCE.txt` |
| [CoreUI Free Icons](https://github.com/coreui/coreui-icons) | CoreUI — [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) | `assets/images/coreui/` : `LICENSE.txt`, `SOURCE.txt` |
| [Flagpack Core](https://github.com/Yummygum/flagpack-core) | Yummygum — MIT | `assets/images/flagpack/` : `LICENSE.txt`, `SOURCE.txt` |

Les fichiers `SOURCE.txt` consignent les versions exactes. CoreUI : couleur adaptée en violet `#7021ff`, géométrie conservée et attribution dans les SVG. Devicon et Flagpack : SVG non modifiés ; SQL utilise l’icône SQLite. Les images accompagnant un libellé ont un `alt` vide pour éviter une lecture répétée.

### Logos du parcours

Fichiers locaux dans `assets/images/logos/`, couleurs et proportions conservées. Sources :

- **Epitech** : [site officiel](https://www.epitech.eu/wp-content/uploads/2023/10/logo-epitech.svg).
- **IAE Toulon** : [fichier source](https://commons.wikimedia.org/wiki/File:Logo_iae_toulon.png), auteur IAE de Toulon, [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Fichier non modifié, dimensions d’affichage adaptées par CSS.
- **Paul-Valéry** : [site officiel](https://www.univ-montp3.fr/sites/default/files/logo_udmpv.jpg).
- **Lycée Marie France** : extrait de la maquette fournie par Melda, `marie-france-maquette.png` ; résolution limitée à celle de la maquette.
- **Castorama** : [fichier source](https://commons.wikimedia.org/wiki/File:Castorama_-_logo_(France,_2014-).svg), indiqué PD-textlogo ; marque protégée.
- **American Vintage** : [site officiel](https://www.americanvintage-store.com/on/demandware.static/Sites-AMV-Site/-/default/dw0bddf59f/medias/images/logo-dark.svg).
- **Groupe AGPM** : [site officiel](https://www.agpm.fr/images/logos/agpm/logo-groupe-agpm-sticky.png).
- **BNP Paribas** : [fichier source](https://commons.wikimedia.org/wiki/File:BNP_Paribas_logo.svg), auteur BNP Paribas, indiqué domaine public pour la géométrie ; marque protégée.
- **UNICEF** : [site officiel](https://www.unicef.org/sites/default/files/styles/inverse_logo/public/English-Inverse_39.png.webp?itok=iCH1Z0yX).

Les marques appartiennent à leurs titulaires. Elles identifient les technologies et organismes présentés, sans suggérer leur soutien au portfolio.
