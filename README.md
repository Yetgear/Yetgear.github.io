**[Home](https://yetgear.github.io/)**    **Project**



I'm currently a final year student in School of Automation at BJUT, advised by Haiying Yuan and Pengyu Liu. My research interests are computer graphics, compiler design, computer architecture.



# Selected Projects

### My Render Engine

#### Sparse Voxel Octree Path Tracing
<img src="https://raw.githubusercontent.com/Yetgear/Yetgear.github.io/master/resume-rtgi-1.PNG" height="72px" align="right">  
a real time path tracing pipeline implemented on Sparse Voxel Octree, which consists of GPU Voxelization pass, Sparse Octree Building pass, Data Filling Pass and path tracing pass. SVOPT runs fairly 100 fps on my computer, which reaches real time frame rates standard. This render pipeline could combine with rasterzation to provide great quality CG effect.

#### Physical Based Rendering with Image Based Lighting 
<img src="https://raw.githubusercontent.com/Yetgear/Yetgear.github.io/master/resume-pbr-ibl.PNG"  height="72px" align="right">
A standard implemention of PBR Rendering pipeline and Image Based Lighting. 

#### Signed Distance Field Global Illumination 
<img src="https://raw.githubusercontent.com/Yetgear/Yetgear.github.io/master/resume-sdf-gi.jpg" height="72px" align="right">
Another solution for real time Global Illumination. Similar to Unreal Engine 4's design, the render pipeline renders the SDF data transfered from the origin triangle data by ray marching. Because the sdf data is stored in 3D textures, the render pipeline is able to ultilize the Tri-lateral filter to filte the distance data and achieve fast frame rate.

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



#### A complete list can be found [here](https://www.github.com).
