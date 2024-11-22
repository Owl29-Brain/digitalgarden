---
{"SR":"QA00000117944","tags":["Service_Request"],"dg-publish":true,"permalink":"/3-d-experience-solidworks-questions/is-it-possible-to-scale-a-texture-to-fit-onto-a-rectangular-face-solidworks-always-seems-to-distort-the-texture/","dgPassFrontmatter":true}
---

# Is it possible to scale a texture to fit onto a rectangular face? SOLIDWORKS® always seems to distort the texture.

SOLIDWORKS® textures are always square (horizontal pixels = vertical pixels), and if the source bitmap is not square then SOLIDWORKS® stretches it to make a square texture. To use a non-square bitmap as a texture, and avoid distortion, use image editing software to add some blank space above or to the right of the image, until it is square. This bitmap does not distort when used in a texture, and can be scaled to move the blank area off the target surface.

This solution is suitable for images that must fit exactly onto a rectangular surface.