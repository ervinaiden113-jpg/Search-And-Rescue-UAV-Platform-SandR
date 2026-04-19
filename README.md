![Nexus UAV](images/Screenshot%202026-04-19%20060240.png)





# Search-And-Rescue-UAV-Platform

SandR Nexus is a compact semi-autonomous electrical vertical takeoff and landing (eVTOL) Unmanned Aerial Vehicle (UAV) purpose built for search and rescue (SAR) missions.
Nexus is designed for rapid deployment by first responders and SAR teams. Nexus combines semi-autonomous flight planning, computer vision based victim detection, and reliable
failsafe systems all within a small portable airframe built to be field diverse. The goal is to put capable autonomous search technology in the hands of teams who need it most, without the cost or complexity of enterprise systems.




# Key Features

# Autonomous Waypoint Navigation
Pre-planned waypoint missions planned in the ArduPilot Mission Planner software. Operators can define search grids or custom flight paths before launch with minimal pilot input required in the field.

# Victim/Object Detection
Custom CV pipeline built for real-time inference for SAR missions. The model is trained to detect humans across varied terrain and lighting conditions.

# Return To Home
Automatic (RTH) Return To Home failsafe on signal loss, low battery, or system failure scenarios. The vehicle recovers itself safely without operator intervention.

# GCS Integration
Full telemetry, live video, and mission control data via MAVLink compatible GCS. Operators get a real-time picture of the mission from the ground.



# Why I Chose To Build Nexus

Most SAR drones are either too expensive for small teams to field, too large to backpack into a wilderness search zone, or too limited to actually do anything useful without an expert pilot present. I wanted to bridge this gap by building something that actually matters. I love drones — in fact the last 3 years I have dedicated to building drones with purpose. From Nexus, a search and rescue drone, to Firefly, a wildfire detection drone, to AeroRelief, a medical delivery drone — building drones that solve real problems is one of my favorite things to do.

# How To Use Nexus
1. Power On & Connect to Ground Control Station
After assembling the aircraft and completing ArduPilot setup, power on the Nexus UAV outdoors with a clear sky view. Connect your laptop or computer to the aircraft using telemetry radio, Wi‑Fi, or USB. Open Mission Planner or any MAVLink‑compatible ground control station. Wait for the HUD to show GPS lock, EKF OK, and healthy sensors. This establishes the live link for telemetry, mission upload, and real‑time monitoring.

2. Load or Create a Waypoint Mission
Nexus supports fully autonomous waypoint navigation. In Mission Planner, open the Flight Plan tab and draw a search grid, lawnmower pattern, or any custom SAR route. Set the mission altitude, speed, and behavior, then click Write to upload the mission to the aircraft. Verify the mission items in the Data tab before flight. This allows you to pre‑plan efficient search patterns with minimal pilot workload.

3. Arm & Launch
Once the mission is loaded, switch the flight mode to AUTO or transition from FBWA to AUTO depending on your workflow. Arm the aircraft after all pre‑arm checks pass. The Nexus will take off automatically if configured for auto‑takeoff, or you can perform a manual launch. The aircraft will immediately begin executing the waypoint mission. Failsafes such as Return‑to‑Home, geofence protection, and battery failsafe remain active throughout the flight.

4. Real‑Time SAR Monitoring
During flight, the ground control station provides live telemetry including position, altitude, battery status, and attitude. Mission progress is displayed in real time. If equipped, a live video feed is available through FPV or a companion computer stream. The onboard computer‑vision model provides real‑time detections, and all detections and flight data are automatically logged. This gives operators a complete picture of the search area as the mission runs.


# Contributing
PRs welcome. Open an issue first for anything significant. I would love to have meaningful contributions to this project — whether that's improvements to the CV pipeline, flight controller configs, or airframe design!


# Images Of Nexus


![Nexus UAV 1](images/Screenshot%202026-04-18%20031229.png)
![Nexus UAV 2](images/Screenshot%202026-04-18%20031229.png)
![Nexus UAV 3](images/Screenshot%202026-04-17%20035021.png)

# Electrical System Architecture

![Electrical System Architecture](images/Screenshot%202026-04-19%20133850.png)

# BOM

![BOM](images/Screenshot%202026-04-19%20091853.png)

# Instructions
see instruction manual in misc folder for print orientation print settings and assembly guide.

# UPDATES

I'll be adding config files and Ardupilot parameter files after my project gets approved and I get my flight controller in.
