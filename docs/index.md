# Vertex Animation Toolset for UE5

Convert skeletal mesh characters into high-performance vertex animations for rendering crowds and multiple animated characters. The toolset preserves animation quality while reducing CPU overhead and enabling efficient GPU-based rendering through mesh instancing.

> **Important**: This plugin requires Unreal Engine 5.4 or above.

![Crowd Cheering](assets/Crowd_09.jpg){: style="display: block; margin: 0 auto; width: 85%; padding: 10px;"}

## Core Features

### Main Components
1. [**Vertex Anim Mesh Component**:](vertex-anim-mesh-component.md) For single-character implementations requiring individual control
2. [**Vertex Anim Instanced Mesh Component**:](vertex-anim-instanced-mesh-component.md) For efficient rendering of multiple characters
3. [**Animation System**:](animation-control.md) Manages animation playback through Single and AnimList modes
4. [**VA Asset Collection**:](va-asset-collection.md) Manages and stores all data required for vertex animations.  It serves as a container holding meshes, animations, and associated data
5. [**Crowd Tools Editor Mode**:](crowd-tools-editor-mode.md) For visual management and configuration of character groups

### Vertex Animations
- **Animation Types**:
    - **Bone Animations**: Enables sharing between meshes, ideal for memory-flexible projects
    - **Vertex Animations**: Reduces material costs, requires more texture memory, unique per mesh
- **Blueprint Integration**: Program animation behavior using Blueprint-based control systems
- **Sequencer Integration**: Use vertex animations in cinematic sequences and cutscenes

### Workflow Integration
- Convert skeletal meshes with right-click menu
- Automatic material fixes during conversion
- Editor tools for placing and managing crowds
- Timeline control through Sequencer

## Use Cases

![Crowd Cheering](assets/Crowd_08.jpg){: style="display: block; margin: 0 auto; width: 85%; padding: 10px;"}

The plugin is most effective for:

- Dense urban environments with background NPCs
- Large-scale battle sequences
- Games requiring numerous background characters
- Performance-critical scenes with multiple animations

## Technical Overview

### Performance
- Eliminates per-frame skeletal computation overhead
- Uses GPU-efficient instanced rendering
- Optimizes memory usage through shared resources
- Scales effectively with large numbers of characters

### Development
- Compatible with UE 5.4 and above
- Flexible animation management
- Integrated editor toolset

![Crowd Cheering](assets/Crowd_06.jpg){: style="display: block; margin: 0 auto; width: 85%; padding: 10px;"}

## To Get Started

- Follow the [Getting Started](getting-started.md) guide to begin implementing the Vertex Animation Toolset in your project
- Explore the [Troubleshooting](troubleshooting.md) page if you encounter any issues
