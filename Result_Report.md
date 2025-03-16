# Result Report: Datapillars Environmentally Friendly Courier Delivery Model

## Overview
This report presents the outcomes of the courier assignment models developed by the DataPillars team at Otto von Guericke University for the course **Seminar: AI Implementation**. The models aim to optimize courier assignments for both speed and environmental sustainability.

## What the Model Does
The project developed two distinct models for courier assignment:

1. **Fastest Vehicle Model**: Optimizes for speed by selecting couriers with the fastest delivery potential, often utilizing cars for longer distances.
2. **Environmentally Friendly Model**: Optimizes for minimal environmental impact by preferring bicycle couriers for shorter distances and assigning low-emission vehicles where feasible.

## Preprocessing Functions
- **Data Conversion**: Unix timestamps were converted to datetime formats for accurate processing.
- **Data Cleaning**: Invalid or default timestamp entries were removed. Time columns were adjusted to ensure realistic working hours.
- **Courier Type Assignment**: Couriers were categorized based on vehicle types (bicycles or cars). For cars, environmental impact data (CO2 emissions) was mapped.
- **City Zoning**: The geographical data was divided into zones (Center, Nearby, Far) based on delivery density.
- **Traffic Adjustment**: Traffic factors were applied dynamically based on zone proximity and time of day to simulate realistic delays.

## Training Process and Learnings
- **Initial Phases**: Training began with a small dataset, but scaling issues led to long-distance assignments.
- **Improvements**: Increasing courier counts, focusing on central city zones, and filtering out impractical orders (>10 km distance) resulted in better outcomes.
- **Key Learning**: The balance between courier numbers and geographical distribution is crucial for efficient operations.

## Results
### Order Assignments
- Both models processed 100,000 orders, successfully assigning 91,647 in each case.

### Delivery Time Efficiency
- **Fastest Vehicle Model**: Total delivery time was 6,227.94 hours, averaging 30 minutes per order.
- **Environmentally Friendly Model**: Total delivery time was 15,887.09 hours, averaging 33 minutes per order—a 3-minute increase for enhanced sustainability.

### Environmental Impact
- **Fastest Vehicle Model**: Generated 21,333,785.83 kg of CO2 emissions.
- **Environmentally Friendly Model**: Reduced emissions significantly to 2,163,834.44 kg—a reduction of approximately 19 million kg.

### Courier Utilization
- **Environmentally Friendly Model**: Managed 91,647 orders using 9,846 couriers, with 81,621 deliveries by bicycle.
- **Fastest Vehicle Model**: Utilized 16,119 couriers, but only 730 were bicycle-based, prioritizing speed over environmental considerations.

## Conclusion
The Environmentally Friendly Model demonstrates that minor increases in delivery time (about 3-6 minutes per order) can lead to substantial reductions in environmental impact. The approach proves effective for sustainable urban logistics, offering an adaptable and scalable solution for eco-conscious delivery operations.
