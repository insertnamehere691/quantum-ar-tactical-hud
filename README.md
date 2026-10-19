# Quantum-Resistant AR/VR Tactical Data HUD

A proof-of-concept simulation framework designed to bridge **Post-Quantum Cryptography (PQC)** telemetry streaming with real-time 3D game engines (Unreal Engine / Unity) for secure AR/VR and holographic displays. 

## Overview
This project simulates a secure tactical telemetry stream where critical operational data is encrypted against future quantum decryption threats. It features a multi-threaded Python backend server that streams JSON-formatted telemetry packets over TCP sockets to be rendered onto immersive holographic UI interfaces in game engines.

## Features
* **Post-Quantum Simulation:** Generates structured tactical telemetry flags simulating NIST-standardized quantum-resistant encryption (e.g., Kyber-512).
* **Socket-Based Streaming:** Utilizes robust TCP socket management to handle continuous data transmission and client reconnections at a 1Hz refresh rate.
* **Game Engine Integration-Ready:** Designed to interface cleanly with C++ (Unreal Engine subsystems) and C# (Unity network receivers) for real-time spatial 3D visualization.

## Project Structure
* `pqc_telemetry_server.py`: The multi-threaded Python server that handles socket connections and broadcasts encrypted mock telemetry.

## Getting Started
1. Run the backend server locally:
   ```bash
   python pqc_telemetry_server.py
