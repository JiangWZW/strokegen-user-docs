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

## Performance Tips

In the beta version, StrokeGen follows a conservative strategy: 
</br><span style="color:#c35340">Each StrokeGen-enabled object should under two million triangles.(1)
{ .annotate } 

1. This will change as the development continues. </span> 

!!! note large "Notes from the developer" 
    StrokeGen consists of intricate and complex GPU code, making it much harder to maintain than normal code.
    
    I only have limited time & energy for it - I developed it alone during my free time, and I need to work to feed myself :smiling_face_with_tear: . 
    
    Considering the variety of users' GPUs, I decide to keep a conservative design. If you think this tool has potential, please provide your feedback on Discord, so that I can gradually improve it & optimize it. 

