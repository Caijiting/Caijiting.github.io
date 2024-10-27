---
title: "Architect: Generating Vivid and Interactive 3D Scenes with Hierarchical 2D Inpainting"
collection: publications
category: conferences
permalink: /publication/paper2
date: 2024-09-01
venue: 'NeurIPS 2024'
paperurl: 'https://arxiv.org/pdf/2407.19666v1'
---

Creating large-scale interactive 3D environments is essential for the development of Robotics and Embodied AI research. However, generating diverse embodied environments with realistic detail and considerable complexity remains a significant challenge. Current methods, including manual design, procedural generation, diffusion-based scene generation, and large language model (LLM) guided scene design, are hindered by limitations such as excessive human effort, reliance on predefined rules or training datasets, and limited 3D spatial reasoning ability. Since pre-trained 2D image generative models better capture scene and object configuration than LLMs, we address these challenges by introducing 
, a generative framework that creates complex and realistic 3D embodied environments leveraging diffusion-based 2D image inpainting. In detail, we utilize foundation visual perception models to obtain each generated object from the image and leverage pre-trained depth estimation models to lift the generated 2D image to 3D space. While there are still challenges that the camera parameters and scale of depth are still absent in the generated image, we address those problems by ''controlling'' the diffusion model by 
. Specifically, having access to ground-truth depth and camera parameters in simulation, we first render a photo-realistic image of only the background. Then, we inpaint the foreground in this image, passing the geometric cues to the inpainting model in the background, which informs the camera parameters. This process effectively controls the camera parameters and depth scale for the generated image, facilitating the back-projection from 2D image to 3D point clouds. Our pipeline is further extended to a hierarchical and iterative inpainting process to continuously generate the placement of large furniture and small objects to enrich the scene. This iterative structure brings the flexibility for our method to generate or refine scenes from various starting points, such as text, floor plans, or pre-arranged environments. Experimental results demonstrate that 
 outperforms existing methods in producing realistic and complex environments, making it highly suitable for Embodied AI and robotics applications.
