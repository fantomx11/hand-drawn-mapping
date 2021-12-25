# Pseudo Hand Drawn Maps for Table Top RPGs

I really like the aesthetics of hand drawn maps, but do not have the artistic ability required to make high quality ones. Likewise for isometric maps, but have even less artistic ability in that department. So I have tried to develop a method to create isometric maps (technically they are dimetric, but that is simply a function of what angle the camera is pointing when rendering).

## Process

The basic process is:

1. Create the map in Blender.
2. Add whatever details I want as edges on the map.
3. Mark those edges as Freestyle edges
4. Enable the Freestyle SVG Export plugin that comes bundled with Blender
5. Render the scene
6. Open the resulting SVG file in Inkscape
  - The SVG file that Blender puts out is formatted weirdly for Inkscape. I find it is best to ungroup everything that Blender has output, create a new Layer, and move all of the ungrouped items to the new Layer. Don't create the new layer until after ungrouping all the items.
7. Create a new layer named "Line art"
8. Make sure that snapping to cusp nodes is enabled
9. Decide which lines that blender created would be done in a single stroke, were I drawing or tracing the image, and create new paths based on those strokes.
10. Group all these lines together and add a Sketch Live Path Effect. Adjust the settings until it looks right. I typically set  Max. end tolerance to 0, set average offset to 0 - 1, set max tremble to 1 - 5, and adjust the tremble frequency until it looks good to me.
11. Add a new layer called "Hatching"
12. Create new shapes for anything that should be in shadow or shaded in some way
13. Add a Hatching Live Path Effect to these new shapes. If some of the shapes should have the hatching running the same direction, group them together and add the hatch effect to the group. I usually uncheck bend hatches and generate thick/thin path. Adjust the green handle until the hatching looks good to you.

## What is Here

I have included a Blender file, and a SVG file from after the steps listed above as an example.
