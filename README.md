**[Home](https://yetgear.github.io/)**    **Project**



I'm currently a Ph.D. candidate in University College Dublin mentored by Abraham G. Campbell with research interests of real-time rendering system development, unified shading language development, large-scale scene visualization. 



# Selected Projects

### VirtualVoxel - Ph.D. Research

#### VirtualVoxel: Render 4194304^3 (4M^3) resolution voxel scene at 167 fps under 4K
<img src="https://raw.githubusercontent.com/Yetgear/Yetgear.github.io/master/resume-virtualvoxel.PNG" height="72px" align="right">

#### VirtualVoxelCrowd: Render 1 Biilion human characters at real-time under 4K
<img src="https://raw.githubusercontent.com/Yetgear/Yetgear.github.io/master/resume-virtualvoxelcrowd.PNG" height="72px" align="right">

### My Render Engine - Ph.D. Project
<img src="https://raw.githubusercontent.com/Yetgear/Yetgear.github.io/master/resume-new-engine.PNG" height="72px" align="right">

#### Virtual Shadow Map

#### Screen Space Reflection & Shadow & AO

#### Visibility Culling

### Unified Graphics Language - Ph.D. Project
<img src="https://raw.githubusercontent.com/Yetgear/Yetgear.github.io/master/resume-ugl.PNG" height="72px" align="right">

#### Write CPU & GPU Code In The Same Language
#### RenderGraph
#### Static Code Validation
#### Virtual Shader Table for Specialization


### My Render Engine - Undergraduate Project

#### Real-time Ray Tracing

<img src="https://raw.githubusercontent.com/Yetgear/Yetgear.github.io/master/resume-rtx.PNG" height="72px" align="right"> 

Powered by Nvidia RTX technology, this graphics pipeline manages to achieve ray tracing in real-time. It is able to render the specular of the light, AO, irradiance and soft shadows in the scene and provide great visual quality. This techniques enables the graphics developers to render the scene with realistic quality in real-time, thus it is the ultimate solution for real-time graphics.

#### Fast Fourier Transformation Based Ocean

<img src="https://raw.githubusercontent.com/Yetgear/Yetgear.github.io/master/resume-ocean.PNG" height="72px" align="right"> 

an ocean rendering solution for real-time graphics, it uses the compute shader to calculate the fft of the spectrum of ocean and generates a vector map of ocean.  This technique provides a flexible solution for realistic ocean rendering.

#### Infinite Terrain Rendering With Physically Based Atmosphere 

<img src="https://raw.githubusercontent.com/Yetgear/Yetgear.github.io/master/resume-terrain.PNG" height="72px" align="right"> 

a terrain rendering solution for real-time graphics, it uses the tessellation shader to generate a mesh-pyramid according to height map. The physically based atmosphere models the sky by mie and Rayleigh Scattering. This solution enables the graphics developers to render the infinite natural scene efficiently.

#### Position Based Dynamics Engine

a real-time physics engine solution, which enables the system to be stable in large simulation step. It uses Morton code and hash code to handle collisions, then projects the correction based on constraints. Due to the limitation of time, I only implemented the collision constraint and rigid body constraint. This technique is able to leverage the parallel computing to support the simulation of massive dynamic objects.

#### Voxel Cone Tracing

<img src="https://raw.githubusercontent.com/Yetgear/Yetgear.github.io/master/resume-vxgi.png" height="72px" align="right">  
a real-time global illumination solution for graphics engine, which provides rough reflection and irradiance of the scene to render. It firstly uses GPU Conservation Rasterization to voxelize the scene to provide the 3D GBuffer, then fetch the global render data in the scene by cone tracing. This technique enables the graphics developers to achieve not only the tradition GI effect, but also manage to do volume rendering in graphics application. 

#### Sparse Voxel Octree Path Tracing
<img src="https://raw.githubusercontent.com/Yetgear/Yetgear.github.io/master/resume-rtgi-1.PNG" height="72px" align="right">  
a real time path tracing pipeline implemented on Sparse Voxel Octree, which consists of GPU Voxelization pass, Sparse Octree Building pass, Data Filling Pass and path tracing pass. SVOPT runs fairly 100 fps on my computer, which reaches real time frame rates standard. This render pipeline could combine with rasterization to provide great quality CG effect.

#### Physical Based Rendering with Image Based Lighting 
<img src="https://raw.githubusercontent.com/Yetgear/Yetgear.github.io/master/resume-pbr-ibl.PNG"  height="72px" align="right">
A standard implementation of PBR Rendering pipeline and Image Based Lighting. 

#### Signed Distance Field Global Illumination 
<img src="https://raw.githubusercontent.com/Yetgear/Yetgear.github.io/master/resume-sdf-gi.jpg" height="72px" align="right">
Another solution for real time Global Illumination. Similar to Unreal Engine 4's design, the render pipeline renders the SDF data transferred from the origin triangle data by ray marching. Because the sdf data is stored in 3D textures, the render pipeline is able to utilize the Tri-lateral filter to filter the distance data and achieve fast frame rate.

#### SVGF-space: the space part of SVGF Filter
<img src="https://raw.githubusercontent.com/Yetgear/Yetgear.github.io/master/resume-svgf-space.jpg" height="72px" align="right">
A real time ray tracing denoiser to reduce the noise on Ray Tracing image. The denoiser is capable to work on a wide range of ray tracing techniques and produce a denoised image with fine quality though only one sample ray is applied to per pixel.



### VPU: Volume Processing Unit

An hardware implementation (IP Core) of SVO with slightly modification.  VPU, as same as Nvidia's RT Core, is designed to accelerate iteration of a tree structure. Whereas VPU can do more than RT cores, the former is able to accelerate not only Ray Tracing, but also fluid simulation, SLAM, 3-dimension object recognition/ segmentation and so on. Currently VPU is implemented in Xilinx SDSoc.






