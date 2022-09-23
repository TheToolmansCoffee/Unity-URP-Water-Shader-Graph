# Unity-URP-Water-Shader-Graph
## A flexible and easily editable water shader for Unity. Made in Shader Graph.

![watershadermain](https://user-images.githubusercontent.com/93699568/191806620-c5d76c41-c1be-458f-a1f9-1c73622c9d18.PNG)

## Properties

![properties](https://user-images.githubusercontent.com/93699568/191807124-5f08e7d5-82a8-41a2-a358-193cf220070e.PNG)

### Water Color - The color of the water, of course (also depends on Metallic, Smoothness, Normal Power & Transparency) Defaults to cyan.

### Normal & Sub Normal - Two normal maps that are panned around the mesh to fake more detail while keeping framerates stable. (THE ONES YOU SEE HERE ARE *NOT* INCLUDED IN THIS PACKAGE!)

### Normal Power - Power of the two normal maps. Defaults to 1.

### Normal Tiling - Tiling of the the normal maps. Should be bigger for bigger models, defaults to 1x1.

### Water Normal Speed - The speed of which the first normal map scrolls. Higher numbers equal slower motion. Max. speed is 100. Defaults to 0.

### Water Normal Speed 2 - The speed of which the second normal map scrolls. Lower numbers equal faster motion. Max. speed is -100. Defaults to 0. SHOULD BE NEGATIVE!

### Wave Scale - The amount of the actual 3D vertex waves. The waves are on the GPU, which means that this option doesn't affect performance, but it still is by no needs needed to be used. Defaults to zero.

### Wave Speed - The speed of the 3D vertex waves. Higher numbers equal slower motion. SETTING THIS OPTION TO NEGATIVE AMOUNTS, OR TO 1-20 MIGHT SLIGHTLY AFFECT PERFORMANCE. Even if the 3D waves aren't being used, this setting needs to be set to AT LEAST 0.0001, or the water object will not render! It's a weird glitch, and sadly seem to have no way to be fixed.

### Transparency - The transparency of the object. 0 = Not visible, 1 = No transparency.

## Water in action

### I'd say that the shader is still missing important features, such as foam & actual reflections that aren't based of the skybox, but I will not publish those features to this shader once I've added them. And the reason why is because this shader is meant to be used as either a base, or a reference for your own shader. But by all means, if you feel like it, use this horrible mess of a shader

Here the shader is viewed in the editor with the parameters from above. I would've uploaded a video, but that has proven to be difficult, so instead, here are a bunch of screenshots!

![waterfromeditor](https://user-images.githubusercontent.com/93699568/191811712-b3a4eec5-1b76-4d2c-8b0c-b59e57f8a11f.PNG)

Here, as you can see, are 20 vertex-heavy planes taken straight from Blender without any changes made running in-engine in a decent FPS, with a fairly bad PC.

![devices](https://user-images.githubusercontent.com/93699568/191812544-904e279d-3dce-4b62-a57e-0724a6b6ef89.PNG)

![watervertices](https://user-images.githubusercontent.com/93699568/191812272-4a456717-15ab-4134-93e6-6289642b2d31.PNG)

![stats](https://user-images.githubusercontent.com/93699568/191812722-42070072-052e-46e9-bb90-204dac5a2640.PNG)

And from the side, to prove that the vertex waves are being used

![watervertices](https://user-images.githubusercontent.com/93699568/191812926-fba13257-fdf9-4486-bba6-e7fb8e8a5a20.PNG)

In shaded mode,

![watervertices](https://user-images.githubusercontent.com/93699568/191813102-a8ec3c03-1347-482f-a092-2880d2f59f9d.PNG)

Shaded wireframe,

![watershadedvertices](https://user-images.githubusercontent.com/93699568/191813330-7d2cd3da-9440-44ca-ba08-83f07996a0a9.PNG)

And let's finish with a few wide shaded pictures.

![waterfromup](https://user-images.githubusercontent.com/93699568/191813665-728663e2-f1d5-4cc6-98cc-cffb19a30f37.PNG)

![waterlastpic](https://user-images.githubusercontent.com/93699568/191813842-fe23b6c9-a340-47ec-b75d-38e5b48891c0.PNG)

## A few things that might be slightly confusing.

SKYBOX NOT INCLUDED

I know that the rep name is "URP Water Shader Graph", but for all I'm aware of, this should work even with HDRP and Built-in! And if not straight from the get-go, it shouldn't be too hard to port over. 

The bright yellow/orange shimmering seen in some of the pics is just the realtime directional light reacting to the smoothness & metallic values. And it of course changes based on your water color, sun color and smoothness/metallic values.

## What this shader is meant for

I created this shader for my own means, and I'm even using it in my current project, (or pevious project, depending on when you're reading this) Totally Medieval. I decided to throw it out here, because I realized that it's pretty damn amazing, even though it's very simple. Plus I like helping people :) Now, I don't really intend for this shader to be used right from the get-go in the project, but instead as a temporary asset, or as a base or reference for your own shader! But as said slightly above, by all means, you're free to use this, even with commercial projects.

## Licensing & Final Words

(MIT License) Yeah, the license might sound pretty scary at first, but it's nothing that bad. Basically all I'm asking you is to add the first few lines from the license (as stated in the license file) to a credits page of your project. This is mainly because I do also like to get some credit from my (be it very bad) work ;)
(Also applies to if you're using this as a reference or as a base for your own shader)

Hopefully you'll enjoy this mess! 

Yours truly,

The remotely professional (and pretty bad),

Timi/"Tespinen", proud shader nerd.

(Jokes aside, this was probably my first shader I did in my three years of Unity, and I'm quite proud of it. Be it mainly a mess, it did spark a passion of shader creation)

Enjoy, and thanks for checking this out.

(ps. If you're facing problems or need any help, just DM me on Discord, Tespinen#1070, or ping me on the official Unity server)

# Preferences

##### What I used to learn/as a reference

[URP water shader tutorial from Unity](https://youtu.be/gRq-IdShxpU)
