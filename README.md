# Toyota bZ4X Dashboard Project

This project folder contains configuration and assets related to the Toyota bZ4X Home Assistant dashboard.

<img src="https://i.imgur.com/iTS27gL.jpeg" width="50%" alt="Toyota bZ4X Dashboard">

## Features
- **All-in-One Monitoring:** A unified view of all critical vehicle stats (security, tires, battery, and location) designed for high visibility and ease of use.
- **Effortless Climate & Power:** Remote start your vehicle and monitor EV battery levels and estimated range from a single, polished interface.
- **At-a-glance Security:** Instantly see if the car is unlocked or if any doors/trunk/hood are open with intuitive bubbles for each item and alert highlighting.
- **Proactive Maintenance:** Intuitive highlighting alerts you when tire pressure drops to 35 PSI or below.
- **Real-time Location Tracking:** Integrated map view to monitor your vehicle's current location and parking status at a glance.
- **Nearby Charger Availability:** Real-time monitoring of available nearby ChargePoint chargers, dynamically placed higher on the dashboard when your vehicle's battery is low.

## Files
- **Requirement:** [ha-toyota-na](https://github.com/widewing/ha-toyota-na) (Toyota North America custom integration for vehicle data).
- **Requirement:** [Bubble Card](https://github.com/Clooos/Bubble-Card) (custom card used for the layout and highlighting).
- `dashboard_config.json`: Exported dashboard configuration.
- `start_bz4x_script.json`: Exported remote start script configuration.
- `chargepoint_sensors.yaml`: REST sensor configuration for nearby ChargePoint chargers. **Note: Copy and paste this content into your Home Assistant `configuration.yaml`.**
- `bz4x.png`: Required vehicle image used for the dashboard's picture card.

## Key Entities
- **Lock:** `lock.2024_bz4x_awd_xle`
- **Battery Sensor:** `sensor.ev_battery_level_2024_bz4x_awd_xle`
- **Tire Pressure Sensors:** 
  - `sensor.front_driver_tire_2024_bz4x_awd_xle`
  - `sensor.front_passenger_tire_2024_bz4x_awd_xle`
  - `sensor.rear_driver_tire_2024_bz4x_awd_xle`
  - `sensor.rear_passenger_tire_2024_bz4x_awd_xle`
- **Remote Start Script:** `script.start_bz4x`
