# VA Asset Editor - Custom Data

This page details the custom data settings in the VA Asset Editor, which allow you to create variations between instances of your vertex animated meshes.

## Per Instance Custom Data

The Per Instance Custom Data system is a powerful feature that enables dynamic material variation across instances. Each custom data entry consists of:

- **Custom Data Name**: A unique identifier used to reference this parameter in your materials
- **Custom Float Range**: Minimum and maximum values for the parameter
- **Round Values to Int**: Option to round the generated values to whole numbers

![Mesh Runtime Data](assets/vacollect_mesh_runtime.jpg){width=600px style="margin-top: 10px; margin-bottom: 5px;"}

The Per Instance Custom Data system allows you to inject randomized or controlled float values into your instanced materials. This creates visual diversity across instances without the need for multiple materials or meshes.

## Usage Examples

You can use custom data for various effects, such as:

- Create color variations by connecting the float value to material color parameters
- Adjust material properties like roughness or metallic values per instance
- Control texture tiling or blending between different textures
- Implement any other material parameter variations you can imagine

## How It Works

When the instance is spawned, each custom float parameter will generate a value within its specified range. These values can then be accessed within your material graphs to create unique variations for each instance.

## Reapply Custom Data

The VA Asset Editor provides a "Reapply Custom Data" button that enables you to inject custom float data into your instanced VA mesh. By modifying these values, you can create visual variations between instances, ensuring each character or object appears unique in your scene.

> **Note:** Remember to click the Rebuild Asset button after making changes to custom data settings.

## See Also

- [VA Asset Editor](va-asset-editor.md) - Main editor overview
- [VA Editor - Animation Settings](va-asset-editor-animation.md) - Configure animation-related settings
- [VA Editor - Mesh Settings](va-asset-editor-mesh.md) - Configure mesh-related settings
- [VA Instanced Mesh Component](vertex-anim-instanced-mesh-component.md) - Use VA Asset Collections with multiple characters
