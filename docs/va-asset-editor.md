# VA Asset Editor

The VA Asset Editor is a specialized tool for configuring and managing VA Asset Collections. This page provides an overview of the editor interface and its main features.

## Interface Overview

The VA Asset Editor window contains several key elements that help you manage and customize your vertex animation data:

![VA Asset Editor Interface Overview](assets/vacollect_02.jpg){style="margin-top: 10px; margin-bottom: 5px;"}

### 1. Rebuild Asset Button
> This button reconstructs your mesh and materials. Use this after making any adjustments in the details panel to ensure your changes are properly applied.

### 2. Preview Mesh Selection
> For Bone VA Asset Collections that contain multiple meshes, this dropdown menu allows you to switch between different meshes in the preview window. This is particularly useful when working with collections that include variations of the same character or object.

### 3. Reapply Custom Data
> This feature enables you to inject custom float data into your instanced VA mesh. By modifying these values, you can create visual variations between instances, ensuring each character or object appears unique in your scene. For more details, see the [Custom Data Settings](va-asset-editor-custom-data.md) page.

### 4. Details Panel
> The right-side panel contains crucial settings divided into several categories:
>
> - [Mesh Build Settings](va-asset-editor-mesh.md#mesh-build-settings)
> - [Animation Data Settings](va-asset-editor-animation.md#animation-build-settings)
> - [Mesh Runtime Data Settings](va-asset-editor-mesh.md#mesh-runtime-data)
> - Asset Validation
> - [Animation Build Settings](va-asset-editor-animation.md#animation-build-settings)
>
> These settings allow you to fine-tune various aspects of your vertex animation. Detailed information about each category is available on the linked pages.

### 5. Animation Preview
> The timeline area displays your currently selected preview animation. You can switch between different animations to visualize how your asset will appear in-game.

### 6. Animation Timeline
> The bottom panel provides standard timeline controls for previewing your animations. Use these controls to play, pause, and scrub through your animation sequences.

## Detailed Settings Pages

The VA Asset Editor settings are organized into three main categories, each with its own dedicated page:

- [Animation Settings](va-asset-editor-animation.md) - Configure animation build options and view runtime animation data
- [Mesh Settings](va-asset-editor-mesh.md) - Configure mesh build options and view runtime mesh data
- [Custom Data Settings](va-asset-editor-custom-data.md) - Configure per-instance custom data for material variations

## See Also

- [Workflow Overview](workflow-overview.md) - Understand how the Asset Editor fits into the overall process
- [Quick Start Guide](quick-start.md) - How to create and configure VA Asset Collections
- [VA Asset Collection](va-asset-collection.md) - The asset type edited by this editor
- [VA Animation Player](va-animation-player.md) - Control animations in your VA Asset Collection
- [VA Mesh Component](vertex-anim-mesh-component.md) - Use edited assets with single characters
- [VA Instanced Mesh Component](vertex-anim-instanced-mesh-component.md) - Use edited assets with multiple characters
