# Déroulement d'une rencontre

## Une femme apparemment normale

La Banshee apparaît d'abord sous une apparence humaine. Elle n'attaque pas :
elle marche, s'arrête, regarde autour d'elle et peut observer un joueur proche.
Elle peut chantonner en se déplaçant en forêt. Il n'y a pas de dialogue.

## Trois façons de la révéler

- Faire un **clic droit** sur elle.
- Lui infliger un **coup** en tant que joueur, si elle survit.
- La viser directement pendant **plus de cinq secondes consécutives**.

Le regard est testé à partir du viseur, jusqu'à **32 blocs**, avec les obstacles
et les autres entités pris en compte. Un arbre, un mur ou un regard détourné
interrompt la durée accumulée. Le mode Spectateur ne déclenche pas la rencontre.

## Pleurs, course et flashs

Une première vision très brève laisse entrevoir son vrai visage. Elle reprend
une apparence humaine, commence à pleurer, puis s'élance dans une course de
plus en plus rapide. Les changements de peau sont irréguliers : il ne s'agit
pas d'un clignotement à fréquence fixe.

Elle cherche des trajectoires praticables autour du joueur et peut utiliser
les arbres pour casser la ligne de vue. Pendant cette préparation, elle
n'effectue pas encore ses attaques de mêlée.

| Étape | Durée normale, à 20 ticks/s |
| --- | --- |
| Pleurs initiaux | 2,5 s |
| Frénésie et course | 8 à 12 s |
| Transformation finale | 1,2 s |
| Cri et pose, mains relevées | 5,15 s |

Les interactions supplémentaires ne recommencent pas la séquence. L'état est
enregistré pour qu'un rechargement du monde ne remette pas la rencontre à zéro.

## Après le cri

Sa forme monstrueuse reste visible et l'agression commence. Les Banshees
ordinaires poursuivent et attaquent au corps à corps. La Matriarche possède
son propre [combat aérien](Matriarche.md). Le joueur déclencheur est prioritaire
lorsqu'il peut être attaqué. Les joueurs Créatif et Spectateur ne sont pas
des victimes de combat.

Un bref effet d'Obscurité peut accompagner la révélation du joueur visé.
Le cri fait partie de la rencontre ; ce n'est pas un effet répété à chaque
attaque. Si la Banshee tue un joueur, celui-ci entend son rire de victoire.

[Accueil](Home.md) · [Banshees](Banshees.md) · [Matriarche](Matriarche.md)

---
[Accueil du wiki](Home.md) · [Installation](Installation.md) · [Galerie](Galerie.md) · [Commandes](Commandes.md)
