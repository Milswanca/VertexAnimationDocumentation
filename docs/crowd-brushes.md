# Crowd Brushes

Tools for controlling how crowd elements are placed and configured in your scene. Brushes define instance properties, animation settings, and placement rules for creating diverse and natural-looking crowds.

![Brush Overview](assets/crowd_brush_overview.jpg){width="70%" style="margin-top: 10px; margin-bottom: 5px;"}

## Overview

### 1. Paint Settings
- **Mesh Index selection:** If using Bone Animation types you can select which sub mesh to use here
- **Shadow casting options:** Toggle shadow casting on the instances when they are placed in the level

### 2. Per Instance Animation Data
- **Animation List Logic:** Select and edit your Animation Logic settings. For more information see [Animation Logic](animation-logic.md)

### 3. Painting Settings
- **Density (per 1Kuu):** Controls the number of instances placed within a 10m² area
- **Min Distance Between Instances:** Sets the minimum spacing required between newly placed instances within the paint brush area
- **Scaling Mode:** Select from various scaling constraints Uniform, Free and Lock XY/XZ/YZ
- **Scale (X, Y, Z):** Define minimum and maximum scale values for each axis - instances will be randomly scaled within these bounds


## Creating Brushes

### Direct Addition
- Click "+ Mesh/Brush Asset" in Crowd Editor
- Select your vertex animation mesh asset

### Drag and Drop
- Drag assets to "Drop Your Assets Here" area
- Configure settings in the brush panel

![Add Brush](assets/crowd_add_brush.jpg){width="70%" style="margin-top: 10px; margin-bottom: 5px;"}

## Distribution

### Basic Controls
- Instance spacing
- Random scatter
- Rotation variation
- Scale randomization

### Advanced Options
- Pattern generation
- Group behaviors
- Custom distribution rules
- Performance optimization

## Read More

- [Crowd Tools Editor Mode](crowd-tools-editor-mode.md) - Main editor interface
- [VA Asset Collection](va-asset-collection.md) - Animation asset management
- [Animation Logic](animation-logic.md) - Custom animation behaviors
