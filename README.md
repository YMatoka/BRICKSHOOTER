# BRICKSHOOTER
Jeu BrickShooter

Pour lancer le jeu il faut RUN le module "brickShooter.py"

Répartition des tâches de dévelopepemnt:

YANN :  brickshooter.py  ==> Menu principal (affichage regle, choix equipement,sauvegaDE)

gameComponents   ==> Creation composant du jeu (joueur, ennemies, terrain, missile) Ecran Fin de Partie / Sauvegarde score et crédit


VOLKAN : collision.py ==> gere  la collision entre les  divers composants du jeu (joueur, ennemies, missile)


PRESLEY : playerMoves.py ==> gere les mouvements du joueur (gauche , droite)
          
bulletMoves.py ==> gere les mouvements des balles (bas vers la limite haute de l'écran)

STEPHEN : ennemiesMoves.py : gere les mouvements des ennemies ( haut vers le bas de l'écran en se déplacant de gauche a doite)
	        
main.py  ==> gere le deroulement du jeu (boucle sur le déroulement du jeu en se servant des divers module réalisés)


Dérouelement du Jeu BRICK SHOOTER:

Le Jeu comprend une premiere interface graphique où le joueur peut realiser diverses actions:

-Lire les regles du jeu
-quitter le jeu
-Choisir son equipement

Une fois arrivé a l'écran de choix d'equipement, si le joueur a gagné précédemment des crédits,
il pourra s'en servir pour ameliorer ou diminuer la vitesse de son vaisseau ou de ses missiles
en cliquant sur les boutons adequats.

S'il a assez de crédit un pop up previendra le joueur qu'il a ffectuerun changement,auquel cas il
previendra l'utilisateur qu'il n'en a pas assez.

En cliquant sur jouer,le jeu se lance. Si un des ennemis le touche ou s'il quitte la partie, l'ecran
de fin de partie apparait et récapitule le score actuelle et le meilleur score du joueur.

La partie est sauvegardé dans un fichier txt nommé sauvegarde.txt.
