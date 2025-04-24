# VA Asset Editor - Mesh Settings

This page details the mesh-related settings in the VA Asset Editor, covering both build configuration and runtime data.

## Mesh Build Settings
![Mesh Build Settings](assets/vacollect_mesh_build.jpg){width=600px style="margin-top: 10px; margin-bottom: 5px;"}

The Mesh Build Settings control how your mesh assets are processed, featuring:

- Source mesh selection and configuration
- LOD and Nanite compatibility options
- Material build settings with bone influence controls
- Animation and frame blending options
- The source materials list

> **Note:** Remember to click the Rebuild Asset button after making changes.

## Mesh Runtime Data
![Mesh Runtime Data](assets/vacollect_mesh_runtime.jpg){width=600px style="margin-top: 10px; margin-bottom: 5px;"}

This panel displays runtime mesh properties and allows configuration of:

- Mesh statistics (vertex count, bones, UV channels)
- Material assignments and references
- Custom float parameter ranges for runtime modification

## Preview Mesh Selection

For Bone VA Asset Collections that contain multiple meshes, the dropdown menu in the VA Asset Editor allows you to switch between different meshes in the preview window. This is particularly useful when working with collections that include variations of the same character or object.

## See Also

- [VA Asset Editor](va-asset-editor.md) - Main editor overview
- [VA Editor - Animation Settings](va-asset-editor-animation.md) - Configure animation-related settings
- [VA Editor - Custom Data](va-asset-editor-custom-data.md) - Configure per-instance custom data
- [VA Mesh Component](vertex-anim-mesh-component.md) - Use VA Asset Collections with single characters
- [VA Instanced Mesh Component](vertex-anim-instanced-mesh-component.md) - Use VA Asset Collections with multiple characters
