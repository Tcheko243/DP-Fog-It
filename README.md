# Fog It - Blender Addon

## Overview
Fog It is a powerful Blender addon that allows you to add realistic volumetric fog to your scenes. It supports both Eevee and Cycles render engines, offering different fog solutions optimized for each renderer.

## Features
- Real-time fog updates
- Support for both Eevee (2D) and Cycles (3D) render engines
- Customizable fog properties:
  - Density control
  - Color settings
  - Volume size and position
  - Noise patterns with animation
  - Height-based gradient
  - Color ramp controls
- Cycles-specific features:
  - Anisotropic scattering
  - Temperature control
  - True volumetric rendering

## Installation
1. Download the latest release
2. In Blender, go to Edit > Preferences > Add-ons
3. Click "Install" and select the downloaded ZIP file
4. Enable the addon by checking the checkbox next to "3D View: Fog It"

## Usage
1. Open the sidebar in the 3D Viewport (Press N)
2. Look for the "Fog It" tab
3. Click "Add Fog" to create a fog volume
4. Adjust parameters in the panel to customize your fog

### Main Controls
- **Volume Size**: Control the dimensions of the fog volume
- **Start Height**: Set the base height of the fog
- **Density**: Adjust the opacity of the fog
- **Color**: Set the fog color

### Noise Settings
- **Use Noise**: Enable procedural noise patterns
- **Noise Scale**: Adjust the size of noise features
- **Noise Detail**: Control the complexity of the noise
- **Noise Roughness**: Adjust the irregularity of the noise
- **Animate Noise**: Enable noise animation
- **Animation Speed**: Control the speed of noise animation

### Gradient Settings
- **Use Height Gradient**: Enable height-based density falloff
- **Gradient Height**: Control the height of the gradient effect

### Color Ramp
- **Position 1 & 2**: Control the gradient positions
- **Colors 1 & 2**: Set the colors for the gradient

### Cycles-Specific Settings
- **Anisotropy**: Control the directional scattering of light
- **Temperature**: Adjust the volume temperature

## Render Engine Specifics

### Eevee
- Uses a 2D plane with transparent shader
- Optimized for real-time viewport performance
- Best for quick previews and game-engine style fog

### Cycles
- Uses true 3D volumetrics
- Physically accurate light scattering
- Better for final renders and realistic fog effects

## Requirements
- Blender 2.80 or newer
- Minimum system requirements:
  - 8GB RAM recommended
  - GPU with OpenGL 3.3+ support
  - CPU with SSE2 support

## Known Issues
- Heavy noise settings may impact viewport performance
- Large volume sizes with high density may increase render times in Cycles
- Real-time updates might be slower on lower-end systems
- if nothing work when you add fog, just change on parameter to refresh

## Tips & Tricks
1. Start with lower density values and adjust gradually
2. Use noise sparingly for better performance
3. For outdoor scenes, enable height gradient
4. Adjust color ramp positions for more natural-looking fog
5. In Cycles, use lower density values than in Eevee

## Contributing
Feel free to submit issues and enhancement requests through GitHub.

## License
This project is licensed under the GNU License - see the LICENSE file for details.

## Credits
Created by Dimona Patrick

## Version History
-1.2.1:Current release
  -Material creation for Fog_volume work now
  -2D Fog for evee and 3D Fog for cycles work well now
- 1.2: Current release
  - Added real-time updates
  - Improved noise controls
  - Added height gradient feature
- 1.1: Initial public release

## Support
For support, please create an issue in the GitHub repository or contact the developer directly.

## FAQ
Q: Why does the fog look different in Eevee and Cycles?
A: Each render engine handles volumetrics differently. Eevee uses a simplified 2D approach for performance, while Cycles calculates true 3D volume scattering.

Q: How can I improve performance?
A: Reduce noise detail, use larger noise scale values, and keep the volume size reasonable for your scene.

Q: Can I animate the fog properties?
A: Yes, all properties can be keyframed, and the noise pattern can be animated using the built-in animation controls.

