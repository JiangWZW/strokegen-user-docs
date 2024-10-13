![Image title](img/StrokeGen.svg){ align=left }
The goal of StrokeGen is to empower 3D artists with a powerful tool for creating high-quality line art. 
</br>It is developed as a customized Blender build(1) by Wangziwei Jiang(2). 
{ .annotate } 

1. Why not a plugin? Because the core algorithm requires deep integration with Blender's viewport and GPU modules, which is not possible with a python plugin. 
2. Who is Wangziwei Jiang? A graphics programmer and 3D artist who is passionate about NPR and has been working on this project for years.

<div class="grid cards" markdown size="50%">

-   :octicons-download-16: __Downlads__

    [Beta Releases](https://github.com/JiangWZW/strokegen-releases/releases)
    </br>Stable Releases

-   :material-book-open-outline: __Tutorials__

    [Quick Start](./Quick%20Start.md)
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
![](img/0.png){: .off-glb slot="first" }
![](img/1.png){: .off-glb slot="second" }
</img-comparison-slider>



<div class="grid cards" markdown>

-   :material-account-group:{ .lg .middle } __Driven by Community__

    ---
    Strokegen is still in development, and your feedback is essential to its success.
    
    :octicons-arrow-right-24: Join the [Discord](https://discord.gg/9Q45afM2Es) community to share your thoughts and ideas.

-   :material-scale-balance:{ .lg .middle } __Open Source__

    ---
    Strokegen is open-source software, and you can find the source code on [GitHub](https://projects.blender.org/WangZiWei-Jiang/fork-npr-strokegen.git)
    </br>If you are interested in contributing to this project, joint the Discord community and let us know.

</div>





## Roadmap
The current version of StrokeGen is a beta release, 
</br>the main goal is to improve the stability of the software and improve the user experience. 
</br>However, there are some exciting features planned for the future: 

=== "Temporal denoiser" 

    Improve the flicker of stylized curves. 
    </br>There is already a backbone for this feature, 
    </br>but any further development requires the feedback from the community.

=== "Intersection curves"

    Generate intersection curves for two or more objects. 
    </br>The goal is to implement a GPU-based algorithm for this feature and make it real-time.
    </br>This feature is still in the research phase.

=== "AI shading / colorization"
    
    Implement a neural network for cel shading and colorization. 
    </br>This feature is still in the research phase, 
    </br>and I am looking for collaborators to help me with this.