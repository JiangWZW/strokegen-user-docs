# User Guide

## Prepare your mesh

StrokeGen requires a polygonal mesh to work with. 

For the best results, ensure that:

- The mesh is triangulated. For example, if you applied a subdivision surface modifier, a triangulation modifier has to be attached before feeding the mesh into StrokeGen. 
- The mesh has a decent topology; if you ever did subdivision modeling, you know what I mean - proper flows of quad loops, uniform vertex valency, adaptive density of quads, etc. Otherwise, like any other rendering algorithms, trash-in, trash-out. 
- Avoid thin shells. For example, when modeling your model, you might thicken the mesh, leading to a shell consisting of two layers of very close surfaces. This causes StrokeGen to render lines for both layers, resulting in unpleasant results. 

## StrokeGen Features

### Global Settings

### Per-Object Settings