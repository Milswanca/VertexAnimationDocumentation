# UVAAnimationPlayer

The VA Animation Player is the core animation system that powers all vertex animation playback in the Vertex Animation Toolset. You can access it through any VA Mesh Component using the "Get Anim Player" node in Blueprints.

## Getting Started

To access the Animation Player in Blueprints:

1. Get a reference to your [UVAMeshComponent](vertex-anim-mesh-component.md) or [UVAInstancedMeshComponent](vertex-anim-instanced-mesh-component.md)
2. Call the "Get Anim Player" function
3. Use the returned Animation Player reference for playback control

## Blueprint Functions

### Basic Animation Control

![Animation Control Nodes](assets/animation-control.png)

**Play Animation**
```
Play Animation
├─ Animation Index: Integer (which animation to play)
├─ Start Position: Float (0-1, where in animation to start)
├─ Blend Duration: Float (seconds to blend from current to new animation)
└─ Loop: Boolean (whether to loop the animation)
```

**Play Animation List**
```
Play Animation List
└─ Animation List Index: Integer (which list to play)
```

**Simple Controls**

  - Stop Animation
  - Pause Animation
  - Resume Animation

### Playback Settings

- **Set Play Rate**: Change animation speed (1.0 is normal speed)
- **Set Position**: Jump to specific point in animation (0-1)
- **Set Playing**: Start/stop playback
- **Set Reverse**: Play animation backwards
- **Step Forward/Backward**: Move one frame at a time

### State Information

Get current animation state:

- Get Current Animation
- Get Animation List
- Get Play Rate
- Get Position (0-1)
- Get Playing
- Get Reversed
- Get Scaled/Unscaled Duration
- Get Remaining Time
- Get Start Position
- Get Timestamp

## Animation Lists

Animation Lists help you organize and control sequences of animations.

## Blueprint Examples

### Basic Character Animation
```
// Set up basic idle animation
Event BeginPlay
└─► Get Anim Player
    └─► Play Animation
        ├─ Animation Index: 0 (Idle)
        ├─ Start Position: 0.0
        ├─ Blend Duration: 0.2
        └─ Loop: True

// Switch to running when movement starts
Event Move
└─► Get Anim Player
    └─► Play Animation
        ├─ Animation Index: 1 (Run)
        ├─ Blend Duration: 0.5
        └─ Loop: True
```

### Using Animation Lists
```
// Random idle animations
Event BeginPlay
└─► Get Anim Player
    └─► Play Animation List
        └─ List Index: 0 (Idle List)

// Sequential walk cycle
Event Move
└─► Get Anim Player
    └─► Play Animation List
        └─ List Index: 1 (Walk Sequence)
```

### Environmental Animation
```
// Windmill example with variable speed
Event BeginPlay
└─► Get Anim Player
    ├─► Play Animation
    │   ├─ Animation: WindmillSpin
    │   └─ Loop: true
    └─► Set Play Rate
        └─ Rate: WindSpeedVariable
```

## Events

The Animation Player provides several events you can bind to in Blueprints:

- **On Animation Started**: Called when a new animation begins
- **On Animation Finished**: Called when an animation completes
- **On Animation List Completed**: Called when all animations in a list have played
- **On Instance Registered/Unregistered**: Called when animation instances are added/removed

## Tips & Best Practices

### Performance
- Use Animation Lists for organized playback control
- Leverage the built-in blending system
- Keep blend durations reasonable (0.2-0.5 seconds typically)

### Animation Control
- Store animation indices as Blueprint variables for clarity
- Use animation names when possible
- Set up proper animation sequences for smooth transitions

### Common Patterns
- Use Sequence Lists for locomotion animations
- Use Random Shuffle Lists for idle variations
- Leverage events for animation-driven gameplay logic

## See Also

- [Workflow Overview](workflow-overview.md) - Understand how animation control fits into the overall process
- [VA Animation Lists](vertex-anim-lists.md) - Organize and manage animation sequences
- [VA Animation Logic](animation-logic.md) - Define custom animation behaviors
- [VA Mesh Component](vertex-anim-mesh-component.md) - Control animations for single characters
- [VA Instanced Mesh Component](vertex-anim-instanced-mesh-component.md) - Control animations for multiple characters
