# Control y Simulación de un Péndulo de 1 Grado de Libertad (1-DOF)

**Autor:** Profesor Abdiel Mercado
**Plataforma:** ROS 2 Jazzy + Gazebo Harmonic

Este repositorio contiene un proyecto didáctico completo para simular un robot tipo péndulo simple (1-DOF) y controlarlo mediante inyección de torque (esfuerzo) mientras se leen los datos de un sensor inercial (IMU) en tiempo real.

## 📦 Estructura del Proyecto

El proyecto se compone de dos paquetes principales de ROS 2:
1. `robot_1dof_sim`: Paquete CMake que contiene el modelo físico (URDF), la configuración de los controladores de hardware (YAML) y los archivos Launch para orquestar Gazebo y RViz.
2. `robot_1dof_control`: Paquete Python que contiene el nodo de control en lazo cerrado, el cual inyecta una señal senoidal de torque y se suscribe a los datos de la IMU.

---

## 🚀 Tutorial de Instalación y Ejecución

Sigue estos pasos para replicar el proyecto en tu computadora. Se asume que ya tienes instalado Ubuntu 24.04 y ROS 2 Jazzy.

### Paso 1: Crear el Espacio de Trabajo
Abre una terminal y crea la estructura base del workspace:
```bash
mkdir -p ~/robot_1dof_ws/src
cd ~/robot_1dof_ws/src
