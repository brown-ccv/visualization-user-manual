---
description: >-
  Image segmentation is the process of partitioning a digital image into
  multiple segments (sets of pixels, also known as image objects). Fiji give us
  multiple tools to separate and analyze data.
---

# Segmentation

We are going to identify particles inside the following image.

![](../../.gitbook/assets/image%20%289%29.png)

Please download the file.

{% file src="../../.gitbook/assets/cell\_colony.jpg" %}

Open Fiji and go to File -&gt; Open and select the file.

We want to transform the image's data into a binary file where any algorithm can identify different pieces of it. First, let's check the Image pixel color histogram. Go to Image -&gt; adjust threshold. Click Auto in the pop up window.

![](../../.gitbook/assets/image%20%2831%29.png)

The particles are the darker points or blobs inside the image. Some of the points \( the smaller ones \) are not painted in red, so we are going to play with the slides to include them as part of the data we have interested in. The first slide controls the lower bound of the threshold, and the second slide the upper bound. Keep the value of the former and increase the value of the latter.

![](../../.gitbook/assets/image%20%2821%29.png)

Unfortunately, by increasing the maximum value of the threshold to include more points, some noise data has been added to the result image. This could be due to the background noise. Let's try to fix this. IN the menu bar Go to Image -&gt; Duplicate and pre-append "bg" to the name of the file and click ok.

Go to Process -&gt; Filters  and select Gaussian Blur. Check the Preview option, and play with different values in the pop up window.

![](../../.gitbook/assets/image%20%287%29.png)

When you find the right value, do click on ok. This image represents an smoother version of the image, with a reduced level of noise. Let's operate the two images. In the menu bar go to Process -&gt; Image calculator. In the Image 1 drop list select the original image, and in the Image 2 drop list select the background filtered image. Select Divide in the operation drop list.  Check Create new window and 32 bit float result.

![](../../.gitbook/assets/image%20%285%29.png)

We have a less noise version of the image. Transform it to 8 bit. Go to Image -&gt; type and select 8 bit.



![](../../.gitbook/assets/image%20%2833%29.png)

Next, go to Process -&gt; Binary -&gt; Options and check Background. Click ok.  In our example objects of interest will be displayed white on black background

Now, let's see the histogram of this new image and fix the threshold. Select Image -&gt; Adjust -&gt; Threshold. Now can increase the upper limit, and more points will be painted red without including the background noise.

![](../../.gitbook/assets/image%20%2832%29.png)

Adjust the threshold as much as you like and then click on Apply.

![](../../.gitbook/assets/image%20%2825%29.png)

At this point, you can pass the resulting image over to an algorithm to analyze it. For example, we can identify and level the particles.  On the Menu bar go to Analyze -&gt; Analyze particles,  check the clear results option, in the show combo list select Outlines and click Ok.

![](../../.gitbook/assets/image%20%2824%29.png)

