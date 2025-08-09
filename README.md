Creative Eyes Hero Component
An interactive and visually stunning hero section for React, featuring a pair of large, stylized 3D eyes that dynamically follow the user's cursor. Built with Three.js and designed to be easily integrated into modern web projects.

(Note: Replace with an actual GIF or screenshot of your component)

Features
Interactive 3D Background: A beautifully rendered Three.js scene that runs smoothly behind your UI.

Cursor Tracking: The eyes dynamically look towards the user's mouse position, creating an engaging and playful interaction.

Procedural Iris Shader: The iris of each eye is procedurally generated with a custom GLSL shader, featuring vibrant, animated radial lines.

Dynamic Pupil Dilation: Pupils subtly dilate and constrict over time, adding a lifelike quality.

"Jiggle" Physics: A simple spring-like physics effect causes the eyes to jiggle in response to fast mouse movements.

Atmospheric Particles: A system of glowing, drifting particles adds depth and a sense of atmosphere to the scene.

Post-Processing Effects: Includes a bloom effect for a soft, futuristic glow.

Easy Integration: Designed as a self-contained React component that can be dropped into any project.

Usage
To use this component, simply import it into your main page or layout file and place it in your JSX. The component is designed to run in the background, so you can overlay your own UI elements on top of it.

// In your main App.js or page.tsx
import { CreativeEyes } from '@/components/ui/CreativeEyes'; // Adjust the import path

export default function HomePage() {
  return (
    <div>
      {/* Your UI Overlay (header, text, buttons, etc.) */}
      <div className="overlay">
        <header>
          {/* ... */}
        </header>
        <div className="main-content">
          {/* ... */}
        </div>
      </div>

      {/* The 3D background component */}
      <CreativeEyes />
    </div>
  );
}

Customization
Currently, the component is self-contained and does not accept props for customization. To change parameters like eye color, particle count, or bloom intensity, you can modify the values directly within the CreativeEyes.tsx file.

Eye Position: Adjust the position.x values for eyeGroup1 and eyeGroup2 in the setupCreativeEyes function.

Particle Count: Change the particleCount variable in the setupParticles function.

Bloom Effect: Modify the strength, radius, and threshold values for the UnrealBloomPass in the setupPostProcessing function.

Dependencies
This component relies on the following libraries:

React (^18.0.0)

Three.js (^0.164.1)

Ensure these are included in your project's package.json.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Copyright (c) 2025 Dhileep Kumar GM            


DEMO : https://21st.dev/dhileepkumargm/creative-eyes-hero-section/default
