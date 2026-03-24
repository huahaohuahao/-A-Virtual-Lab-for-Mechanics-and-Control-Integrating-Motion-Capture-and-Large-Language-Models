# Unity Intelligent Realm — A Virtual Lab for Mechanics and Control Integrating Motion Capture and Large Language Models

**Unity Intelligent Realm** is an open virtual simulation experiment platform built on the Unity engine, designed to bridge the disciplinary gap between classical mechanics and automatic control, providing students, educators, and researchers with a highly flexible, immersive, and scalable online experimental environment.

---

## ✨ Features

- 🧩 **Modular Component Design**  
  All experimental components are encapsulated as "prefabs," supporting free drag-and-drop, combination, and parameter adjustment. Users can construct their own experiments like building with blocks.

- 🔁 **Deep Integration of Mechanics and Control**  
  The platform integrates physical objects with control algorithms seamlessly through the `ISensor`, `IController`, and `IActuator` interface design, supporting real-time validation of classic control strategies such as PID on authentic physical models.

- 🧠 **Intelligent Interaction Experience**  
  - **Real-time motion capture** based on **YOLOv26**, supporting gesture recognition and natural manipulation.  
  - **Large language model (e.g., DeepSeek) voice interaction** integrated, enabling natural language commands to control experimental workflows.

- 📊 **Rich Data Visualization**  
  Built-in real-time charts, trajectory plotting, and other visualization tools help users intuitively understand physical quantities and control responses.

- 🌍 **Interdisciplinary Integration**  
  The platform not only supports mechanics and control experiments but can also be extended to fields such as thermodynamics and electronics, encouraging interdisciplinary exploration.

---

## 🏗️ System Architecture

The project adopts a three-tier client-server-resource management architecture:

- **Client (Unity 3D)** : Responsible for 3D rendering, user interaction, and integration of motion capture and voice modules.
- **Server (Simulation Computation)** : Executes complex dynamics calculations and control algorithms.
- **Resource Management Module** : Stores user data and experiment records, supporting experimental process analysis and intelligent recommendations.

---

## 🧪 Experiment Examples

| Experiment Name | Description |
|-----------------|-------------|
| Moment of Inertia Measurement Using a Three-Wire Pendulum | Use photoelectric counters, pendulum disk, weights, and other components to measure moment of inertia |
| Surface Tension Measurement Using the Cantilever Beam Method | Simulate strain gauges and multimeters to accurately calculate liquid surface tension |
| PID Ball Position Control | Use positional/incremental PID algorithms to achieve stable ball control under disturbance |
| Lissajous Figure Plotting | Visualize trajectory patterns at different frequency ratios using vibration synthesizers and laser pens |

> More than 28 experiments are currently supported, and users can freely design new experiments.

---

## 🧠 Intelligent Interaction Modules

### 🖐️ YOLOv26-Based Motion Capture

- Real-time capture of upper body skeletal data and gestures
- Maps hand movements to virtual models, enabling natural interactions such as grabbing, rotating, and assembling

### 🎙️ Large Language Model-Based Voice Control

- Supports natural language commands (e.g., "generate a pendulum," "start PID control")
- Combines speech recognition with large language model semantic parsing to drive scene object responses

---

## 📈 Evaluation Results

We conducted a comparative teaching experiment with 100 automation major students:

| Discipline | Experimental Group (Virtual Lab) | Control Group (Traditional Teaching) | p-value |
|------------|----------------------------------|--------------------------------------|---------|
| Mechanics | 83.11 ± 6.76 | 77.36 ± 4.53 | < 0.0001 |
| Control Theory | 77.91 ± 4.38 | 74.43 ± 4.83 | 0.0003 |

**User Satisfaction**:  
- Data Visualization: 4.5 / 5  
- Ease of Operation: 4.1 / 5  
- Interdisciplinary Integration: 3.8 / 5  
- 90% of students preferred using this platform for learning

---

## 🛠️ Technology Stack

- **Development Engine**: Unity 2022.3.49 LTS  
- **Render Pipeline**: Universal Render Pipeline (URP)  
- **Modeling Tool**: Blender  
- **Visualization**: XCharts  
- **Motion Capture**: YOLOv26  
- **Large Language Model**: DeepSeek (supports voice parsing)

---

## 📦 Quick Start
https://the-lab-of-physics-and-control.netlify.app/
### Requirements

- Unity 2022.3 LTS or higher
- GPU that supports URP
- Camera (for motion capture functionality)
- Microphone (for voice interaction)

