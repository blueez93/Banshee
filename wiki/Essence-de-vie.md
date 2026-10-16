# Essence de vie de banshee

Une relique permanente qui donne la forme de la Matriarche et un vol lent
pendant la nuit.

## Obtenir l'essence

- **1 %** de chance sur une Banshee ordinaire vaincue dans les conditions du butin.
- **10 %** sur une Matriarche vaincue, à la place de sa larme légendaire.

L'objet n'est pas consommé et ne s'use pas après activation.

## Activer et voler

1. Être vivant dans l'Overworld et attendre la nuit.
2. Tenir l'essence et faire un clic droit.
3. Le joueur prend la forme de la Matriarche transformée, avec sa robe et ses cheveux blancs.
4. Utiliser les touches normales de déplacement ; **saut pour monter**, **accroupissement pour descendre**.

Le vol est maintenu par la transformation et reste soumis aux collisions.
Il est lent : vitesse de vol de base réglée à la moitié du vol Créatif vanilla.
Le pouvoir conserve les pleurs et la présentation de transformation, dont la
caméra arrière imposée et les bords sombres.

## Une fois par nuit et par joueur

La nuit admissible va des ticks solaires **13 000 à 22 999**.
La limitation est enregistrée sur **le joueur**, pas sur l'objet. Posséder deux
essences, changer de main, mourir ou se reconnecter ne redonne pas un usage
pendant la même nuit. Une nouvelle nuit rend la même essence utilisable.

## Mettre fin au pouvoir

- Refaire un **clic droit avec l'essence**.
- Attendre l'**aube**, à partir de 23 000 ticks.
- Boire du lait, mourir, quitter l'Overworld ou se déconnecter.

Arrêter ne rembourse pas l'utilisation nocturne. L'effet et la permission de
vol sont retirés, et la caméra précédente revient. **Le joueur retombe
normalement** : l'essence n'ajoute pas de chute lente après la fin du vol.

Une sauvegarde effectuée pendant l'effet conserve correctement ses données ;
le pouvoir ne peut être repris au chargement que si les conditions nocturnes
et l'autorisation enregistrée sont encore valides. Une déconnexion normale
met, elle, fin au pouvoir tout en gardant la nuit dépensée.

L'essence ne donne pas les 160 PV de la Matriarche, ni ses attaques de souffle,
ni les bonus Force/Régénération permanents de la potion enchantée.

## Essai avec commandes

```mcfunction
/give @s horrorbanshee:banshee_life_essence
/gamemode survival
/time set night
```

Si cette nuit est déjà utilisée, employer `/time add 24000` pour passer à la
nuit suivante. Pour simuler l'aube pendant le pouvoir : `/time set 23000`.
Les commandes qui réécrivent l'horloge peuvent changer le numéro de nuit considéré.

[Accueil](Home.md) · [Potions](Potions.md) · [FAQ](FAQ-et-depannage.md)

---
[Accueil du wiki](Home.md) · [Installation](Installation.md) · [Galerie](Galerie.md) · [Commandes](Commandes.md)
