# Laser Defender – 2D Space Shooter (Unity)

A top-down 2D space shooter: fly your ship, dodge enemy fire and destroy successive waves of enemies.

## Features

- **Data-driven enemy waves** defined as ScriptableObjects (`WaveConfigSO`): enemy prefabs, path waypoints, speed and randomised spawn timing, with optional looping.
- **Waypoint pathfinding** for enemy movement.
- **Shooting system** shared by player and AI enemies, with randomised firing rate.
- **Health and damage** components, with the player kept inside screen bounds.
- Player controls with Unity's **new Input System**.
- Sprites and sounds from Kenney's Space Shooter asset pack.

## Tech stack

Unity 2022.3 LTS (2D) · C#

## Scripts

| Script | Role |
|---|---|
| `Player.cs` | movement with input and screen padding |
| `Shooter.cs` | projectile firing for player and enemies |
| `Health.cs`, `DamageDealer.cs` | hit points and damage on collision |
| `EnemySpawner.cs` | spawns waves in sequence, optional looping |
| `WaveConfigSO.cs` | ScriptableObject describing one wave |
| `PathFinder.cs` | moves enemies along their waypoints |

## Run it

Open the folder with Unity Hub (Unity 2022.3.53f1 or a later 2022.3 LTS), open `Assets/Scenes/SampleScene.unity` and press Play.

## Credits

Built while following the GameDev.tv Unity 2D course. Art and sounds: [Kenney](https://kenney.nl) (CC0).

## Author

Ridha Lezzar · [LinkedIn](https://linkedin.com/in/ridha-lezzar-8322222b5)
