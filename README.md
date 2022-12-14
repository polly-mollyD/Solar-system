
780.214 – Introduction to Computer Graphics Summer Term, 2022 <br />
Project Write Up <br />

# SOLAR SYSTEM IMPLEMENTATION IN BLENDER

Palina Dubatouka, 12116714 <br />
## Introduction
The illustration of the Solar System in Blender implementation will be
presented and discussed in the given project report. The general idea is to develop
a model that can take the approximate positions, masses and velocities of some
planets and illustrate a realistic picture of the Solar System. <br />
As these planet’s movements/motions are very hard to be captured from a
real-time camera, computer graphic techniques can be utilized and equipped as
another solution to generate the same expected frame of a planet’s movement.
Blender is a program designed for any type of movie graphics. It has many
lighting and angle capabilities, as well as a three-dimensional coordinate system. <br />
This report outlines the methods used to visualize the artificial Solar
System and presents a short animation (10 sec.) of created Solar System as a final
achievement of the project.

## Objects

The Solar System is the planetary system with the sun and planets. There
are eight planets in total that orbit the Sun. For the given model implementation
three planets have been taken as well as the Moon and the Sun.

### Texture

Initially, the planets are simple UV spheres. Materials of the planets
have been taken as an Image Texture from the internet [1].

![My Image](images/photo_2022-12-02_00-21-21.jpg) <br />
Earth <br />

![My Image 1](images/2k_moon.jpg) <br />
Moon <br />

![My Image 2](images/2k_venus_surface.jpg) <br />
Venus <br />

![My Image 3](images/2k_mercury.jpg) <br />
Mercury <br />

In the middle of the scene – Sun, I chose a specific material to
represent it. This is a yellow color material with Bloom, Ambient Occlusion
and Motion Blur effects on. Further improvements have been made in
Shader Editor: <br />

![My Image 4](images/photo_2022-12-02_00-15-43.jpg) <br />
![My Image 5](images/photo_2022-12-02_00-15-12.jpg) <br />
<br />

### Rotation

Since the Sun is located in the World Origin I can set the Origin of
each of the planets to the “Origin to the 3D Cursor”, by that I will be able to
rotate the planets in the orbit around the Sun. Different settings are applied
to the Moon since its orbit is located around the Earth. Thus the World
Origin should be set in the middle of the Earth. <br />
The table below shows the actual parameters for the planets but for
this project I took the approximate values for the distance from the Sun,
diameter, rotation time, and speed: <br />

![My Image 6](images/photo_2022-12-02_00-14-14.jpg) <br />

Planetary Fact Sheet – Metric [2] <br />
The parameters for the planets of the scene are presented in the table
below (the interpolation is set to Linear for each planet): <br />

![My Image 7](images/photo_2022-12-02_00-16-22.jpg) <br />

Sun Mercury Venus Earth Moon <br />

The rotation around the Y-axis of the planets (around itself) can be done
in the following way for each of the planets but with the different values (can be
seen in the table above): <br />

![My Image 8](images/photo_2022-12-02_00-16-43.jpg) <br />
![My Image 9](images/photo_2022-12-02_00-17-44.jpg) <br />

## Light
To represent how the light works in the solar system, the directional
light type is selected. With directional light, the planets will have the lights
based on the direction from the light source. The main source of light is set
up in the center of the scene over the Sun and illuminates all the other
planets. It makes the effect of the Sun lighting to the planets. The Area light
has the shape of a disk and power of 4500 W which makes it possible to
light the distant elments of the scene. <br />

![My Image 10](images/photo_2022-12-02_00-18-17.jpg) <br />

## Blender result
The obtained video of 10 seconds captures all the developments which I described
above. The overall issue of the work with Blender for me was only my lack of
experience. The right movement implementation, texture and light initialization
cause huge time spent. Rendering a two-dimensional image taking into
consideration 3D objects, virtual camera and light sources take a lot of effort to
make it acceptable for presentation. <br />

For the planets it is not sufficient to apply just a shape and color, some
additional properties should be initialized, for instance, high-quality image
textures, which also require a lot of memory. Adding functions such as random
noise, and Worley noise can make the material more detailed. <br />

Just correctly installing the light sources can change the whole presentation
for a better way considering the fact that lights in general make the picture more
realistic. It is necessary to understand what is the right position of light should be
set and what type of light should be chosen. <br />

During the implementation, I have been using the data from the lecture
slides as well as I found it useful to search on the Internet for more specific aspects
of my Solar System project. I hope the resulted video can successfully represent
the learned techniques and skills I acquired in the given course. <br />

## References
[1] Free Solar Textures. https://www.solarsystemscope.com/textures/ <br />
[2] Planetary Fact Sheet. https://nssdc.gsfc.nasa.gov/planetary/factsheet/ <br />
[3] Tutorial - How to make 3D Animation of Solar System easily using Blender
software <br />
