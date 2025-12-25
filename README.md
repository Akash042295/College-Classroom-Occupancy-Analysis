# College Classroom Occupancy Analysis

## Overview
This project is a Python-based data analysis tool designed to evaluate the efficiency of classroom usage in educational institutions. By analyzing the relationship between **Room Capacity** and **Total Enrolled Students**, the script calculates a "Utilization Percentage" to identify inefficiencies.

This tool helps administrators identify:
* **Underutilized Rooms:** Large rooms used for small classes (wasted space).
* **Overcrowded Rooms:** Classes that exceed room capacity.
* **Optimization Opportunities:** Data-driven insights for rescheduling and room allocation.

## Features
* **Data Structure:** Utilizes a structured DataFrame to manage Room IDs, Capacities, Courses, and Time Slots.
* **Automated Calculation:** Automatically computes the `Utilization %` for every scheduled class.
* **Visual Analysis:** Generates a Bar Chart using `Matplotlib` to visualize occupancy rates across different rooms.
* **Group Analysis:** Uses Pandas `groupby` to handle multiple classes per room (scalable for larger datasets).

## Technologies Used
* **Python 3.x**
* **Pandas** (Data manipulation and analysis)
* **Matplotlib** (Data visualization)
* **NumPy** (Numerical operations)

## Analysis Logic
The core metric for this analysis is the **Utilization Rate**, calculated as:

Utilization = {Total Students / Capacity} * 100

* **Utilization < 50%:** Indicates the room is too large for the class (Inefficient).
* **Utilization > 100%:** Indicates the room is overcrowded (Safety hazard).

## Installation & Usage

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Akash042295/classroom-occupancy-analysis.git](https://github.com/Akash04295/classroom-occupancy-analysis.git)
    ```

2.  **Install dependencies:**
    Ensure you have Python installed, then run:
    ```bash
    pip install pandas matplotlib numpy
    ```

3.  **Run the script:**
    ```bash
    python analysis.py
    ```

## Sample Output
The script generates a DataFrame showing the calculated utilization:
*(Note: The script also produces a bar chart window displaying these statistics visually.)*

## Future Improvements
* Import data directly from CSV/Excel files instead of hardcoding.
* Add a "Time Slot" heatmap to see when the building is busiest.
* Export the optimization report to PDF.
