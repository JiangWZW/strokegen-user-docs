!!! bug large "Flickers"
    Flickering occurs for stylized lines when the camera / object is moving.
    </br>This happens because of multiple reasons:
    </br>**Inaccurate visibility**, **Unstable curve segmentation**, etc. 

    No existing renderer / research can solve this perfectly.
    </br>But I'm working on it. For details see the [**Roadmap**](./Roadmap.md) section. 

!!! bug large "Occasional Lagging"
    Lagging occasionally happens when you enable / disable StrokeGen globally or per-object.
    </br>This is due to StrokeGen preparing the GPU resources for processing your meshes. 