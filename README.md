# CRT and VHS Filter for Godot-4.1
Originally created by pend00, I took the liberty to port over his amazing shader. Check out his other works over at https://godotshaders.com/author/pend00/


An effect to simulate a CRT monitor or an old TV. It also has settings to make it look like an old VHS recording (discolorations, noise, and rolling distortion, check pend00 page for a visual reference).

This is a “true” CRT simulation with every scanline being divided into multiple sets of red, green, and blue squares – the technique called aperture grille.

It has many, many uniforms. I won’t list them all here but they include settings for scanlines, grille, pixels, discolorations, screen warping, noise, distortions, etc.


# Important instructions
You can use the shader in two ways:

   1 - To affect the node it is applied to, like a Sprite or ViewportContainer. Uncheck the Overlay parameter in the inspector.
  
   2 - As an overlay filter to affect the nodes below it in the Scene hierarchy. Add the shader to a ColorRect or TextureRect and check the Overlay parameter in the inspector.

The original shader had issues on MAC with it's overlay, I cannot confirm if my version works on MAC so feel free to let me know.
