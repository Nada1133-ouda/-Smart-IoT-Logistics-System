# Smart IoT Logistics & Warehouse Management System 

An autonomous, data-driven warehouse management and cargo loading system built to eliminate inefficiency, reduce human error, and optimize truck capacity in real-time.

# The Problem & Solution
In traditional logistics, trucks are often under-utilized or loaded inefficiently, leaving critical shipments behind due to manual sorting. 
This system automates the loading dock using an IoT approach. When a truck gets within 10cm of the dock, the system triggers an autonomous optimization loop.

# Core Logic & Features
Cargo Management UI:A built-in interface to input and manage new cargo data directly into the database.
Dynamic Optimization: The Java backend queries the SQLite database and uses a (Priority Queue) to sort cargo by weight and priority.
Capacity Utilization: It algorithmically packs the truck to its maximum capacity, skipping heavy items if needed and selecting smaller items to fill remaining gaps.
Real-time Persistence: Updates shipment status to SHIPPED in the database the exact millisecond it's loaded.

Tech Stack
Backend:Java (OOP, Multi-threading).
Data Structures: Priority Queue Optimization.
IoT Components: ESP32, Ultrasonic Distance Sensor, Servo Motor (Simulated on Wokwi).
Connectivity: MQTT Protocol (via HiveMQ Cloud Broker).
Database: SQLite.
