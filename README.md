### Wireshark Data Analysis

This Python script analyzes Wireshark capture data stored in a JSON file and plots various graphs to visualize the data. It uses the PyShark library to process the JSON file and Matplotlib for plotting.

#### Requirements
- Python 3.x
- PyShark
- Matplotlib

#### Installation
1. Install Python 3.x from [Python's official website](https://www.python.org/downloads/).
2. Install PyShark and Matplotlib using pip:
   ```bash
   pip install pyshark matplotlib
   ```

#### Usage
1. Replace `"E:\sensio\\rawdata.json"` in the `file_path` variable with the path to your Wireshark JSON file.
2. Run the script to analyze and plot the data.

#### Features
1. **RSSI Graphs**:
   - Plots the Received Signal Strength Indicator (RSSI) over time for all packets.
   - Separately plots RSSI over time for empty packets, advertising packets, and data packets.

2. **Malformed Packets**:
   - Calculates and prints the percentage of malformed packets among all advertising packets.

#### Notes
- Ensure the JSON file contains the expected Wireshark capture data with the necessary fields (e.g., `frame.time_epoch`, `nordic_ble.rssi`, `btle.length`).
