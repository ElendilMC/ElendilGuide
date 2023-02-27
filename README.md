# Elendil Guide
Regroupement de technologies intéressantes (Performance).

## Server Software
- Bukkit: Le serveur minecraft de base avec support plugin. Recommandé pour les survies de <= 5 joueurs maxiumum.
- [Spigot](https://getbukkit.org/download/spigot): Spigot est un fork performance de bukkit, permettant de supporter plus de plugins.
- [Paper](https://papermc.io/downloads): Paper est un fork de spigot orienté performance, patchant des bugs de spigot et du vanilla (duplication). Pas recommandé pour la survie vanilla.
- [Purpur](https://purpurmc.org/): Purpur est un fork optimisation et customisation de Paper, implémentant [Pufferfish](https://pufferfish.host/downloads). Il est recommandé pour la survie vanilla: un comportement 100% vanilla est possible avec la bonne configuration.
- [Kaiiju](https://github.com/KaiijuMC/Kaiiju/releases): Kaiiju est un fork de Purpur, créé spécialement pour les serveurs survie vanilla/anarchie massifs. Il incorpore les optimisations de Lithium, C2ME et VMP.
- [Forge](https://files.minecraftforge.net/net/minecraftforge/forge/): Forge est un modloader. Il est recommandé d'utiliser fabric, plus performant.
- [Fabric](https://fabricmc.net/use/server/): Fabric est un modloader. Plus lent que Purpur/Kaiiju même avec mods, mais plus facile à configurer. Il est recommandé pour des serveurs communautaires.

Par ordre croissant de performance:

Bukkit < Forge < Spigot < Fabric < Paper < Purpur < Kaiiju

## Mods
### Fabric
- [Lithium](https://modrinth.com/mod/lithium/versions): Améliore la performance de Minecraft tout en restant vanilla.
- [Phosphor](https://www.curseforge.com/minecraft/mc-mods/phosphor): Améliore les performances du moteur de lumière de Minecraft. Il est recommandé d'utiliser [Starlight](https://modrinth.com/mod/starlight/versions) a la place.
- [Starlight](https://modrinth.com/mod/starlight/versions): Améliore les performances du moteur de lumière de Minecraft. Beaucoup plus rapide que Phosphor.
- [Memory Leak Fix](https://modrinth.com/mod/memoryleakfix/versions): Supprime les leak de mémoire dans Minecraft.
- [C2ME](https://github.com/RelativityMC/C2ME-fabric): Améliore la génération de Minecraft. Expérimental.
- [VMP](https://modrinth.com/mod/vmp-fabric): Améliore la performance de Minecraft tout en restant vanilla. Expérimental.
- [Spark](https://spark.lucko.me/): Permet de diagnostiquer les lags de son serveur, de surveiller la performance et d'avoir des statistiques.

## Plugins
- [View Distance Tweaks](https://github.com/froobynooby/ViewDistanceTweaks): Changer la simulation et la view distance en fonction des performances du serveur. Il est recommandé d'utiliser la version de ce plugin maintenue par Kaiiju, étant plus à jour. [Lien](https://github.com/KaiijuMC/ViewDistanceTweaks)
- [AFK View Distance](https://github.com/KaiijuMC/AFKViewDistance): Limiter la view distance et la simulation distance des joueurs AFK.
- [Spark](https://spark.lucko.me/): Permet de diagnostiquer les lags de son serveur, de surveiller la performance et d'avoir des statistiques.

## Autre
- [GraalVM](https://www.graalvm.org/downloads/): Une JavaVM beaucoup plus rapide. Il est recommandé d'utiliser la version EE.
- [GC Flags](#): Guide des flags du Garbage Collector. Optimisation de la RAM, permet de réduire les lag spikes. Création en cours.
