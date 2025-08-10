# Oglaf's Home Assistant Configuration 🏠

Welcome to my Home Assistant configuration repository! This setup is built with three core principles in mind: **Convenience**, **Energy Savings**, and **100% Local Control**. Everything is designed to be automated, efficient, and reliable.

---

## ✨ Dashboards

I utilize several custom dashboards, each tailored for a specific purpose, from high-level server monitoring to detailed device control.

### Main Dashboard
The main dashboard gives a comprehensive overview of the house. Key sections include family member locations, weather forecasts, and quick toggles for the most-used devices in the Office, Kitchen, Living Room, and Bedroom. It's designed for quick access to essential controls and information.

![Main Dashboard](<image/2025-08-10 19_13_31-Home – Home Assistant and 19 more pages - Personal - Microsoft​ Edge.png>)

### Mobile Dashboard
Designed for on-the-go use, this dashboard is optimized for a mobile screen. It provides quick access to scenes, device controls, and status information for each room in a compact, scrollable format.

![Mobile Dashboard](<image/2025-08-10 19_17_35-Home Assistant and 18 more pages - Personal - Microsoft​ Edge.png>)

### Server & Network Dashboard
A technical dashboard dedicated to monitoring the health of my server and network infrastructure. It tracks WAN uptime, network speeds, and ping times to critical services like Cloudflare and Google. It also displays real-time CPU, RAM, and storage metrics for the main server and Hyper-V host.

![Server Dashboard](<image/2025-08-10 19_16_57-Server – Home Assistant and 18 more pages - Personal - Microsoft​ Edge.png>)

### Energy Dashboard
This dashboard is the heart of my energy-saving efforts. It provides a detailed breakdown of energy consumption and costs for individual appliances like the computer, washing machine, and various lights. A historical graph tracks usage over time, helping to identify opportunities for more savings.

![Energy Dashboard](<image/2025-08-10 19_14_22-Home – Home Assistant and 19 more pages - Personal - Microsoft​ Edge.png>)

### Vacuum Dashboard
A dedicated control center for my vacuum cleaner. It allows for starting routines, cleaning specific rooms, and monitoring the status of the battery and maintenance items like the filter, brushes, and sensors.

![Vacuum Dashboard](<image/2025-08-10 19_14_31-Vacuum – Home Assistant and 19 more pages - Personal - Microsoft​ Edge.png>)

### Lighting Dashboard
This dashboard provides centralized control over the lighting in the Living Room, Office, and Bedroom. It includes toggles for Adaptive Lighting, Sleep Mode, and Theater Mode, as well as a color wheel for precise lighting adjustments.

![Lighting Dashboard](<image/2025-08-10 19_14_10-Home – Home Assistant and 19 more pages - Personal - Microsoft​ Edge.png>)

---

## 🚀 Key Features & Automations

My configuration is packed with automations that make my home smarter and more efficient. Here are some highlights:

* **Adaptive Lighting:** Automatically adjusts the color temperature and brightness of lights throughout the day. The sunset offset is dynamically changed based on whether the sky is clear, ensuring the perfect lighting mood.
* **Automated Energy Tariffs:** The electricity tariff automatically switches between Peak, Shoulder, and Off-Peak rates throughout the day to accurately track energy costs.
* **Smart Office Environment:** The office lights turn on automatically at sunset if a computer is in use. When the last computer turns off, the lights and thermostat gracefully shut down.
* **Theater Mode:** When "Theater Mode" is activated, playing a movie automatically turns off the living room lights, and pausing the movie brings them back on for convenience.
* **Presence-Based Automation:** When everyone leaves the house, all lights and TVs are automatically turned off to save power.
* **Humidity Alerts:** The system compares indoor and outdoor humidity and sends a notification to open or close the windows to maintain the best indoor air quality.
* **Scheduled WoL:** My PC is automatically turned on via Wake-on-LAN on business days, ready for the workday.
* **Washing Machine Notifications:** I receive a notification on my phone as soon as the washing machine has finished its cycle.

---

## 🛠️ Software & Integrations

This setup relies on a curated list of powerful community integrations to enhance functionality.

### Key HACS Integrations
* **[Adaptive Lighting](https://github.com/basnijholt/adaptive-lighting):** The core of my smart lighting system, this component adjusts lights to mimic natural daylight.
* **[Tuya Local](https://github.com/make-all/tuya-local):** Enables direct, local control over my Tuya-based devices, avoiding the cloud.
* **[Powercalc](https://github.com/bramstroker/homeassistant-powercalc):** Provides accurate power consumption estimates for devices that don't have built-in power monitoring.
* **[Watchman](https://github.com/dummylabs/the-watchman):** A helpful tool that monitors my configuration files for missing entities and services, keeping my setup clean and error-free.

### Automation Blueprints
* **Advanced Medication Reminder:** A blueprint used for sending timely medication reminders to an Android device.
* **ZHA - Sonoff SNZB-01:** Blueprints that map single and double presses from Sonoff wireless switches to control lights and trigger scripts.