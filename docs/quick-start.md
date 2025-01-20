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
After choosing your animation type, you'll see a window displaying all compatible animations for your mesh. Select the animations you want to include in your Vertex Animation Asset.

   ![Animation Selection](assets/quick_1.png)

   - Use "Select All" or "Deselect All" to quickly manage your selection  
   - Individual animations can be toggled using the checkboxes  
   - Click "Create Asset" when you're satisfied with your selection

### 3. Save Your Asset
Choose a location in your content browser to save the new Vertex Animation Asset.

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
After completing these steps, you'll have a new Vertex Animation Asset in your content browser.

   ![Vertex Animation Asset](assets/quick_4.png)
