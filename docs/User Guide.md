# Best Practices

## Prepare your mesh

Like any other rendering algorithm, the performance of StrokeGen depends on the quality of your mesh. 
</br>To ensure the best performance, it is suggested to: 

- **Retopology you model if it's messy** 
  </br>If you ever did modeling, you know what I mean by that - proper flows of quad loops, uniform vertex valency, adaptive density of quads, etc. 
- **Triangulate your mesh(s)** 
  </br>For example, a triangulation modifier is required for a quad mesh / after a subdivision modifier. 
- **Avoid thin shells** 
  </br>For example, an old outline trick is to apply a solidify modifier and slightly extrude the surface into a shell of two layers. This causes StrokeGen to render lines for both layers, resulting in unpleasant results. 

