# Commandes de test et identifiants

Ces commandes nécessitent les triches en solo ou les permissions opérateur
appropriées sur un serveur. Elles servent aux tests ; le jeu normal ne les exige pas.

## Entités

```mcfunction
/summon horrorbanshee:banshee ~3 ~ ~
/give @s horrorbanshee:banshee_spawn_egg
```

Forcer une des trois femmes ordinaires, sans tirage Matriarche :

```mcfunction
/summon horrorbanshee:banshee ~3 ~ ~ {LadyBanshee:0b,HumanVariant:0}
/summon horrorbanshee:banshee ~3 ~ ~ {LadyBanshee:0b,HumanVariant:1}
/summon horrorbanshee:banshee ~3 ~ ~ {LadyBanshee:0b,HumanVariant:2}
```

Matriarche humaine, puis Matriarche déjà révélée :

```mcfunction
/summon horrorbanshee:banshee ~3 ~ ~ {LadyBanshee:1b}
/summon horrorbanshee:banshee ~3 ~ ~ {LadyBanshee:1b,BansheeState:"BANSHEE"}
```

La première permet de tester la préparation complète ; la seconde inspecte
directement la forme finale et ne rejoue pas le cri initial. `LadyBanshee`
est le nom NBT conservé pour la compatibilité des sauvegardes.

## Objets

```mcfunction
/give @s horrorbanshee:banshee_tear
/give @s horrorbanshee:matriarch_tear
/give @s horrorbanshee:banshee_potion
/give @s horrorbanshee:enchanted_banshee_potion
/give @s horrorbanshee:banshee_life_essence
```

## Alambic

```mcfunction
/give @s minecraft:brewing_stand
/give @s minecraft:blaze_powder
/give @s minecraft:potion[minecraft:potion_contents={potion:"minecraft:awkward"}] 3
```

## Monde et combat

```mcfunction
/difficulty normal
/gamemode survival
/time set night
/time add 24000
/time set 23000
/gamerule doMobLoot true
```

Dans l'ordre : difficulté de combat, mode attaquable, nuit, nuit suivante,
aube et activation du butin. Ne pas exécuter toutes les commandes de temps
à la suite si l'objectif est de rester la nuit.

## Crypte

```mcfunction
/locate structure horrorbanshee:banshee_crypt
```

Attendre la réponse asynchrone. Le diagnostic `/horrorbanshee forest` est un
outil réservé au lancement développeur avec `-PforestDebug`, pas une commande
normalement disponible dans le JAR de publication.

[Accueil](Home.md) · [Dépannage](FAQ-et-depannage.md)

---
[Accueil du wiki](Home.md) · [Installation](Installation.md) · [Galerie](Galerie.md) · [Commandes](Commandes.md)
