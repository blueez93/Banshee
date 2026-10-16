# Installation et compatibilité

| Élément | Version documentée |
| --- | --- |
| Jeu | Minecraft **Java Edition 1.21.1** |
| Chargeur | **NeoForge 21.1.256** ; le mod déclare la branche 21.1 à partir de cette version |
| Java | **21** |
| Bibliothèque | **GeckoLib pour NeoForge 1.21.1**, version testée **4.9.3** |
| Horror Banshee | **0.11.1** |

## Installation sur le client

1. Installer une instance Minecraft Java 1.21.1 avec NeoForge.
2. Fermer le jeu.
3. Placer `horrorbanshee-0.11.1.jar` et GeckoLib compatible dans le dossier `mods` de cette instance.
4. Retirer l'ancien JAR Horror Banshee pour ne conserver qu'une seule version.
5. Démarrer l'instance NeoForge.

GeckoLib n'est pas inclus dans le JAR. La dépendance déclarée accepte les
versions GeckoLib 4 à partir de 4.9.3 ; 4.9.3 reste la version vérifiée ici.
Le mod ne fonctionne pas comme pack de ressources ou datapack autonome.

## Serveur

Installer Horror Banshee et GeckoLib **sur le serveur et sur les clients**.
Utiliser des versions correspondantes. Le serveur choisit les variantes,
gère les rencontres, les récompenses et la permission de vol nocturne.

Le projet comporte des tests serveur et des scénarios avec serveur intégré.
Une compatibilité universelle avec tous les modpacks et générateurs de terrain
n'est pas revendiquée.

## Monde existant

Les entités et objets peuvent être utilisés dans un monde existant.
Les cryptes se génèrent dans de **nouveaux chunks**, dans l'Overworld, avec la
génération des structures activée. Elles ne sont pas ajoutées rétroactivement
à une zone déjà explorée.

## Ce qui n'est pas pris en charge

- Minecraft Bedrock Edition.
- Chargement direct sous Fabric, Quilt ou Forge à la place de NeoForge.
- Une autre version Minecraft simplement parce qu'elle porte aussi le numéro 1.21.

Le dépôt contient la documentation et la galerie. La présence d'un JAR dans
une section de téléchargement ne doit pas être déduite d'une image de présentation.
Les liens de distribution seront ajoutés lors de la publication du mod.

[Accueil](Home.md) · [Première rencontre](Rencontres.md) · [Dépannage](FAQ-et-depannage.md)

---
[Accueil du wiki](Home.md) · [Installation](Installation.md) · [Galerie](Galerie.md) · [Commandes](Commandes.md)
