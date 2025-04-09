# 🦿 Biomechanical Simulation of a Kick — 2D Leg Model

This project uses **SymPy**, **PyDy**, and **Matplotlib** to model and simulate the dynamics of a human kick, focusing on a 2D analysis of the leg (thigh and shin).

The simulation includes graphical visualization of angular kinematics, linear motion, reaction forces, and an animation of the leg's movement during the kick.

---

## ⚙️ Model Description

The leg is modeled as a system of two rigid bodies:

- **Thigh**: Body 1 (mass `m1`, length `l1`)
- **Shin**: Body 2 (mass `m2`, length `l2`)

The bodies are connected by rotational joints with generalized coordinates `q1` and `q2`, with the hip fixed in space.

The equations of motion are derived using Kane’s method via the PyDy library.

---

## 📚 Dependencies

- [SymPy](https://www.sympy.org/en/index.html) – symbolic mathematics
- [PyDy](https://www.pydy.org/) – multibody dynamics modeling
- [NumPy](https://numpy.org/) – numerical operations
- [SciPy](https://scipy.org/) – numerical integration
- [Matplotlib](https://matplotlib.org/) – plotting and animation

Install all dependencies via pip:

```bash
pip install sympy pydy numpy scipy matplotlib
```

📈 Simulation Outputs
The following plots are generated:

Angular Kinematics:
Position, velocity, and acceleration of q1 (thigh) and q2 (shin)

Linear Kinematics:
Velocity and acceleration of the foot

Forces and Torques:
Reaction forces at the hip and knee joints

Generalized torques from the dynamic model
A 2D animation of the leg performing a kick is also rendered using Matplotlib.

▶️ How to Run
Clone this repository or download the script.
Ensure the dependencies are installed.

Run the script:

```
python kick_simulation.py
```

The script will display the plots and play the animation.

🛠️ Adjustable Parameters
You can customize the following parameters directly in the script:

Lengths: l1, l2
Masses: m1, m2
Gravity: g
Initial conditions: q1, q2, u1, u2
Simulation duration: t_max

🚀 Future Improvements
Include muscle forces (Hill-type muscle models)

Add ground contact and impact dynamics
Export results to CSV or MATLAB for further analysis
Create an interactive GUI with parameter sliders

👤 Author
Developed by Israel Mendes Fernandes — Mechanical Engineer with interests in biomechanics, multibody systems, and dynamic simulations.

📄 License
This project is open-source and available under the MIT License.
