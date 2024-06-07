# Bump vector to normal map node group

 This is a little Blender shader node group which converts the output of a Bump node into a tangent space normal map. Useful if you want to create a normal map from a shader without the need for baking.

This .blend file also contains it being used with a procedural plaster/drywall texture to demonstrate it. It was created with Blender version 4.1.1 Stable so I reccomend that you use this with that version or later.



# How to get started

1. Open up a new Blender window

2. Set `Render Properties > Color Management > View Transform` to `Raw`. This ensures that the color info will be exported correctly.

3. Go to `File > Append`.

4. Use the newly opened browser to search for the .blend file in the repository.

5. Once you find the .blend file, double-click on it. This will take you inside the .blend file.

6. Double-click the `NodeTree` folder. There should be one NodeTree called `Bump Vector to Normal Map`.

7. Hit Append.

8. Make a new material. It should start off with a Principled BSDF.

9. Create a Bump node, and attach something like a Noise Texture node into the Height socket.

10. Plug the output of the Bump node into the Normal socket of the Principled BSDF.

11. Plug the output of the Bump node into the Surface socket of the Material Output.

12. Add the appended NodeTree by going to `Add > Group > Bump Vector to Normal Map`. Insert it between the Bump node and the Material Output. You should see that it generated a normal map texture.



# Created by catboy-catfish on GitHub. Credit is appreciated.






