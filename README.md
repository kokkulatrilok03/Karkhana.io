# Karkhana.io

Python code to model and visualize a Möbius strip using parametric equations. Includes numerical surface area and edge length estimation, with interactive 3D plotting via matplotlib.

# Möbius Strip Visualization 🌀

This project models a Möbius strip using parametric 3D equations in Python. It includes:

- A `MobiusStrip` class for generating mesh coordinates
- Numerical approximation of:
  - Surface area (via double integration)
  - Edge length (via distance calculation)
- 3D visualization using `matplotlib`

---

## 🧠 Parametric Equations

\[
x(u,v) = (R + v \cdot \cos(u/2)) \cdot \cos(u)  
\]
\[
y(u,v) = (R + v \cdot \cos(u/2)) \cdot \sin(u)  
\]
\[
z(u,v) = v \cdot \sin(u/2)  
\]

Where:
- \( u \in [0, 2\pi] \)
- \( v \in [-w/2, w/2] \)

---

## 📦 Requirements

```bash
pip install numpy scipy matplotlib
🚀 Usage
from mobius_strip import MobiusStrip

mobius = MobiusStrip(R=1.0, w=0.4, n=300)
print(f"Surface Area ≈ {mobius.surface_area():.4f}")
print(f"Edge Length ≈ {mobius.edge_length():.4f}")
mobius.plot()
📊 Output
Surface Area: Computed via 2D Simpson’s Rule

Edge Length: Summation of boundary segment distances

Visualization: Rendered using matplotlib 3D surface plots

💡 Applications
3D geometry and topology education

Mesh generation and rendering

Surface integration and geometric computation


---
