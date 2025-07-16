# Projet 3 – Wild Foot Hub

Ce dépôt centralise l’ensemble des données extraites depuis FBref pour analyser les performances des joueurs de football. Chaque CSV correspond à une facette de leur jeu :

- **players.csv**  
  Fiche d’identité de chaque joueur : nom, nationalité, poste, âge. Sert de table de base pour relier toutes les autres données.

- **standard_stats.csv**  
  Statistiques globales de match : nombre de matchs joués, minutes disputées (et leur équivalent en matchs de 90 min), buts marqués, passes décisives, cartons, penalties, et métriques avancées comme xG (buts attendus) et xAG (passes attendues).  
  *Imaginez un résumé général de la saison, un peu comme la « ligne de carrière » d’un joueur.*

- **shooting_stats.csv**  
  Détail de l’activité de tir : volume total de tirs et tirs cadrés, précision, tirs par 90 min, rendement (buts par tir), distribution des tirs (distance moyenne, coups francs), et indicateurs avancés (xG pour évaluer la qualité des occasions).  
  *Cela vous dira si un attaquant est un « renard des surfaces » ou s’il enchaîne plutôt les frappes lointaines.*

- **passing_stats.csv**  
  Tout sur la distribution du ballon : passes réussies/tentées, taux de réussite, distances moyennes (totale et progressive), répartition par courte/moyenne/longue, passes clés, centres, et écart entre passes attendues et effectives (xA).  
  *Une manière de mesurer la vision du jeu et la qualité de la relance d’un milieu ou d’un défenseur relanceur.*

- **pass_types_stats.csv**  
  Répartition détaillée par type de passe : passes en jeu, sur phases arrêtées, corners, passes en profondeur, switch (changement d’aile), etc.  
  *Utile pour voir si un joueur est spécialiste des coups francs, des centres millimétrés ou des relances longues.*

- **goal_shot_creation.csv**  
  Actions créatrices : SCA (actions qui débouchent sur un tir) et GCA (actions qui débouchent sur un but), normalisées par 90 min, et ventilées selon leur origine (passes, dribbles, fautes provoquées, etc.).  
  *Idéal pour repérer ceux qui « font bouger les lignes » avant même de tirer ou marquer.*

- **defense_stats.csv**  
  Statistiques défensives : tacles (tentés, réussis, localisation sur le terrain), duels (gagnés, perdus), interceptions, contres, dégagements, erreurs aboutissant à un but adverse, et efficacité en un-contre-un.  
  *Pour identifier les véritables « stoppeurs » et leurs points forts/faibles dans la récupération du ballon.*

- **possession_stats.csv**  
  Données de possession : touches de balle (zones du terrain), dribbles tentés/réussis, pertes de balle, portées (progressions balle au pied), réceptions, etc.  
  *Permet de mesurer l’influence d’un joueur sur la maîtrise du ballon et la construction du jeu.*

- **playing_time_stats.csv**  
  Temps de jeu et impact (« On–Off ») : minutes jouées, titularisations, entrées en jeu, et indicateurs d’influence sur le score et l’xG de l’équipe quand le joueur est sur le terrain ou non.  
  *Donne une idée de l’importance de chaque joueur pour son équipe, au-delà des simples statistiques individuelles.*

- **goalkeeper_stats.csv**  
  Performances des gardiens : buts encaissés, arrêts, pourcentage d’arrêts, clean sheets, xG sur tirs cadrés, performance par rapport au xG, interventions hors surface, relances, etc.  
  *Pour dresser le portrait du gardien, de ses réflexes aux multiples facettes de son jeu au pied et son positionnement.*

---

## Structure du dépôt

├── data/
│ ├── standard_stats.csv
│ ├── shooting_stats.csv
│ └── …
├── notebooks/
│ ├── scraping_fbref.ipynb
│ └── test_fbref.ipynb
├── .gitignore
└── README.md

