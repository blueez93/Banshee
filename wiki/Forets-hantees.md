# Les forêts hantées

![Progression réelle du brouillard](../media/brouillard-comparatif.webp)

De gauche à droite : forêt sans brume, apparition progressive, brouillard dense.
Ces captures de validation ont été réalisées pendant la Phase 4A (0.7.0),
sans shaders. [Voir les captures originales](Galerie.md#le-brouillard-des-forêts-hantées).

Certaines grandes taïgas vanilla reçoivent une atmosphère hantée : la brume se
renforce progressivement, la visibilité diminue et de rares voix se font entendre.
Le biome reste vanilla, y compris dans F3 ; aucun bloc ni arbre spécial n'est
ajouté par ce système.

## Biomes concernés

- `minecraft:taiga`
- `minecraft:old_growth_pine_taiga`
- `minecraft:old_growth_spruce_taiga`

La classification vise de grands ensembles d'environ **300 blocs dans les
deux directions**. Elle utilise une grille et une approximation géographique
bornée, pas un comptage précis de chaque arbre. Les petits îlots sont écartés.

Un tirage déterministe de 50 % choisit parmi les ensembles admissibles : cela
ne signifie pas que la moitié exacte de chaque monde devient hantée. Le résultat
dépend de la graine et de la géographie, et reste stable lors des recalculs
avec les mêmes règles. Couper quelques arbres ne désactive pas la zone.

## Entrer et sortir

Les premières secondes restent normales. La brume monte sur environ quinze
secondes et dépend aussi de la profondeur dans la forêt. Une brume basse
complète le brouillard de distance. Sortir le fait disparaître progressivement,
environ deux secondes après détection. Aucun bandeau ne révèle la présence
d'une « zone hantée » au joueur.

Ce n'est ni un nouveau biome ni une nuit artificielle permanente. L'eau, la
lave et les effets comme Cécité ou Obscurité conservent leurs priorités de rendu.
Avec les particules minimales, les nappes de brume sont désactivées, pas tout
le brouillard de distance.

## Des sons volontairement rares

Après l'entrée dans une zone suffisamment profonde et admissible :

- premier son après **2 à 4 minutes** ;
- ensuite **5 à 10 minutes entre deux ambiances**, toutes catégories confondues ;
- murmures, chants, pleurs lointains, et un drone plus profondément dans la forêt.

Une seule ambiance joue à la fois ; les rencontres et transformations sont
prioritaires. Le rire de victoire n'appartient pas au catalogue forestier.
Le silence fait partie du rythme normal du mod.

## À distinguer des apparitions de Banshees

En 0.11.1, les apparitions naturelles de Banshees ciblent les quatre biomes
forestiers listés dans [Banshees](Banshees.md). Le système de taïga hantée
est distinct et n'ajoute pas à lui seul des Banshees dans ces trois taïgas.

[Accueil](Home.md) · [Audio](Audio.md) · [FAQ](FAQ-et-depannage.md)

---
[Accueil du wiki](Home.md) · [Installation](Installation.md) · [Galerie](Galerie.md) · [Commandes](Commandes.md)
