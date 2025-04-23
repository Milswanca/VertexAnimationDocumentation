# Vertex Anim Instanced Mesh Component

The Vertex Anim Instanced Mesh Component is designed for scenarios where you need to display multiple instances of the same vertex-animated mesh. This component provides efficient rendering and animation control for crowds or repeated elements in your scene.

This component functions exactly like the [VA Mesh Component](vertex-anim-mesh-component.md) but allows you to create multiple instances just like you would with a regular Instanced Static Mesh Component. When not using a Nanite-enabled VA Asset Collection, this component also supports LODding for optimal performance with large numbers of instances.

## Features
- Efficient multi-instance rendering
- Batch animation control
- Memory-efficient instance management
- Performance optimized for large numbers of instances
- LOD support (when not using Nanite-enabled VA Asset Collection)

## Animation Control

For details on animation setup and control, refer to the [VA Mesh Component](vertex-anim-mesh-component.md) documentation, as both components share the same animation functionality.

## See Also
- [Workflow Overview](workflow-overview.md) - Understand how components fit into the overall process
- [Crowd Tools](crowd-tools-editor-mode.md) - Tools for managing crowd instances
- [VA Mesh Component](vertex-anim-mesh-component.md) - For single instance usage
- [VA Animation Player](va-animation-player.md) - Control animations in your component
- [VA Animation Lists](vertex-anim-lists.md) - Organize and manage animation sequences
- [VA Animation Logic](animation-logic.md) - Define custom animation behaviors
- [VA Asset Collection](va-asset-collection.md) - The asset type used by this component
