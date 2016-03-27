# Lighting/Camera Fixtures 
## for DIY Pick and Place Machine Vision

Electronics built with Altium 15, Mechanics Solidworks 2015.
STL Provided - will upload Gerbers/BOM once the boards are finalised. The boards are built using my open source Altium library.

# Bottom Vision
The bottom vision camera is designed to use a cheap 32mm USB board camera (lots on eBay) Many 34/36/38mm board cameras are actually 32mm  board cameras with extra frame that you can break off.


## Support Structure
![AssemblyImage](https://github.com/issus/Pick-And-Place-Lights/raw/master/Bottom%20Light%20Array/Mounting/AssemblyPreview.jpg)
The camera sits in a 3d printed support structure, with 8 wedges around to make an octogon of light panels.


## Light Panels
![WedgeImage](https://github.com/issus/Pick-And-Place-Lights/raw/master/Bottom%20Light%20Array/BoardPreview.jpg)
The light panels each have their own enable line (default on) and current limiter IC. They are designed to run on 24v, however there is a pin compatible LED (same series) that has 6.1VF rather than 3VF so you could use this as a 24v or 48v light.

Each panel has 16x 32 lumen LEDS which are current limited by an integrated circuit rather than resistors for even light between the panels and less heat.

The 8 panels solder together with the top tabs carrying 24v and the bottom tabs being ground. The middle of the board has a 3 pin connector that has gnd, 24v, and "off". The off connection can be used to disable an individual panel's light output, or for high speed PWM (so the camera isn't affected). Just one panel needs 24v, however each panel is individually controllable for brightness.

Each panel is perpendicular to a point 55mm above the top of the camera board. This is so the bottom vision can be mounted under a table with a 1" wood top that is sitting on 2" high extrusion and not bottom out below, whilst having the light at an optimal angle to reduce reflections back to the camera and limit lighting of the area above the part in view for easier machine vision.
