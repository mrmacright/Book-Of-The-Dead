# CHANGELOG

## 2025 - Unity 6 Migration Update

**Version Tag** : `6000.3.0`

* Updated Unity from 2022.2.9 to 6000.3.0f1
* Updated Input System to 1.16.0 (Unity Registry)

### Fixes and Changes
* Updated legacy code to restore compatibility with modern Unity reflection APIs  
  * Modified `Hapki.EnumExtensions.cs` to replace deprecated `Activator.CreateInstance` usage
* Updated TerrainEvo3 editor code to remove unsupported `MeshCollider` properties  
  * Removed usage of `inflateMesh` and `skinWidth`, which are no longer exposed in modern Unity  
  * Convex hull inflation is now handled internally by PhysX
* Enabled VSync (Every V Blank) via HDRP Quality settings to reduce screen tearing
* Project now builds and runs correctly under Unity 6 with HDRP
* Updated minimum macOS target from 12.0 to 15.0 for Unity 6 compatibility
* App icon added

### Known Issues
* No in-game graphics or resolution options (legacy Unity launcher dialog is no longer supported in Unity 6)
* Performance and visual behaviour are fully driven by HDRP assets and project settings
