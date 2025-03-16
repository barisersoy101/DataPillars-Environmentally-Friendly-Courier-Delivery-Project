# Datapillars Environmentally Friendly Courier Delivery Model

## Overview

This project, developed by the DataPillars team from Otto von Guericke University, focuses on analyzing and optimizing courier delivery data with an emphasis on environmental sustainability. It was created as part of the course **Seminar: AI Implementation**. The project processes datasets related to courier operations, vehicle emissions, and delivery timings to identify insights that can help reduce environmental impact and improve operational efficiency.

## Model Description

The model is designed to optimize courier assignments based on environmental impact and efficiency. Two types of models are used:

1. **Fastest Car Model**: Prioritizes the fastest delivery time for couriers. 
2. **Environmentally Friendly Model**: Prioritizes minimizing environmental impact by considering CO2 emissions and fuel consumption data.

### System Requirements

- **Python Version**: 3.11.9
  > Note: The 'append' method is deprecated in future Python versions. For newer versions, use the 'concat' method to add final data to a DataFrame.
- **Execution Environment**: The model was trained using Jupyter Notebooks but can also run as a standalone `.py` file without modifications.

### Memory and CPU Requirements

- **Single Courier Training**: 600 MB of RAM is required per model.
- **Multiprocessing**: The model processes data per day for the available dates in the data. For 8 days, 4.8 GB of RAM is recommended.
- **CPU**: 8 GB of CPU is recommended for running both models in parallel for 8 days of data.

### Training Time

Training both models for 100,000 orders and 20,000 couriers with an average of 4 days (8 hours of availability) will take:

- **8 hours per model**
- **16 hours in total**

> The current code is optimized to train with 100 orders and around 20,000 couriers for faster execution during tests.

## Installation
You can try it below, I think it will work, but it takes so long time for the model to work. Therefore, I advise you to try it in Jupyter Notebooks with less data. 
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/environmentally-friendly-courier-model.git
   cd environmentally-friendly-courier-model
   ```
2. Install required packages:
   ```bash
   pip install pandas numpy datetime psutil
   ```

## Usage

1. Place your data files in the specified directory paths or update the paths in the notebook accordingly.
2. Alternatively, you can access similar Meituan datasets available online to replicate and try the project.
3. Run the notebook in a suitable Python environment (e.g., Jupyter Notebook).
4. Follow the code cells sequentially to process and analyze the data.

> **Note for Data Loading**: The data loading code is located in the second cell of the notebook. Update the paths as necessary.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or suggestions.

## Contact

For any inquiries or support, please contact [[your-email@example.com](mailto:your-email@example.com)].
