---
layout: project
title: AI-Assisted CAD + FEM Structural Optimization
description: An M.Eng. research project connecting generative geometry with implicit representations and GPU-accelerated structural analysis.
image: /assets/images/ai-cad-fem-prototype.jpg
imagealt: Prototype interface showing a generated elephant model with a displacement-magnitude visualization
hide_cover: true
technologies: [Python, Streamlit, TripoSG, NVIDIA Warp, PyTorch, CUDA, SDF, Octrees]
---

<p class="project-status">Cornell University M.Eng. Project · In progress</p>

**Advisor:** Prof. Nikolaos Bouklas  
**Collaborator:** Xueling Luo

## Project Overview

This project explores an AI-assisted workflow that connects generative geometry creation with GPU-accelerated finite element analysis and structural optimization. The goal is to reduce the engineering effort required to move from a design concept to an analyzable structure.

The developing system accepts text, images, or sketch-like inputs and generates an implicit 3D representation. The longer-term goal is to connect this representation directly to differentiable FEM and optimization, with an application and AI-agent layer coordinating the process.

## First Working Prototype

This recording documents the first working prototype of the software. It follows a text-to-geometry example using an elephant model, boundary-condition setup, and a mesh-based FEM result displayed as displacement magnitude. The interface brings generation and analysis into a single application; the later implicit-geometry and structural-optimization workflow remains under development.

<figure class="project-demo">
  <video controls muted playsinline preload="metadata" poster="{{ '/assets/images/ai-cad-fem-prototype.jpg' | relative_url }}" aria-label="Silent demonstration of the first working AI-assisted geometry prototype" aria-describedby="prototype-caption">
    <source src="{{ '/assets/videos/ai-cad-fem-prototype.mp4' | relative_url }}" type="video/mp4">
    Your browser does not support embedded video. <a href="{{ '/assets/videos/ai-cad-fem-prototype.mp4' | relative_url }}">Download the prototype demonstration</a>.
  </video>
  <figcaption id="prototype-caption">First working prototype · September 10, 2026 · Text-to-geometry, boundary-condition setup, and a mesh-based FEM displacement visualization. 72-second excerpt, without audio.</figcaption>
</figure>

## My Contributions

My work focuses on integrating the generative-design, user-interface, and engineering-analysis portions of the project.

- Developed and tested an early Streamlit interface for text prompts, uploaded images, and sketch/scribble inputs, connecting the application to TripoSG and displaying generated 3D results.
- Migrated toward Xueling Luo's `implicit_optimize` research codebase, integrating the interface and agent architecture with its implicit geometry pipeline.
- Configured and debugged the Python, CUDA, PyTorch, NVIDIA Warp, and TripoSG environment on a dual NVIDIA RTX A6000 GPU system.
- Tested text-to-implicit-geometry generation and successfully produced an octree through `text2octree.py`.
- Helped restructure application integration around wrapper functions in `src/triposg_wrapper`.
- Developed the foundation for an AI-agent layer to coordinate geometry generation and, eventually, simulation and optimization.

## Workflow and Current Status

The intended workflow connects six stages. The early prototype demonstrates geometry generation and mesh-based FEM feedback. Text-to-octree execution has also been demonstrated separately; connecting the newer implicit representation to FEM and optimization remains ongoing.

<ol class="research-workflow">
  <li><strong>User input</strong><span>Text descriptions, images, or sketches supplied through the application.</span></li>
  <li><strong>Generative geometry</strong><span>TripoSG-based tools generate a 3D representation.</span></li>
  <li><strong>Implicit representation</strong><span>Signed distance fields and octree data prepare geometry for downstream analysis.</span></li>
  <li class="in-development"><strong>Finite element analysis · Integration ongoing</strong><span>Connect implicit geometry to the GPU-accelerated NVIDIA Warp FEM pipeline.</span></li>
  <li class="in-development"><strong>Structural optimization · In development</strong><span>Use differentiable FEM to update the design against structural objectives.</span></li>
  <li class="in-development"><strong>Results and iteration · In development</strong><span>Return simulation and optimization results through the application.</span></li>
</ol>

## Completed Results

The initial Streamlit application demonstrated text-prompt-driven GLB generation and was expanded to support image and scribble inputs. The prototype recording also shows boundary-condition setup, mesh-based FEM solver output, and an interactive displacement-magnitude visualization. This is an early software demonstration, not a quantitative validation of analysis accuracy. The research environment was configured for NVIDIA Warp and GPU execution on two NVIDIA RTX A6000 GPUs.

Within `implicit_optimize`, the prompt **“a mechanical bracket”** successfully produced a valid `test_octree.pkl` through the text-to-octree pipeline. This establishes a working path from natural-language input into the implicit representation needed by downstream analysis tools. The octree result is a separate milestone from the early prototype recording above.

## Ongoing Work

- Implementing and testing `img2octree.py` and `scribble2octree.py` within the consolidated pipeline.
- Completing wrapper interfaces and connecting octree and signed-distance-field outputs to FEM.
- Connecting the AI agent to simulation and optimization functions.
- Returning analysis results to the interface, testing integration reliability, and improving setup documentation.

The intended outcome is a unified application for generating analysis-ready geometry, performing structural simulation and optimization, and inspecting the results in one place.
