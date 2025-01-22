# Vertex Animation Toolset for UE5

The Vertex Animation Toolset converts Skeletal Mesh characters into Vertex Animation-based Static Meshes, significantly improving performance when rendering multiple animated characters.

> **Important**: This plugin requires Unreal Engine 5.4 or above.

![Crowd Cheering](assets/Crowd_09.jpg)

## Overview

This plugin addresses performance bottlenecks in scenes with multiple animated characters by converting skeletal animations to vertex animations. The conversion process preserves animation quality while reducing CPU overhead and enabling efficient GPU-based rendering through mesh instancing.

## Core Features

### Animation Types
- **Bone Animation**: Enables animation sharing between multiple meshes. Best for projects where memory isn't a primary constraint.
- **Vertex Animation**: Reduces material costs but requires more texture memory. Animations are unique to each mesh.

### Components
1. **Vertex Anim Mesh Component**: For single-character implementations requiring individual control
2. **Vertex Anim Instanced Mesh Component**: For efficient rendering of multiple characters
3. **Crowd Tools Editor Mode**: For visual management and configuration of character groups

### Animation Logic
- **Blueprint Integration**: Program animation behavior using Blueprint-based control systems
- **Event-Driven**: Trigger animations based on game events and conditions
- **State Management**: Define complex animation states and transitions
- **Runtime Control**: Dynamically adjust animation behavior during gameplay
- **Flexible Rules**: Create custom animation selection logic and priority systems

### Performance
- Eliminates per-frame skeletal computation overhead
- Uses GPU-efficient instanced rendering
- Optimizes memory usage through shared resources
- Scales effectively with large numbers of characters

### Workflow Integration
- Direct conversion from existing skeletal animations
- Automatic material system integration
- Built-in crowd management tools
- Multiple character placement methods

## Use Cases

The plugin is most effective for:

- Dense urban environments with background NPCs
- Large-scale battle sequences
- Games requiring numerous background characters
- Performance-critical scenes with multiple animations

## Technical Overview

### Runtime Performance
- Reduced CPU overhead per frame
- Efficient GPU batch processing
- Optimized memory footprint
- Streamlined rendering pipeline

### Development
- Compatible with UE 5.4 and above
- Flexible animation management
- Integrated editor toolset


Check out the [Quick Start Guide](quick-start.md) to begin implementing the Vertex Animation Toolset in your project.
