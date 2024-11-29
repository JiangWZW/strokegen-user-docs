
![Image title](../img/StrokeGen.png){ align=left style="height:370px;width:535px" }
</br>StrokeGen is a customized Blender build(1) developed by Wangziwei Jiang(2). 
{ .annotate } 

1. Why not a plugin? Because the algorithm requires deep integration inside Blender, which is not possible with a python plugin. 
2. Who is Wangziwei Jiang? ![](../img/avatar_1.png){: .off-glb .image-left } A graphics programmer and 3D artist who is passionate about NPR and has been working on this project for years.




<div class="grid cards" markdown size="50%">

-   :octicons-download-16: __Downlads__

    :octicons-arrow-right-24: [Beta Releases](https://github.com/JiangWZW/strokegen-releases/releases)
    </br>:octicons-arrow-right-24: Stable Releases

-   :material-book-open-outline: __Tutorials__

    :octicons-arrow-right-24: [Quick Start](./Quick%20Start.md)
    </br>:octicons-arrow-right-24: [Best Practice](./Best%20Practices.md)
</div>

##Features

<div class="grid cards" style="margin-bottom: 0;" markdown>

-   :material-brush: __Elegant curve topology__
    
    ---
    Generate curves with a visually pleasant topology, essential for creating high-quality line art.

-   :simple-rocket: __Real-time response__

    ---
    StrokeGen is designed to provide real-time feedback, allowing you to focus on your art.
</div>


<script
  defer
  src="https://cdn.jsdelivr.net/npm/img-comparison-slider@8/dist/index.js"
></script>
<link
  rel="stylesheet"
  href="https://cdn.jsdelivr.net/npm/img-comparison-slider@8/dist/styles.css"
/>
<img-comparison-slider markdown=1>
![](../img/0.png){: .off-glb slot="first" }
![](../img/1.png){: .off-glb slot="second" }
</img-comparison-slider>



<div class="grid cards" markdown>

-   :material-account-group:{ .lg .middle } __Driven by Community__

    ---
    Strokegen is still in development, and your feedback is essential to its success.
    
    :octicons-arrow-right-24: Join the [Discord](https://discord.gg/9Q45afM2Es) community to share your thoughts and ideas.

-   :material-scale-balance:{ .lg .middle } __Open Source__

    ---
    Strokegen is open-source software, and you can find the source code on [GitHub](https://projects.blender.org/WangZiWei-Jiang/fork-npr-strokegen.git)
    
    In the future, if the feedbacks were good, we plan to merge the code into official Blender.

</div>





## Roadmap
StrokeGen is in the beta stage, and the current goal is to improve the stability and user experience.
</br>However, there are some exciting features planned for the future:

=== "Temporal stablizer" 

    Improve the flicker of stylized curves to make StrokeGen feasible for animations.
    </br>There is already a backbone for this feature, 
    </br>but any further development requires the feedback from the community.

=== "More curve types"

    Generate intersection/crease/shadow/highlight curves from the 3d surface. 
    </br>The goal is to implement a GPU-based algorithm for this feature and make it real-time.
    </br>This feature is still in the research phase.

=== "Grease Pencil"
    
    Support seamless conversion between strokegen curves and Grease Pencil strokes.
    </br>If possible, our temporal denoiser can be used to track Grease Pencil drawings. 

=== "AI shading / colorization"
    
    Implement a diffusion model for interactive cel shading and colorization. 
    </br>This feature is still in the research phase, 
    </br>and I am looking for collaborators to help me with this.

The development of StrokeGen depends on the feedback from the artist community, 
</br>please join the [Discord server](https://discord.gg/9Q45afM2Es) and share your thoughts and ideas!