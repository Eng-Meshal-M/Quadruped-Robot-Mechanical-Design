# 🤖 Simple Quadruped Robot - Preliminary Mechanical Design

> **Designed by:** Meshal Talal AL Mehmady  
---

## 📌 Task Purpose
The goal of this task is to design a simple, entry-level mechanical structure for a 4-legged robot (robotic dog) using **Tinkercad**. The focus is on learning the basic mechanics required to make the robot stand and walk, without advanced or complex systems.

<img width="1230" height="951" alt="Screenshot 2026-07-06 033459" src="https://github.com/user-attachments/assets/65d0b6c6-57a6-411f-9ee6-9acbd4e23893" />

---

## 🛠️ Chassis & Body Features

### 1. Main Structure
The body is a simple, hollow rectangular chassis designed to hold the basic electronics (such as an Arduino board and a small battery).

- **Side Door:** A simple grey panel on the side to easily open the robot and check the wiring.
- **Buttons:** Red and green buttons on the chassis to easily turn the robot ON and OFF.

<img width="1077" height="663" alt="Screenshot 2026-07-06 033537" src="https://github.com/user-attachments/assets/b6755c5b-a486-4a09-bece-beca85f25e72" />

### 2. Charging Port
- **Power Input:** On the other side, there is a simple circular opening labeled **"5V IN"** for a standard DC jack to charge the battery directly.

<img width="2049" height="861" alt="Screenshot 2026-07-06 035836" src="https://github.com/user-attachments/assets/3b2881fe-3276-42d5-adfa-8a29b6505eff" />

---

## 🦵 Legs & Joints (Degrees of Freedom)

- **Leg Design:** Each leg consists of two main parts (thigh and shank). Different colors are used to make the structure easier to understand.
- **Joints & DoF:** Each leg has **2 joints** (one hip joint and one knee joint). With 4 legs, the robot has a total of **8 Degrees of Freedom (8 DoF)**. This simple layout is enough for a basic quadruped robot to stand and perform simple walking motions.

---

## ⚡ Motor Choice & Simple Torque Logic

- **Selected Motors:** The design is made to fit standard **MG996R servo motors**. They are affordable, easy to control using a microcontroller, and have metal gears that are suitable for a beginner robotics project.

- **Basic Torque Idea:**
  - Estimated robot weight: **2 kg**
  - During movement, two legs may support most of the robot's weight, so one leg is assumed to carry about **1 kg** (≈10 N).
  - Assuming a leg length of **10 cm (0.1 m)**:

  $$
  \text{Torque} = 10\text{ N} \times 0.1\text{ m} = 1\text{ N.m}
  $$

  which is approximately **10.2 kg·cm**.

  Since the **MG996R** servo can provide up to **11 kg·cm** of torque, it is suitable for this preliminary design.

---

## 🚶 Walking & Balance

- **Center of Gravity:** The battery and electronics are placed near the center of the chassis to improve balance and stability.
- **Proposed Gait (Static Crawl):** The robot lifts only one leg at a time while the other three legs remain on the ground. This provides better stability for a simple quadruped robot.

---

## ⚠️ Expected Mechanical Problems

1. **Gear Backlash:** Low-cost hobby servos may have a small amount of gear play, causing slight joint movement.
2. **Joint Friction:** 3D-printed parts may rub against each other, reducing movement efficiency.

---

## 📚 Learning Reference

This task was created as part of my self-learning journey in robotics. I first learned the basic design concepts from YouTube tutorials, then modified the design by adding my own ideas, such as the side maintenance panel, control buttons, charging port, the **"5V IN"** label, and my name to better match the task requirements.
