# VA Asset Collection

The VA Asset Collection is the core asset type in the Vertex Animation Toolset that manages and stores all data required for vertex animations. It serves as a container that holds meshes, animations, and their associated data.



## Overview

A VA Asset Collection contains:

- Source skeletal meshes and their build settings
- Built vertex animation meshes
- Animation data stored in textures
- Material configurations
- Per-mesh custom data

## Components

### Mesh Data
- Stores converted static meshes optimized for vertex animation
- Maintains UV channel information
- Contains bone data for skeletal mesh animations
- Tracks vertex counts and bounds
- Stores material configurations and overrides

### Animation Data
- Position and rotation/normal texture data
- Animation frame data
- Animation bounds
- Frame rates and timing information
- Animation sequence metadata

### Material Settings
- Source material references
- Material build configurations
- Material parameter mappings
- Custom material data per mesh

## Editor Features

A custom editor window is available for working with VA Asset Collections. See the [VA Asset Editor](va-asset-editor.md) page for more information.

![VA Asset Collection](assets/vacollect_01.jpg){width="70%" style="margin-top: 10px;"}

## Technical Details

### Storage Format
- Animations are stored as texture-based vertex data
- Positions and rotations/normals are split into separate textures
- Each mesh maintains its own vertex layout and UV configuration
- Build hashes track asset changes and dependencies

### Performance Considerations
- Optimized for runtime texture sampling
- Efficient memory usage through texture-based storage
- Minimal runtime overhead
- Built data is preprocessed for optimal playback

## See Also
- [VA Mesh Component](vertex-anim-mesh-component.md) - Component for playing vertex animations
- [VA Animation Player](va-animation-player.md) - Animation playback system
- [Quick Start Guide](quick-start.md) - How to create and configure assets
