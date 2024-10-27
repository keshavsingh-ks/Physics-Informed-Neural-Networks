# Physics-Informed-Neural-Networks
 
Overview

This repository showcases my journey into Physics-Informed Neural Networks (PINNs), applying them to physics and computational fluid dynamics (CFD). The projects cover a progression from simple ordinary differential equations (ODEs) to complex partial differential equations (PDEs), highlighting the practical use of PINNs to solve real-world physics problems.

Learning About PINNs

My journey began with the idea of leveraging neural networks to solve physics problems by embedding physical laws into the loss function. The combination of data-driven learning with physics-informed constraints felt groundbreaking and opened a new way of using deep learning for scientific computing.

### Project 1: 1D Harmonic Oscillator (ODE)
![img1](https://github.com/keshavsingh-ks/Physics-Informed-Neural-Networks/blob/main/deepxde1.png)
I started with the 1D underdamped harmonic oscillator using TensorFlow. The model combined data loss and physics loss to solve the ODE, providing a foundation in training networks to obey physical laws. This taught me the limitations of optimizers like Adam in converging to precise solutions.

### Project 2: Heat Equation with DeepXDE (PDE)
![img2](https://github.com/keshavsingh-ks/Physics-Informed-Neural-Networks/blob/main/deepxde3.png)
Next, I tackled PDEs using DeepXDE to solve the heat equation. DeepXDE helped me understand how to define geometries, use boundary conditions, and combine time and space domains. It highlighted the power of physics-informed loss functions for simulating physical processes without traditional meshing.

### Project 3: Cylinder Wake with TensorFlow - Adam vs. L-BFGS-B
![img3](https://github.com/keshavsingh-ks/Physics-Informed-Neural-Networks/blob/main/TvPTFU.png)
Moving to fluid dynamics, I modeled the cylinder wake using Navier-Stokes equations in TensorFlow. Initially using Adam yielded decent results, but switching to L-BFGS-B significantly improved precision, demonstrating its strength in overcoming local minima. This project deepened my understanding of fluid dynamics and how PINNs can simulate complex flow directly.

### Project 4: Burgers' Equation in PyTorch
![img4](https://github.com/keshavsingh-ks/Physics-Informed-Neural-Networks/blob/main/Burger%20Equation.png)
I then tackled the Burgers' equation in PyTorch, adding initial condition loss, boundary condition loss, and PDE residual loss. Balancing these losses allowed the network to learn the dynamics effectively, enhancing my understanding of how initial and boundary conditions influence fluid behavior.

### Project 5: Revisiting Cylinder Wake with PyTorch
![img5](https://github.com/keshavsingh-ks/Physics-Informed-Neural-Networks/blob/main/PTCW.png)
I revisited the cylinder wake problem using PyTorch to solve the full Navier-Stokes equations. Using LBFGS optimization, I accurately modeled fluid flow past a cylinder, capturing the formation and shedding of vortices. This project was a significant milestone, applying everything I had learned to a challenging CFD scenario.

Key Learnings and CFD Applications

PINNs: Embedded physical laws into loss functions to solve ODEs and PDEs.

Optimization: Compared Adam and L-BFGS-B for training PINNs, noting L-BFGS-B's superior precision.

DeepXDE: Used DeepXDE for solving PDEs like the heat equation.

Burgers' and Navier-Stokes: Applied PINNs to Burgers' equation and Navier-Stokes for real-world scenarios like the cylinder wake.

CFD without Meshing: Explored solving CFD problems without numerical grids, demonstrating PINNs' scalability.

Conclusion

These projects demonstrate my journey in applying PINNs to physics and CFD, from simple ODEs to complex fluid flows like the cylinder wake. This exploration shows how deep learning can bridge the gap between data-driven models and physics-based insights. Feel free to explore each project, and reach out if you'd like to collaborate or discuss further!
