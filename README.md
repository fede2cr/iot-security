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
- [ ] LiPo batteries that report charge
- [ ] Weatherproof devices
- [ ] Wireless charging
- [ ] Very low false positives, to increase confidance when alerts happen

## Sensors

For detecting intruding humans, the idea is to use:

- [Human body detection module](https://www.crcibernetica.com/rcwl-0516-human-body-detector-module/): Uses microwaves and doppler effect to sense human presence. Because of heavy transit of other primates (capuchin monkeys and howler monkeys) this has to be tested so that it does not create false positives. Expected range: 5m-7m.
- [ESP32-cam](https://www.crcibernetica.com/esp32-with-camera/) or IMX462: Cameras that work well at night, either with light control or a low light optimized sensor to capture clear and useful images/video to detect human presence. This images/video should be offloaded for archival and for processing with Microsoft's Megadetector. The face detection features from the ESP32 can also be used, if tested properly with non-human-primates.
