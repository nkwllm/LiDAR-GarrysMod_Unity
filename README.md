# LiDAR from Garry's Mod in Unity3D
This project tries to replicate the LiDAR extensions from Garry's Mod in the Unity game engine. It uses the VFX-Graph to spawn and manage the dots.

### Development Platform
- Windows 10 x64

### Unity Version
- Unity Version: 2022.1.10f1
- Using the High Definition Render Pipeline

### Target Platform
- Standalone Windows x64
- MacOS Standalone

### What is LiDAR Garry's Mod?
- [Steam page](https://steamcommunity.com/sharedfiles/filedetails/?id=2813176307)
- [The Librarian Youtube Gameplay](https://www.youtube.com/watch?v=ac1LXZUkn8c)


### How?
*Using the HDRP, VFX Graph and Raycasts mostly.*
The Raycasts get the points on the mesh that need a particle to be spawned at. By encoding the position information in a 2D texture, we send it to the GPU (the VFX-Graph). Every particle gets assigned a uv coordinate with represents its position. The uv coordinates position gets set and the particles spawn.

