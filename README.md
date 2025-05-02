# 📡 Electromagnetic Wave in Free Space Medium using MATLAB

This project models and simulates the behavior of electromagnetic (EM) waves in an ideal free space medium using MATLAB. It demonstrates the transverse nature of electric and magnetic fields as they propagate without attenuation, following Maxwell’s equations.

---

## 📚 Abstract

Electromagnetic waves travel through free space at the speed of light, governed by Maxwell’s equations. This project focuses on simulating and visualizing these waves using MATLAB, providing insights into wave propagation, impedance, polarization, and phase relationships. The simulation outputs show electric and magnetic fields oscillating orthogonally and propagating in the x-direction.

---

## 🎯 Objectives

- Understand EM wave propagation in a vacuum.
- Visualize the electric and magnetic field components.
- Simulate plane wave equations using MATLAB.
- Study the effect of parameters like frequency, impedance, and direction.

---

## 🧮 Mathematical Foundation

The time-harmonic equations used in the simulation are:

Ey(x, t) = E0 * cos(ωt - βx)

Hz(x, t) = (E0 / η) * cos(ωt - βx)


Where:
- `E0` = Amplitude of electric field  
- `ω` = Angular frequency  
- `β = ω / c` = Phase constant  
- `η = 377 Ω` = Intrinsic impedance of free space  
- `c = 3 × 10⁸ m/s` = Speed of light in vacuum

---

## 💻 MATLAB Code

```matlab
clear all;
close all;
clc;

c = 3 * 10.^ 8; % speed of light
w = 10.^8; % angular frequency of wave
beta = w/c; % Phase constant
t = -1.5:0.01:1; % time
x = -1.5:0.01:1; % space (direction of propagation)
m = zeros(size(t));

Ey = 30*cos(w*t - beta *x); % electric field
Hz = (30/377)*cos(w*t - beta*x); % magnetic field

figure(1);
plot3(x,Ey,m,'r'); % Plotting 3d electrical wave
hold on;
t = -1.5:0.01:1;
plot3(x,m,Hz,'g'); % Plotting 3d magnetic wave
grid on;
hold off;
ylabel('Electric Field');
zlabel('Magnetic Field');
xlabel('Direction of Wave');
title('Em Wave components in Free Space Medium');
view(10,10);

```

## 📊 Output and Visualization

- A 3D plot shows both the electric field (red) and magnetic field (green) propagating orthogonally.
- The fields are in phase and maintain constant amplitude, demonstrating transverse propagation.
- Helps understand polarization and wave impedance visually.



## 📌 Applications

- 📡 Wireless and Satellite Communication
- 🌌 Deep Space Signal Transmission
- 📶 Antenna Design
- 📻 Radar and Microwave Engineering
- 🛰️ Electromagnetic Wave Research

## 📁 Documentation

- [Project Report PDF](https://github.com/DuttPanchal04/EM-Waves-in-Free-Space-Using-MATLAB/blob/main/ELECTROMAGNETIC%20WAVE%20IN%20FREE%20SPACE%20MEDIUM%20USING%20MATLAB.pdf)

## 📘 Key Learnings
- Visualizing Maxwell’s equations in action
- MATLAB as a tool for EM field simulation
- Relationship between electric and magnetic field components
- Theoretical + practical understanding of EM wave propagation

## 🤝 Connect
- Project by Dutt Panchal.
- 📧 Email: dattpanchal2904@gmail.com
- 🔗 [Github](https://github.com/DuttPanchal04)
- 🔗 [LinkedIn](https://www.linkedin.com/in/dattpanchal04/)

⭐ If you found this project helpful or insightful, please consider starring the repository!