# Générateur de décors OPR

Outil web, en un seul fichier HTML, qui tire des décors et propose une mise en place du plateau pour **Age of Fantasy** et **Grimdark Future** (One Page Rules), à partir des règles avancées v3.6.0.

> Projet de fan, non officiel et non affilié à One Page Rules. Les règles, noms et marques appartiennent à leurs propriétaires.

## Utilisation

1. Télécharger `generateur-decors-opr.html` et l'ouvrir dans un navigateur récent (aucune installation, aucun serveur).
2. Choisir le jeu, la taille de table, le style de placement, le générateur de décors et la taille des grandes pièces.
3. Cliquer sur **Générer**, puis exporter en PDF ou en SVG.

Pour le publier en ligne, activer GitHub Pages sur le dépôt (Settings → Pages) en pointant vers la branche principale.

## Fonctionnalités

- **Deux jeux** : la police, les noms et les icônes des décors changent selon le jeu (par exemple bâtisse ou tour en Fantasy, bâtiment ou bloc industriel en Grimdark Future).
- **Tables** : 6'x4', 4'x4' et 3'x3', avec les dimensions en pouces et en centimètres.
- **Quatre générateurs de décors** des règles avancées (Générique, Hospitalier, Désolation, Mortel) et un mode Libre avec un nombre de pièces au choix.
- **Six styles de placement** : Aléatoire, Alternée (libre), Alternée (restreinte, avec ses six restrictions), Table entière, Deux moitiés, Six carrés. Le style peut être tiré au hasard (1D6).
- **Règle des 6"** : les pièces doivent rester à plus de 6" (15 cm) les unes des autres ; les pièces qui ne trouvent pas de place sont retirées et listées.
- **Formes naturelles** aléatoires pour les décors naturels (forêts, collines, lacs, rivières sinueuses, etc.). Les bâtiments, murs et barricades restent rectangulaires. Les dimensions affichées sont celles du rectangle englobant.
- **Tailles des grandes pièces** réglables : 4–8", 5–10" ou 6–12". Les tailles sont arrondies aux pouces et aux centimètres entiers.
- **Pièces dangereuses** désignées automatiquement, avec un contour rouge en pointillé sur le plan.
- **Contrôles** : recommandations de couvert, de terrain difficile, de blocage de vue et de surface, avec deux indicateurs d'équilibre entre les moitiés de table. Une case permet de relancer jusqu'à un équilibre correct.
- **Ma collection** : voir la section suivante.
- **Exports** : PDF (impression du navigateur, A4 portrait) et SVG avec les mêmes informations.

## Ma collection de décors

Dans la zone dépliable « Ma collection de décors », chaque joueur saisit les pièces qu'il possède : type, nom (facultatif), longueur et largeur en cm, quantité.

- Choisir la source « Ma collection » : le générateur détermine les types de décors demandés, puis chaque type est pioché dans la collection (une pièce n'est utilisée qu'une fois par table).
- Les pièces sont posées en rectangles à leurs dimensions réelles.
- Si un type manque, la case « Compléter avec des pièces génériques » décide si l'outil le remplace par une pièce abstraite ou l'ignore.
- La collection est enregistrée dans le navigateur (localStorage). Elle peut être exportée et importée en JSON pour la partager ou la sauvegarder.

## Hypothèses et limites

Source : GF / AoF Advanced Rulebook v3.6.0 (placement, générateurs de terrain, recommandations).

- Les pièces sont placées de la plus grande à la plus petite, à des emplacements tirés au hasard par le code (les joueurs choisiraient).
- Style « Aléatoire » : la pièce part du centre d'une zone et avance jusqu'à 2D6" vers le centre d'une autre zone, en s'arrêtant avant de passer à 6" ou moins d'une pièce. C'est une interprétation de la règle, et ce style retire souvent beaucoup de pièces.
- Dans le PDF du Grimdark Future, le tableau du générateur Désolation n'a pas d'entrée 4 ; celle du PDF d'Age of Fantasy est appliquée aux deux jeux.
- Les noms et icônes thématiques varient selon le jeu, mais les effets de règle restent ceux des tableaux.
- Les contrôles d'équilibre gauche-droite et haut-bas sont une heuristique de l'outil, pas une règle.
- La surface de 25 % recommandée est rarement atteinte avec l'écart de 6" (environ 19 % au maximum sur 6'x4' avec les pièces 6–12").
- Les icônes sont des emojis : leur rendu dépend du système. Sur de très petites pièces, les numéros peuvent se chevaucher.
- Les polices (Orbitron, IM Fell English) sont chargées depuis Google Fonts ; hors connexion, des polices de repli sont utilisées, y compris dans l'export SVG.
- Pour le PDF, désactiver les en-têtes et pieds de page et activer les graphiques d'arrière-plan dans la fenêtre d'impression.

## Feuille de route

- **Phase 2** : photos des décors des joueurs, affichées sur le plan à la place des icônes abstraites.

## ⚠️ À propos des droits

Ce dépôt contient des éléments dérivés de l'**Advanced Rulebook** d'OPR Games (noms et composition des tableaux de décors, recommandations de terrain), un contenu proposé via leur Patreon (donc non gratuit). Cet outil est un projet de fan, non affilié à OPR Games.

## Licence

Le code (HTML/CSS/JS) de cet outil peut être réutilisé librement. Cette licence ne s'étend pas au contenu textuel et graphique des règles OPR Games intégré dans l'outil, qui reste la propriété d'OPR Games.
