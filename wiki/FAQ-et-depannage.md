# FAQ et dépannage

## La femme ne m'attaque pas

C'est son comportement humain normal. Un clic droit, un coup non mortel ou un
regard direct de plus de cinq secondes déclenche la rencontre. Elle ne frappe
pas pendant les pleurs, la frénésie ou la pose du cri. Passer en Survie pour
tester le combat : Créatif et Spectateur ne sont pas des cibles de chasse.

## Le regard ne la transforme pas

Viser réellement sa boîte de sélection à 32 blocs maximum et garder le viseur
dessus sans interruption. Un obstacle ou une autre entité peut masquer le rayon.
Le mode Spectateur ne compte pas. Une rencontre déjà commencée ne se relance pas.

## Aucun son dans ma forêt

Vérifier les volumes Minecraft. Le système hanté vise les trois grands biomes
de taïga listés dans [Forêts hantées](Forets-hantees.md), pas toutes les forêts.
Une zone doit être assez grande, choisie par la graine, et le joueur assez
profond. Les délais de plusieurs minutes sont normaux. Le rire est uniquement
un son de victoire sur le joueur, jamais une ambiance aléatoire.

## Aucune crypte trouvée

Explorer de nouveaux chunks de l'Overworld avec les structures activées.
Les montagnes avec de l'eau restent seulement des candidates. `/locate` peut
prendre du temps et s'arrête après 90 secondes : attendre sa réponse, puis
réessayer depuis une autre région. Un monde superplat ou un terrain très
modifié n'offre pas nécessairement les conditions requises.

## Plus aucun chunk ne charge après une ancienne commande /locate

Mettre à jour une ancienne version du mod : la recherche de crypte est
asynchrone depuis 0.6.2. La version documentée 0.11.1 inclut ce correctif.
Après mise à jour, conserver `latest.log` si le problème persiste ; ne pas
confondre une recherche sans résultat avec une fermeture réelle du jeu.

## Une Banshee n'a rien laissé à sa mort

Les chances ne garantissent pas un objet ordinaire. La créature doit être
révélée, tuée par un joueur et `doMobLoot` actif. Voir [les taux exacts](Objets-et-butin.md).
Une Matriarche admissible donne l'un de ses deux objets spéciaux.

## Impossible de brasser la potion

Utiliser une **potion étrange buvable**, l'ingrédient correct et du combustible
Blaze. Les fioles d'eau, potions jetables et recettes de redstone ne remplacent
pas [les recettes prévues](Potions.md).

## La potion bloque F5

C'est prévu. Les deux potions et l'essence imposent leur vue arrière pendant
la transformation, avec une bordure sombre. La perspective précédente revient
à l'arrêt. Le lait permet d'écourter le pouvoir.

## L'essence ne marche plus cette nuit

L'usage est limité par joueur : un arrêt volontaire, le lait, la mort ou la
déconnexion ne rendent pas l'activation. Attendre la prochaine nuit. En test,
`/time add 24000` avance d'une nuit ; remettre simplement la même heure nocturne
ne constitue pas nécessairement une nouvelle nuit.

## Les cheveux semblent encore se détacher

La version 0.11.1 rattache les mèches avant et arrière de la Matriarche humaine
et transformée à la tête. Retirer l'ancien JAR, garder une seule version et
redémarrer complètement le jeu pour charger la nouvelle géométrie.

## Signalement utile

Sur les [issues GitHub](https://github.com/blueez93/Banshee/issues), joindre :
la version Minecraft/NeoForge/GeckoLib/mod, la liste des autres mods, les étapes
pour reproduire, `latest.log` et le rapport de crash s'il existe. Pour un souci
de génération, ajouter la graine et les coordonnées. Masquer les informations
personnelles ou adresses de serveur privées avant d'envoyer un journal.

[Accueil](Home.md) · [Installation](Installation.md)

---
[Accueil du wiki](Home.md) · [Installation](Installation.md) · [Galerie](Galerie.md) · [Commandes](Commandes.md)
