# Vertex Anim Mesh Component

The Vertex Anim Mesh Component (VAMeshComponent) is a specialized component that enables vertex animation playback in your Blueprints. It can be added to any Actor to play vertex animations created with the Vertex Animation Toolset.

## Adding to Your Actor

1. In your Actor Blueprint, click "Add Component"
2. Search for "VA Mesh Component"
3. Add it to your Actor

## Basic Setup

1. Select the VA Mesh Component in your Components panel
2. In the Details panel:
   - Set the "Vertex Animation Asset" to your VAT asset
   - Set the "Vertex Animation Mesh Index" if your asset has multiple meshes

## Blueprint Functions

### Asset Management
- **Set Vertex Animation Asset**: Change the VAT asset being used
- **Get Vertex Animation Asset**: Get the current VAT asset
- **Set Vertex Animation Mesh Index**: Switch to a different mesh in the asset
- **Get Vertex Animation Mesh Index**: Get current mesh index

### Animation Control
Through the Animation Player (Get Anim Player node):
- **Play Animation**: Start playing a specific animation
- **Stop**: Stop the current animation
- **Pause**: Pause the current animation
- **Resume**: Resume a paused animation
- **Set Play Rate**: Change animation speed
- **Play Animation By Name**: Play an animation using its name
- **Set Loop Animation**: Enable/disable animation looping

### Animation State
- **Is Playing**: Check if an animation is currently playing
- **Is Paused**: Check if the animation is paused
- **Get Current Animation**: Get the index of the playing animation
- **Get Animation Progress**: Get current animation progress (0-1)
- **Get Current Time**: Get current animation time in seconds

### Material & Custom Data
- **Reapply Custom Data**: Update custom vertex data
- **Refresh Material Values**: Force update of material parameters

## Example Blueprints

### Basic Animation Playback
```
Event BeginPlay
└─► Get Anim Player
    └─► Play Animation
        - Animation Index: 0
        - Loop: True
```

### Animation with Blending
```
Event Action Input
└─► Get Anim Player
    └─► Play Animation
        - Animation Index: 1
        - Blend Duration: 0.5
        - Loop: False
```

## Tips & Best Practices

### Asset Setup
- Assign your VAT asset in the component details
- Verify the correct mesh index is selected

### Animation Control
- Use the Animation Player for all playback control
- Store animation indices as variables for easy reference
- Use animation names when possible for better readability

### Performance
- Avoid updating material parameters manually
- Use the built-in blending system instead of manual blending
- Consider using animation lists for organized animation management

## Common Issues

### No Mesh Visible
- Check if VAT asset is assigned
- Verify mesh index is valid
- Ensure materials are properly set up

### Animation Not Playing
- Confirm animation index is valid
- Check if Animation Player is properly initialized
- Verify animation is not paused

### Material Issues
- Make sure materials are compatible with VAT
- Check if dynamic materials are generating correctly
- Use Reapply Asset Materials if materials are missing

## Events

The component provides several events you can bind to:
- **On Vertex Animation Asset Changed**: Called when the asset is changed
- **On Animation Finished**: Triggered when an animation completes
- **On Animation Started**: Fired when an animation begins playing

Use these events to coordinate animation logic with other game systems.

> **Note**: This component is designed to be easily used in Blueprints while providing powerful vertex animation capabilities. Most common use cases can be handled entirely through Blueprint functions without needing to write C++ code.
