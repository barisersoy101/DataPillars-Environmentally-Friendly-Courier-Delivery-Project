Datapillars Environmentally Friendly Courier Delivery Model

Project Overview

The Datapillars Environmentally Friendly Courier Delivery Model is a data-driven system designed to optimize courier assignments while minimizing environmental impact. The model balances speed, efficiency, and sustainability by selecting couriers based on their vehicle type, availability, and estimated delivery time.

Features

Courier Selection Optimization: Assigns couriers based on three criteria:

Fastest Bicycle Courier (not affected by traffic)

Least Environmental Impact Courier (prioritizing eco-friendly vehicles)

Fastest Courier (without environmental considerations)

Traffic-Aware Delivery Time Calculation

Environmental Impact Assessment: Includes CO2 emissions based on vehicle type and traffic delays.

Geospatial Visualization: Uses map-based visualizations to analyze courier distribution and city zones.

System Requirements

Programming Language: Python 3.11.9

Datasets Used:

all_waybill_info_meituan.csv

2021_Cars_Aggregated.csv

Memory Requirements:

600MB RAM per courier model

4.8GB RAM for an 8-day training period

8-hour training time for 100,000 orders with 20,000 couriers

Data Overview

The model utilizes multiple datasets:

Courier Availability (courier_availability DataFrame): Contains information about couriers' working hours, locations, and vehicle types.

Order Data (orders_df): Includes order IDs, pickup and drop-off coordinates, and timestamps.

City Zones (city_zones_df): Defines urban, suburban, and rural zones based on geospatial clustering.

Car Emissions Data (cars_aggregated_df): Maps vehicle types to CO2 emissions.

How It Works

Preprocessing: Data is cleaned and formatted, ensuring all couriers and orders are mapped correctly.

Courier Assignment:

Orders are matched with couriers based on availability, location, and vehicle type.

Different optimization objectives are used to assign couriers based on speed and environmental impact.

Impact Calculation:

Traffic conditions affect estimated delivery times.

Emissions are calculated based on vehicle usage and time on the road.

Visualization:

City zones, courier locations, and delivery paths are plotted for analysis.

Installation & Usage

Install required Python libraries:

pip install pandas numpy matplotlib scikit-learn folium

Run the Jupyter Notebook (Datapillars Environmentally Friendly Courier Delivery Model.ipynb).

Load datasets into the model.

Execute the courier assignment and environmental impact calculations.

Visualize results on maps.

Future Improvements

Integrating real-time traffic data

Enhancing machine learning models for delivery time prediction

Expanding dataset coverage for better optimization

Contributors

Datapillars Team from Seminar: AI Implementation

Otto von Guericke University Magdeburg

License

This project is licensed under the MIT License.
