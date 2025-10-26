# Traffic-Light-Controller
The purpose of this project is to design a methodology using Verilog to control the traffic with specified time delays for a T-Shaped road.

## 📘 Table of Contents
1. [Introduction](#introduction)
2. [Methodology](#methodology)
   - [Directions Considered](#directions-considered)
   - [Problem Statement](#problem-statement)
   - [State Diagram](#state-diagram)
   - [State Table](#state-table)
3. [RTL Code](#rtl-code)
   - [RTL Schematic View](#rtl-schematic-view)
4. [Testbench](#testbench)
5. [Output Waveforms](#output-waveforms)
6. [References](#references)


## Introduction

Traffic congestion and road safety are two of the most common challenges in today’s rapidly growing cities. Uncontrolled intersections often lead to confusion, delays, and accidents, especially at T-junctions where three different traffic flows meet. To address this problem, an intelligent traffic signal controller can be used to manage the movement of vehicles in a systematic and collision-free manner.

This project focuses on designing a T-junction traffic light controller using a finite state machine (FSM) approach. The system controls traffic flow from three roads — two from the main road and one from a side road — by sequencing green, yellow, and red signals based on predefined timing and safety rules. Each signal phase is carefully designed to allow smooth movement of vehicles in one direction while preventing conflicts from other lanes.

The FSM-based design makes the system deterministic, reliable, and easily scalable. Each state in the controller represents a specific traffic phase, such as:
- TMG – Main Road Green  
- TY – Main Yellow  
- TTG – Turn Green  
- TSG – Side Green  

Transitions between these states are triggered by timing signals, ensuring safe vehicle movement, reduced waiting time, and efficient traffic coordination even under heavy flow conditions.

Overall, this project demonstrates how digital logic design and state machine control can be effectively applied to real-world problems like urban traffic management, offering a smart and cost-efficient alternative to manual or sensor-based systems.


## Methodology

### Directions Considered
The directions M1, MT, M2, and S are considered for analysis in this project.  
They represent the main road and side road traffic flow in the T-junction.

<p align="center">
  <img src="traffic_light_controller_direction.jpg" alt="Directions Considered" width="500"><br>
  <em>Figure 1: Directions considered for T-junction</em>
</p>
