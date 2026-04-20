# Design by Cloé — Site Vitrine

> Partenaire stratégique et créative en communication à Charleville-Mézières, Ardennes.

## Présentation

Site vitrine professionnel de **Design by Cloé**, micro-entreprise de graphisme freelance et communication stratégique fondée par Cloé Laurin. Le site présente les services, le portfolio, les informations de contact et les pages légales.

**URL de production :** [https://designbycloe.fr](https://designbycloe.fr)

---

## Structure du projet

```
designbycloe.fr/
├── index.html              # Page d'accueil
├── services.html           # Détail des prestations
├── portfolio.html          # Réalisations clients
├── a-propos.html           # Présentation, valeurs, outils
├── contact.html            # Coordonnées et réseaux sociaux
├── mentions-legales.html   # Mentions légales obligatoires
├── cgv.html                # Conditions générales de vente
├── confidentialite.html    # Politique de confidentialité / RGPD
├── 404.html                # Page d'erreur personnalisée
├── style.css               # Feuille de styles globale
├── script.js               # JavaScript (loader, menu, reveal, compteurs)
├── .htaccess               # Configuration Apache (sécurité, redirections, cache)
├── robots.txt              # Directives pour les robots d'indexation
├── sitemap.xml             # Plan du site pour les moteurs de recherche
├── security.txt            # /.well-known/security.txt — contact sécurité
├── README.md               # Ce fichier
└── img/
    ├── Cloe_Laurin.jpg
    ├── logo_horizontal.png
    ├── logo_principal.png
    ├── logo_principal_2.png
    ├── logo_rb.jpg
    ├── logo_ad.jpg
    ├── logo_apero.jpg
    ├── logo_cmt.jpg
    ├── logo_secouriste.jpg
    ├── gestion_RS_RB.jpg
    ├── Gestion_RS_buddy.jpg
    ├── gestion_RS_RT.jpg
    ├── affiche_SP.jpg
    ├── flyer_ad.jpg
    ├── flyer_friterie.jpg
    └── Tee_shirt_cR.jpg
```

---

## Stack technique

| Élément        | Technologie                          |
|----------------|--------------------------------------|
| Langages       | HTML5, CSS3, JavaScript ES6 (vanilla)|
| Typographies   | Montserrat, DM Sans (Google Fonts)   |
| Hébergement    | Serveur Apache (OVH / autre)         |
| Certificat SSL | Let's Encrypt (ou inclus hébergeur)  |
| Versioning     | Git                                  |

---

## Palette de couleurs

| Nom         | Hex       | Usage                        |
|-------------|-----------|------------------------------|
| Blue Light  | `#afc1ed` | Accents secondaires, fonds   |
| Blue Mid    | `#6296f7` | Liens, éléments interactifs  |
| Blue Pale   | `#f0f2f9` | Arrière-plans de sections    |
| Coral       | `#f76c5e` | CTA, accents principaux      |
| Blue Dark   | `#2321bc` | Titres, navigation, footer   |
| White       | `#ffffff` | Fond de cartes               |
| Black       | `#1a1a2e` | Texte principal              |

---

## Déploiement

### Mise en ligne (FTP / SSH)

1. Transférer **tous les fichiers** à la racine du dossier `www/` ou `public_html/` de l'hébergement.
2. S'assurer que le fichier `.htaccess` est bien uploadé (fichier caché).
3. Vérifier que le certificat SSL est actif (HTTPS obligatoire).
4. Tester toutes les pages et le formulaire de contact.

### Vérifications post-déploiement

- [ ] Toutes les pages chargent en HTTPS sans erreur
- [ ] Le fichier `.htaccess` redirige HTTP → HTTPS
- [ ] La page 404 personnalisée s'affiche pour les URLs inexistantes
- [ ] Le `robots.txt` est accessible à `https://designbycloe.fr/robots.txt`
- [ ] Le `sitemap.xml` est accessible et soumis à Google Search Console
- [ ] Les images sont toutes visibles (pas de 404 sur les images)
- [ ] Le site est responsive (tester mobile, tablette, desktop)
- [ ] Les performances sont correctes (PageSpeed Insights > 90)

---

## SEO

- Chaque page possède un `<title>` unique et une `<meta description>` descriptive.
- URL canonique définie via `<link rel="canonical">`.
- Balises Open Graph renseignées sur la page d'accueil.
- `sitemap.xml` généré pour la soumission à Google Search Console.
- `robots.txt` configuré pour autoriser l'indexation complète.

---

## Sécurité

Le fichier `.htaccess` inclut :
- Redirection HTTP → HTTPS
- Headers de sécurité (X-Frame-Options, X-Content-Type-Options, CSP, Referrer-Policy, Permissions-Policy)
- Protection contre le hotlinking des images
- Désactivation du listing des répertoires
- Protection des fichiers sensibles (.htaccess, .git, etc.)
- Mise en cache des assets statiques

---

## Maintenance

- **Mise à jour du contenu** : éditer directement les fichiers HTML.
- **Ajout d'un projet au portfolio** : ajouter un `<div class="portfolio-item">` dans `portfolio.html` avec la bonne `data-category`.
- **Modification des couleurs** : changer les variables CSS dans `:root` de `style.css`.

---

## Crédits

- **Design & développement** : Cloé Laurin — Design by Cloé
- **Photos portrait** : Laura Vergne
- **Typographies** : Google Fonts (Montserrat, DM Sans)

---

## Contact

- **Email** : designbycloe@outlook.fr
- **Téléphone** : 06 02 18 61 01
- **Instagram** : [@designbycloe.fr](https://www.instagram.com/designbycloe.fr/)
- **LinkedIn** : [Design by Cloé](https://www.linkedin.com/company/design-by-cloe/)

---

## Licence

© 2026 Design by Cloé — Tous droits réservés.
Toute reproduction ou utilisation du contenu de ce site sans autorisation écrite est interdite.
