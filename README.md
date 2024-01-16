# Unity Project - **Early Access** (bugs may be present)

Ce projet à été réalisé pour la matière "Programmation multimédia"

Membres du projet:
- Thomas RUBINI
- Mélanie HUGUES

Je (Thomas) me suis occupé de la plupart des scripts de gameplay et des modèles importés depuis le Unity Asset Store, et Mélanie s'est occupée de la map et des animations

Dans ce jeu, on retrouve des élements tels que des pièces, un téléporteur, et un coffre qui peut s'ouvrir à l'aide d'une clé présente dans la map. (voir Chest.cs)

Ces objets sont maintenus dans la main du joueur. Pour cela, nous avons modifié son rig en ajoutant un GameObject dont le seul but est d'être le parent des objets tenus par le joueur. (Voir Player.cs#setHeldObject())

Pour gérer la mort du joueur, nous avons créé un GameObject à un endroit spécifique du monde, qui agit comme variable stockant les coordonnées de respawn (spawnpoint, voir Player.cs#TpToSpawnpoint())

Les événements globaux du jeu, tels que le début/fin de la partie, la gestion du chronomètre et des coins, sont dans GameManager.cs, qui agit comme gestionnaire global du jeu.

Certains modèles/textures ont été créés par nous à l'aide de blender et ont été importés via le format fbx, tandis que d'autres ont été trouvés sur le Unity Asset Store

Dans la création des scripts, nous avons essayé de respecter la notion de composant, et de généraliser les composants utilisés: Par exemple, un comportement "Pickupable" à été créé au lieu d'un comportement "Clé", ce qui laisse la possibilité de rendre d'autres objets récupables par le joueur dans le futur


Ressources du Unity Asset Store utilisées:
- https://assetstore.unity.com/packages/p/animated-pbr-chest-demo-194755
- https://assetstore.unity.com/packages/p/handpainted-keys-42044
- https://assetstore.unity.com/packages/3d/props/weapons/watermelon-sword-191078
- TextMesh Pro
- https://assetstore.unity.com/packages/vfx/shaders/aquas-lite-built-in-render-pipeline-53519
- https://assetstore.unity.com/packages/3d/characters/animals/dog-knight-pbr-polyart-135227

Les autres textures externes utilisées ont été choisie pour leur licence libre (e.g. CC0)
- https://www.freepik.com/free-photos-vectors/leaves-texture
- https://www.freepik.com/free-photos-vectors/grass-texture
- https://www.freepik.com/free-photos-vectors/wood-texture
