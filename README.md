**[Home](https://yetgear.github.io/)**    **Project**



I'm graduated from the Information Department in BJUT, advised by Haiying Yuan, Pengyu Liu and Abraham Compbell. My research interests are computer graphics, compiler design, computer architecture.



# Selected Projects

### My Render Engine

#### Real-time Ray Tracing

<img src="https://raw.githubusercontent.com/Yetgear/Yetgear.github.io/master/resume-rtx.PNG" height="72px" align="right"> 

Powered by Nvidia RTX technology, this graphics pipeline manages to achieve ray tracing in real-time. It is able to render the specular of the light and shadows in the scene and provide great visual quality. This techniques enables the graphics developers to render the scene with realistic quality in real-time, thus it is the ultimate solution for real-time graphics.

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

#### And More advanced rendering techniques are available here [github](https://www.github.com) (coming soon..)

### VPU: Volume Processing Unit

An hardware implementation (IP Core) of SVO with slightly modification.  VPU, as same as Nvidia's RT Core, is designed to accelerate iteration of a tree structure. Whereas VPU can do more than RT cores, the former is able to accelerate not only Ray Tracing, but also fluid simulation, SLAM, 3-dimension object recognition/ segmentation and so on. Currently VPU is implemented in Xilinx SDSoc.

### WorldScript  

 a Heterogeneous computing and Geometric Representation Language run simultaneously on CPU and GPU. The GPU function of this Language is based on Vulkan Compute Shader and the CPU function is supported by LLVM. It takes the advantage of Signed Distance Function to represent and operate geometries. Currently the development of WorldScript  is still in a early stage, but functions listed above has been implemented, now I am working on the improvement of the structure robustness and overall performance. 

### Car Chassis Inspector

A robot which can inspect whether there is something abnormal on the chassis of target car by splice the image data captured by camera and then transfer to ground station to check whether there is something wrong on the chassis. The robot also equipped with a ground station implemented on Qt, which provides the function includes ground station server and client server on arm board, the driver of the arm board camera, the task scheduler of arm board, the picture splicer.
<u>All those Functions made entirely on my own.</u> 




