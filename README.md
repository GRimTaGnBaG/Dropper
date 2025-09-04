# Dropper
Dropper attachment for drones


## Project Structure

This repo contains four Arduino sketches, divided into two system types:

### 1. Dropper Attachment (simpler payload release)
- **AT-Drone.ino** – Drone-side code for AT-command-driven payload dropper.
- **BaseStationAT.ino** – Base station code for communicating with the AT-Drone.

### 2. Dropper + Crane Attachment (advanced payload lift and release)
- **DroneCrane.ino** – Drone-side code for crane attachment with servo control.
- **Cranestation.ino** – Base station code for communicating with the DroneCrane.

---

### Usage Notes
- **Pick one system**:  
  - Use **AT-Drone + BaseStationAT** if you only want a simple dropper.  
  - Use **DroneCrane + Cranestation** if you want the dropper with crane functionality.  

- Open the `.ino` files in Arduino IDE or PlatformIO.  
- Select your board (ESP32) and correct COM port.  
- Upload the appropriate code to the drone and base station ESP32s.
