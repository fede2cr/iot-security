# iot-security
A physical security system, using IoT communications and sensors

## Introduction

This is a physical security system, designed for detecting human intrussions in private land. It will be modified slowly to also work as a biodiversity camera trap, but only when the security goals are working correctly.

## Goals

- [ ] Human detection sensors that use an external pin for interrupt
- [ ] Deep Sleep with external interrupt connected to the sensors
- [ ] Comms via espnow mesh
- [ ] Comms via LoRa
- [ ] Area configuration and coverage mapping (using esp32+GPS mapper)
- [ ] Camera and light control
- [ ] External human detection on camera with Microsoft Megadetector
- [ ] Remote camera viewing from external console
- [ ] Easy display of triggered areas
- [ ] Panic mode for calling for help on other external consoles connected to the system
- [ ] Archival of events for debugging and for interaction with authorities
