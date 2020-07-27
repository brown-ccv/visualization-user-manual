---
description: >-
  Although Fiji is a 2D viewer, this plugin will help you to open 3D meshes,
  Tiff Stacks and other 3D formats
---

# ImajeJ 3D Viewer

Once you open Fiji, go to Plugins-&gt; 3D Viewer

![](../../../.gitbook/assets/image%20%284%29.png)

A window will pop up

 

![](../../../.gitbook/assets/image%20%2812%29.png)

Most of the plugin's documentation can be found in the following link

```text
https://imagej.net/3D_Viewer:_User_FAQs
```

Here, we will guide you on the basic usage with a short example.

Download the following dataset.

{% file src="../../../.gitbook/assets/3d\_chromosome.tif" caption="Example Data" %}

Go to **File -&gt; Open**  and select the example data. You should see the following.

![](../../../.gitbook/assets/image%20%2813%29.png)

Do right click  on the ImajeJ 3D Viewer window and drag the mouse to rotate. Use the Mouse wheel to zoom in and out. Holding Shift, do right click on the image and drag the mouse to translate the view.

![](../../../.gitbook/assets/image%20%2822%29.png)

Let's play with it analyzing and editing the datasets channels. In this example, we are going to highlight the internal representation of the chromosome. For that we will use transfer functions.

Go to Edit -&gt;  Transfer function.

![](../../../.gitbook/assets/image%20%2814%29.png)

The graph at the left represents the value of pixels vs their transparency value. You can see the function for each of the channels RGB \(red, green, blue\). We want to remove the yellow block surrounding the dataset. Yellow is the combination of red and green, let's modify the transfer function on those two channels. You can do and hold left click on the graph and drag the mouse to change the shape of the function.

![](../../../.gitbook/assets/image%20%2826%29.png)

![](../../../.gitbook/assets/image%20%2811%29.png)

You can export this model in any of the available formats for ImajeJ 3D Viewer.

Go to **File -&gt; Export -&gt; WaveFront.**   It will export it as a .obj file that can easily be opened in other 3D editors.





