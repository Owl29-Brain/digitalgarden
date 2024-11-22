---
{"SR":"SR01255368-01","tags":["Visualize","SOLIDWORKS"],"dg-publish":true,"permalink":"/3-d-experience-solidworks-questions/custom-texture-application-in-solidworks-and-visualize/","dgPassFrontmatter":true}
---

# Problem Statement 
While applying the custom texture file becomes distorted when applied to a model in SOLIDWORKS/Visualize. The distortion appears as the texture either being stretched or duplicated across the surface. 

Despite trying different mapping methods, the correct appearance could not be achieved due to the image size. There is a suggestion to blend duplicated textures as a potential solution, but it's unclear if SOLIDWORKS/Visualize supports this feature.

# Response 1 
The issue the customer is facing isn't specific to SOLIDWORKS or SOLIDWORKS Visualize; it would occur with any software where an image or texture is applied to a surface significantly larger than the image itself. The options are either scaling the image, which stretches it, or patterning it, which may result in visible joins if the image isn't designed for tiling. The quality of the result depends entirely on the design of the image.

If you look at standard SOLIDWORKS textures, like those in `‘C:\Program Files\Dassault Systemes\SOLIDWORKS 3DEXPERIENCE\SOLIDWORKS\data\Images\textures’
they are designed for seamless tiling, where the edges align perfectly to avoid visible joins. This allows for effective scaling without distortion.

The methods you've already tried—scaling or patterning—are the only ones available in SOLIDWORKS and SOLIDWORKS Visualize for applying the texture. To achieve the customer's desired result, it’s recommended to either use a different image that can be repeated without noticeable joins or edit the current image using photo manipulation software to make it seamless.

# Response From Myside
If there are specific size formats or image types responsible for achieving a perfect blend when applying standard texture files. Noticed that all the standard textures were in square format and JPG type, so similar settings but still didn’t get the desired seamless result. The customer is asking if there are any other parameters that need to be considered for a perfect texture blend.


# Response 2
You may find the following QA articles useful regarding the size, shape and quality of the images used:
- [[3DExperience SOLIDWORKS Questions/Is it possible to scale a texture to fit onto a rectangular face. SOLIDWORKS always seems to distort the texture.\|QA00000117944]] Is it possible to scale a texture to fit onto a rectangular face? SOLIDWORKS® always seems to distort the texture. 
- [[3DExperience SOLIDWORKS Questions/QA00000104714\|QA00000104714]]: On a large scale model building, when applying a brick material to the faces there are a very few number of bricks even with the scale turned all the way down. How can a realistic brick look for the building be achieved? 
- [[3DExperience SOLIDWORKS Questions/Why customized textures appear blurred into final render\|QA00000114613]]: Why customized textures appear blurred into final render? 

With the customers image simply resizing it will not help with the repeatability of the image in a pattern. The image is different shades at each side, and has a different edge pattern so will not match up.