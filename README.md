# Building Occupancy & Waiting Room Dashboard

A Raspberry Pi–based smart-building system for monitoring room occupancy, waiting-room activity, and building status in real time.

## Overview

This project was developed to solve a practical problem in a multi-office clinical environment: determining which rooms are occupied, whether clients are waiting, and what is happening throughout the building without requiring staff to manually update a centralized system.

The system uses smart-building devices and a locally hosted Raspberry Pi application to translate physical activity within the building into a simple visual dashboard.

## Key Features

- Real-time room occupancy monitoring
- Whole-building occupancy count
- Individual room status
- Waiting-room/lobby status display
- Occupancy timestamps and event history
- Empty-building detection
- Smart-switch integration
- Matter/device discovery
- Lighting and dimming controls
- Administrative dashboard
- Dedicated lobby/kiosk interface
- Local data storage
- Raspberry Pi deployment

## Architecture

The system is designed around a Raspberry Pi acting as the local application server and building-control hub.

```text
Smart Switches / Sensors
          ↓
 Matter / Local Network
          ↓
      Raspberry Pi
          ↓
 Occupancy Processing
          ↓
     Local Storage
          ↓
 ┌───────────────┬───────────────┐
 │ Admin Display │ Lobby Display │
 └───────────────┴───────────────┘
```

## Technologies

- Raspberry Pi
- Node.js
- TypeScript
- HTML/CSS/JavaScript
- Matter
- Local network device discovery
- Smart switches
- Local data storage

Earlier prototypes also explored Google Sheets and browser-based dashboards before the system transitioned toward a locally hosted Raspberry Pi architecture.

## Design Goals

The system was designed around several principles:

**Local first** — Core building functions should continue operating without dependence on a cloud service.

**Passive interaction** — Staff should not need to manually update room occupancy.

**Immediate visibility** — Building status should be understandable at a glance.

**Expandable architecture** — Additional sensors and building systems can be incorporated over time.

## Future Development

Potential extensions include:

- Indoor/outdoor pressure monitoring
- HVAC status integration
- Environmental sensors
- Automated ventilation monitoring
- Temperature and humidity monitoring
- Building energy monitoring
- Historical occupancy analytics
- Additional Matter-compatible devices
- Automated alerts based on building conditions

## Project Status

Active development / prototype deployment.

The project continues to evolve as additional building sensors and automation capabilities are added.
