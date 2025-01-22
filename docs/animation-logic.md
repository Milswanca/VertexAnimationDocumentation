# UVAAnimationListLogic

Blueprint system for controlling vertex animation behavior.

## Setup

1. Content Browser → Right-click → Blueprint Class
2. Parent Class: VAAnimationListLogic
3. Name your Blueprint (e.g., "BP_IdleWalkLogic")

![Creating Logic](assets/placeholder-create-logic.png)

## Blueprint Events

### Begin Instances
```
Event Begin Instances
└── Play Animation
    ├── Instance ID
    ├── Animation Index
    └── Looping = true
```

### End Instances
```
Event End Instances
└── Stop Animation
    └── Instance ID
```

### Update Instances
```
Event Update Instances
└── [Your update logic]
```

### Animation Completed
```
Event Animation Completed
└── [Handle completion]
```

### Custom Events
```
Event On Custom Animation Event
└── [Handle event]
```

## Example: Idle/Walk System

![Idle Walk Logic](assets/placeholder-idle-walk.png)

```
Begin Instances
└── Play Idle

Update Instances
├── Get Speed
└── Branch
    ├── Speed > 0
    │   └── Play Walk
    └── Play Idle
```

## Example: Random Playback

```
Begin Instances
└── Play Random

Animation Completed
├── Random Delay
└── Play Next
```

## Tips

1. **Performance**
   - Keep logic simple
   - Batch operations
   - Cache values

2. **Debug**
   - Print states
   - Use breakpoints
   - Visualize data

For list management, see [VA Lists](vertex-anim-lists.md).
