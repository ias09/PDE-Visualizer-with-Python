# PDE Visualizer: Heat, Wave, and Laplace Equations

This repository provides a Python script (Google Colab-ready) that demonstrates how to solve and visualize three fundamental classes of Partial Differential Equations (PDEs):

- **Elliptic PDE** → **Laplace Equation**
- **Parabolic PDE** → **Heat Equation**
- **Hyperbolic PDE** → **Wave Equation**

The script uses **Fourier sine-series (eigenfunction expansions)** to enforce homogeneous Dirichlet boundary conditions:

- For **Heat** and **Wave** equations:  
  \( u(0,t) = u(L,t) = 0 \)

- For **Laplace equation** in a rectangle:  
  \( u(0,y) = u(L_x,y) = u(x,0) = 0 \), and \( u(x,L_y) = \phi(x) \)

---

## Features

✅ **Heat Equation (Parabolic)**
- Solves \( u_t = \alpha^2 u_{xx} \) with Dirichlet BCs.  
- Uses a customizable initial condition \( u(x,0) = f(x) \).  
- Generates **2D snapshots** and **3D surface plots** of the solution over time.  

✅ **Wave Equation (Hyperbolic)**
- Solves \( u_{tt} = c^2 u_{xx} \) with Dirichlet BCs.  
- Allows both initial displacement \( u(x,0)=f(x) \) and initial velocity \( u_t(x,0)=g(x) \).  
- Produces **time evolution plots** and **3D animations of oscillations**.

✅ **Laplace Equation (Elliptic)**
- Solves \( u_{xx} + u_{yy} = 0 \) on a rectangular domain.  
- Supports a nontrivial boundary condition at the top edge \( u(x,L_y)=\phi(x) \).  
- Visualizes solution with **contour plots** and **3D surfaces**.

---

## Requirements

The script only uses standard scientific Python libraries:

- `numpy`
- `matplotlib`

Both are pre-installed in Google Colab. No extra dependencies are required.

---

## Usage

1. Clone this repository:

```bash
git clone https://github.com/your-username/pde-visualizer.git
cd pde-visualizer
