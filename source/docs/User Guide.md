# Best Practices

## Prepare your mesh

Like any other rendering algorithm, the performance of StrokeGen depends on the quality of your mesh. 
</br>To ensure the best performance, it is suggested to: 

??? note large annotate  "Cleanup messy topology"
    At least, fix all non-manifold geometry (1) and keep a meaningful poly-density for your quads/triangles. 
    </br></br>It would be better if the mesh has been carefully modeled or re-topologized. 
    </br>For 3D modeling people, you know what I mean - quad flows, vertex valency, density of quads, etc. 
1.  Non-manifold geo mainly appears in scanned or brutally simplified meshes. In Blender, enter edit mode, "*select > select All by trait > Non Manifold*" to view them, 

??? note  large "Triangulate your mesh(s)"
    For example, a triangulation modifier is required for a quad mesh / after a subdivision modifier. 

??? note  large "Avoid thin shells"
    For example, an old outline trick is to apply a solidify modifier and slightly extrude the surface into a shell of two layers. This causes StrokeGen to render lines for both layers, resulting in unpleasant results. 


