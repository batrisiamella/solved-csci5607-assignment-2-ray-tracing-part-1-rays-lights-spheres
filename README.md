Download Link: https://assignmentchef.com/product/solved-csci5607-assignment-2-ray-tracing-part-1-rays-lights-spheres
<br>
Overview:In this assignment, you will create a simple ray-tracing application capable of rendering scenes consisting of spheres lit by point light sources. Scenes will be described in a simple, easy to parse text specification file. This is part 1 of a two-part assignment. In the second part you will extend this raytracer to incorporate triangle meshes, more complex lighting, and other extensions for more realistic images.Grading Note:This assignment takes the place of a check-in for the ray tracer. As such, it will be graded quickly and based only on the images you turn in, in order to give you quick feedback. The next assignment (HW3, Raytracing – Part 2) will be graded as normal. For this check-in, you may work with a partner, but you must work alone for HW3.Getting Started:You already have the stb_image_write.h library from HW1. You can use this to create BMP outputs. You may also wish to use SDL or GLFW to create an interactive UI for displaying and modifying your scenes. All other code you should write from scratch.A simple scene format has been posted online [SceneFile.pdf], this contains information on the camera, all objects, lights and materials in the scene, and output formats. You may need to extend it to implement new features, but be sure you can also support existing files in this format. We have uploaded some scenes consisting of only spheres to get you started [SphereExamples.zip]. NB: My rendering of these scenes contains some features such as reflection and refraction, which you do not need to implement until Part 2.Submission Instructions:Create a sample webpage with:-Your source code-Output images-You must show at least one of the sample scenes along with several newscenes of your own designed to show off each feature of your raytracer.-Brief description of your implementation, any issues you saw, and a list ofany extra credit tasks you attempted -Submission to Art Contest (optional)Assignment Requirements:As this is a two-part assignment, Part 1 will be graded out of 50 pts. The number is front is how many points the feature is worth. Partial credit will be given to features that “mostly” work. The required minimum feature set is underlined.

Scene Setup:(5) Camera placement, film resolution, aspect ratio (5) User specified background colors(5) UI + OpenGL output(5) BMP or PNG outputPrimitives:(5) Spheres(5) Difference/Intersection of spheres (Constructive Solid Geometry)Lighting:(5) Ambient lights(5) Point light sources(5) Shadows(5) Multiple light sources (5) Directional light sources (5) Spot light sourcesSampling:(5) Basic Sampling(5) Jittered Supersampling (5) Adaptive Supersampling (5) Motion Blur(5) Depth of FieldMaterials:(5) Color &amp; Specularity (Phong Lighting Model)(5) Refraction (5) ReflectionHints:features. First generate a black image of the correct dimensions. Then create a scene with just a sphere. Have your raytracer return white whenever it hits the sphere. You should see a white sphere on a black background. Now make sure you feel confident in your ray/sphere intersection code. Move the sphere around, make sure the right things happen. When this works, mess around with the image aspect ratio (make it very narrow), make sure everything works as expected. Then try to get material colors working. Then add support for point lights, then phong shading. Only move on to a new feature when you’re sure everything else works so far.-If you don’t do this, you’ll end up with a big pile of broken code and neither I nor the TAs will be able to help you.-Please, please test as you go along!-See the posted HW2 strategy guide [RayTracing-StrategyGuide.pdf]-Test your program incrementally-Honestly, incremental testing will really help!-Get some very small thing working first then move on to more complex