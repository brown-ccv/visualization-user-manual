---
description: This is a better option to load image stacks. It's a more mature plugin.
---

# Volume Viewer

Download the following dataset.

{% file src="../../../.gitbook/assets/3d\_chromosome.tif" caption="Example Data" %}

Open Fiji, go to File -&gt; Open and select the example dataset.

![](../../../.gitbook/assets/image%20%2828%29.png)

Now, keeping the image on top , go to Plugins -&gt; Volume Viewer



![](../../../.gitbook/assets/image%20%2819%29.png)

You will get the following pop up window

![](../../../.gitbook/assets/image%20%2822%29.png)

The official documentation of the plugin cab be found in the following link

```text
https://imagej.net/plugins/volume-viewer.html
```

It is a bit short. Here we are going to play using our example data.

The default view displays a cross section of the data. Let's display the whole volume. The first option of the top menu bar allows you to change the visualization mode. It is set at slice, switch it to volume.

![](../../../.gitbook/assets/image%20%2823%29.png)

Press and hold the mouse left click and drag the mouse to rotate the DataSet

![](../../../.gitbook/assets/image%20%282%29.png)

The different slice representations from different planes are show at the left side of the window. You can see an specific part of the interior of the dataset by moving the slice bars at the bottom left. The top left images will be updated according to the slice index.

![](../../../.gitbook/assets/image%20%283%29.png)

At the right side you can find the transfer function of the data set. We can modify the color space of the data. Switch from Original to GrayScale.

![](../../../.gitbook/assets/image%20%288%29.png)

Switch to thermal. This scale is made to determine cold \(blue\) to hot\(red\) temperatures

![](../../../.gitbook/assets/image%20%2820%29.png)

Try to play with the transfer function graph to change the color of the purple block surrounding the data. Below the graph you can modify the transparency \(alpha value\) of the RGB values according to the color function.

![](../../../.gitbook/assets/image%20%2829%29.png)

You can UNDO all the changes using the button RESET at the top right.

