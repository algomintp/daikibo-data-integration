# Daikibo Telemetry Data Integration

## 📌 Overview

This project is part of the Deloitte Forage Job Simulation.
The objective is to standardize telemetry data coming from industrial IoT devices that use different data formats.

Two different JSON formats are transformed into a single unified structure to enable consistent data analysis.

---

## ⚙️ Problem Statement

Daikibo Industrials receives telemetry data from multiple devices in different formats.
This creates inconsistency and makes it difficult to process and analyze the data.

The goal is to:

* Convert multiple input formats into a unified format
* Ensure consistency in structure and data types
* Enable seamless downstream analytics

---

## 🧩 Solution Approach

The solution includes:

* Parsing input JSON data
* Transforming fields into a common schema
* Converting timestamps into milliseconds since epoch
* Structuring location and device data consistently

Two functions handle the transformation:

* `convertFromFormat1()` → Handles flat JSON structure
* `convertFromFormat2()` → Handles nested JSON structure and timestamp conversion

---

## 📂 Project Structure

```
├── main.py
├── data-1.json
├── data-2.json
├── data-result.json
```

---

## ▶️ How to Run

1. Make sure Python 3 is installed
2. Run the following command:

```
python main.py
```

3. Expected output:

```
OK
```

---

## 🧪 Testing

The project uses Python's built-in `unittest` module.

Test cases validate:

* Conversion from Format 1
* Conversion from Format 2
* Output matches expected unified format

---

## 🛠️ Technologies Used

* Python 3
* JSON
* datetime module
* unittest

---

## 🎯 Key Learnings

* Data transformation and normalization
* Handling multiple data formats
* Timestamp conversion (ISO → Epoch milliseconds)
* Writing testable and structured Python code

---

## 📌 Conclusion

This project demonstrates a simple but practical data engineering workflow, focusing on transforming heterogeneous data into a unified format for better usability and analysis.
