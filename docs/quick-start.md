# Quick Start Guide

## Initial Setup

### 1. Choose Your Animation Type
Right-click on your skeletal mesh and choose between two options:

   - **Make Bone Animation**  
     Allows for animation sharing and is preferable when memory isn't a constraint.

   - **Make Vertex Animation**  
     Uses larger textures but has lower material cost. However, it doesn't support animation sharing (multiple meshes using the same animation asset).

*Which should you choose?*

Consider these trade-offs:

   - For sharing animations across multiple meshes: Use **Bone Animation**  
   - For optimizing material costs: Use **Vertex Animation**

### 2. Select Animations
After choosing your animation type, you'll see a window displaying all compatible animations for your mesh. Select the animations you want to include in your [VA Asset Collection](va-asset-collection.md).

   ![Animation Selection](assets/quick_1.png)

   - Use "Select All" or "Deselect All" to quickly manage your selection  
   - Individual animations can be toggled using the checkboxes  
   - Click "Create Asset" when you're satisfied with your selection

### 3. Save Your Asset
Choose a location in your content browser to save the new [VA Asset Collection](va-asset-collection.md).

### 4. Material Adjustment
Since this is a Vertex Animation system, your materials will need to be modified. A window will appear showing any material errors that need to be resolved.

   ![Material Errors](assets/quick_2.png)

### 5. Resolve Material Issues
When resolving material errors, you'll have two options:

   ![Material Resolution Options](assets/quick_3.png)

   - **Create Copy**  
     Creates duplicates of your materials before making the necessary changes (recommended to preserve originals)
   
   - **Modify Original**  
     Directly modifies your existing materials

### 6. Final Result
After completing these steps, you'll have a new [VA Asset Collection](va-asset-collection.md) in your content browser.

   ![VA Asset Collection](assets/quick_4.png)

### 7. Using Your VA Asset Collection

After creating your [VA Asset Collection](va-asset-collection.md), you have three options for using it in your project:

- **In the Crowd Tools Editor Mode**  
  Use this mode for easy placement of crowd characters with an intuitive editor interface.

- **In a Vertex Anim Mesh Component**  
  Perfect for adding vertex animation to a single actor in your scene.

- **In a Vertex Anim Instanced Mesh Component**  
  Ideal for efficiently rendering multiple instances of the same vertex-animated mesh.

## Next Steps

Choose your implementation path:

- [Learn about Crowd Tools Editor Mode](crowd-tools-editor-mode.md)
- [Use the Vertex Anim Mesh Component](vertex-anim-mesh-component.md)
- [Implement Instanced Mesh Components](vertex-anim-instanced-mesh-component.md)
