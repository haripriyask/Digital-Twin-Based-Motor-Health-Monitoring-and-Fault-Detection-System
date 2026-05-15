# Digital-Twin-Based-Motor-Health-Monitoring-and-Fault-Detection-System
  A Digital Twin-based IoT system for real-time motor health monitoring using ESP32 and multi-sensor data. It integrates Random Forest and Digital Twin analysis to detect faults and provide real-time dashboards and automated alerts for predictive maintenance.

## Objectives

- To monitor motor condition in real time using IoT sensors  
- To detect faults early using machine learning techniques  
- To implement Digital Twin for deviation-based analysis  
- To provide automated alerts for abnormal conditions  
- To reduce downtime and maintenance cost

## System Architecture

The system follows a multi-layer architecture:

1. Sensing Layer – Collects temperature, vibration, sound, and current data  
2. Communication Layer – MQTT-based real-time data transmission  
3. Data Layer – Storage using InfluxDB (TIG Stack)  
4. Intelligence Layer – Random Forest + Digital Twin analysis  
5. Visualization Layer – Grafana and Power BI dashboards  
6. Alert Layer – n8n workflow with Twilio SMS notification


## Components Used

### Hardware
- ESP32 Microcontroller  
- MPU6050 (Vibration Sensor)  
- GY-906 (Temperature Sensor)  
- HW-484 (Sound Sensor)  
- SCT-013 (Current Sensor)  

### Software
- Arduino IDE  
- MQTT Protocol  
- Telegraf, InfluxDB, Grafana (TIG Stack)  
- Python (Random Forest Model)  
- Power BI (Analytics Dashboard)  
- n8n (Automation Tool)  
- Twilio (SMS Alert Service)

## Working Principle

- Sensors collect real-time motor data  
- ESP32 sends data via MQTT  
- Data stored in InfluxDB  
- Grafana & Power BI visualize data  
- Machine learning model predicts motor state  
- Digital Twin compares expected vs actual values  
- n8n triggers alerts when fault is detected

  ## System Outputs

- Real-time sensor data visualization  
- Motor state classification:
  - Normal  
  - Warning  
  - Fault  
  - Overheating  

- Grafana dashboard for live monitoring  
- Power BI dashboard for analytics  
- SMS alert notifications for faults

## Advantages

- Early fault detection  
- Real-time monitoring  
- Low-cost solution  
- High accuracy (>90%)  
- Automated alert system  
- Reduces maintenance cost

## Conclusion

The proposed system successfully implements a Digital Twin-based predictive maintenance framework for motor health monitoring. It improves reliability, reduces downtime, and enables proactive maintenance using IoT, machine learning, and automation technologies.
