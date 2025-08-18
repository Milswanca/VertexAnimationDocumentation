# UVAMeshComponent

A component that allows playback of a single instance of a VA Asset Collection. Perfect for hero characters or any situation where you need precise control over a single animated mesh, rather than managing multiple instances with the VA Instanced Mesh Component.

![Component Details](assets/details_vamesh.jpg){width=600px style="margin-top: 10px; margin-bottom: 5px;"}

## Vertex Animation

### Asset Reference
- **VA Asset Collection**: Select your VA Asset Collection containing the mesh and animation data
- **Vertex Animation Mesh Index**: Select which mesh to use from the asset collection (if it contains multiple meshes)

### Lists
Animation Lists define the behavior of animations through Animation Logic classes. Each list can contain:

- **Animation Logic Class**: Select the type of logic (e.g., UVAAnimationList_Sequence)
- **Logic Settings**: Exposes the public fields of the selected Animation Logic class. For example:
    - Random Start Position
    - Random Start Animation
    - Pause on Finish
- **Animation List**: Add animations from the asset collection to create a list of animations that will be used by the animation logic.

## Animation Playback Functions

See [VA Animation Player](va-animation-player.md) for animation playback functions.

## See Also

- [Workflow Overview](workflow-overview.md) - Understand how components fit into the overall process
- [VA Instanced Mesh Component](vertex-anim-instanced-mesh-component.md) - For managing multiple instances
- [VA Animation Player](va-animation-player.md) - Control animations in your component
- [VA Animation Lists](vertex-anim-lists.md) - Organize and manage animation sequences
- [VA Animation Logic](animation-logic.md) - Define custom animation behaviors
- [VA Asset Collection](va-asset-collection.md) - The asset type used by this component
