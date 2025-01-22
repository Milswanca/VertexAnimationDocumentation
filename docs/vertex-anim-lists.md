# UVAAnimationLists

VA Lists organize and manage animation behaviors for vertex-animated meshes.

## Overview
- Container for Animation Logic instances
- Manages animation state transitions
- Controls playback for multiple instances

## Setup

1. In VA Component details panel, find "Animation Lists"
2. Click "+" to add new Animation List
3. Select Animation Logic class
4. Configure default values

![VA Lists Setup](assets/placeholder-valists-setup.png)

## Core Features

### List Management
```cpp
// Create new animation list
CreateAnimationList(LogicTemplate)

// Remove animation list
RemoveAnimationList(Index)

// Access lists
GetAnimationList(Index)
```

### Component Integration
```cpp
// Set owning component
SetOwningComponent(Component)

// Get owning component 
GetOwningComponent()
```

## Best Practices

1. **Organization**
   - Group related animations
   - Use clear naming conventions
   - Keep lists focused and modular

2. **Performance**
   - Minimize list count
   - Clean up unused lists
   - Use appropriate update frequencies

For implementation details, see [Animation Logic](animation-logic.md).
