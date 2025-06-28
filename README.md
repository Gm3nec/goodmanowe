# Shooting Over Hill

This repository contains a minimal Unity setup for a simple shooter where the player fires bullets at a hill. The scripts demonstrate continuous collision detection so fast-moving bullets don't pass through the terrain.

## Project Structure

```
Assets/
  Scripts/
    Bullet.cs
    PlayerShooter.cs
  Scenes/
```

## Getting Started

1. Create a new 3D Unity project and copy these folders into the project directory.
2. Add a Terrain object to your scene, tag it `Hill`, and ensure it has a `Terrain Collider`.
3. Create a player object with the `PlayerShooter` component.
   - Assign a child transform as the `shootPoint`.
   - Provide a bullet prefab with a `Rigidbody`, collider, and the `Bullet` script.
4. Press Play and use the left mouse button (Input `Fire1`) to shoot.

The bullet uses `CollisionDetectionMode.ContinuousDynamic` to handle collisions even when moving quickly.
