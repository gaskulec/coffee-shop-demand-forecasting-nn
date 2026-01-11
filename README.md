# coffee-shop-demand-forecasting-nn
# Coffee shop demand forecasting (neural network)

## Business Problem
[cite_start]Coffee shop management faces high variability in customer traffic due to weather, day of the week, and local events[cite: 3]. Inefficient resource management leads to:
* [cite_start]**Unnecessary labor costs** during slow periods[cite: 5].
* [cite_start]**Decreased service quality** during unexpected rushes[cite: 6].
* [cite_start]**Food waste** due to inaccurate daily production estimates[cite: 7, 45].

[cite_start]**Solution:** A regression Neural Network model that predicts the daily number of transactions to optimize staffing and inventory[cite: 8, 9].

## Technical Implementation
[cite_start]The model is built using a **Sequential Neural Network** architecture:
* [cite_start]**Input Layer:** Accepts 6 parameters including Temperature, Precipitation, Local Events, and short-term sales trends[cite: 11, 16, 17].
* [cite_start]**Hidden Layers:** Two dense layers (32 and 16 neurons) with **ReLU** activation to capture non-linear relationships.
* [cite_start]**Output Layer:** Single numerical value representing predicted daily customers[cite: 19, 29].
* [cite_start]**Optimization:** Trained using the **Adam** optimizer and Mean Squared Error (**MSE**) loss function over 100 epochs[cite: 29, 31].

## Model Performance
* [cite_start]The model was trained on 12 months of historical Point-of-Sale (POS) data[cite: 22].
* [cite_start]**Learning Process:** The training curve shows a consistent decrease in loss, indicating the model successfully learned traffic patterns related to weather and events[cite: 32, 33].
* [cite_start]**Practical Application:** The system automatically generates an **Operational Schedule**, suggesting "Standard" or "Reinforced" staffing based on the forecast[cite: 34, 37].

## Project Structure
* [cite_start]`demand_forecast_model.ipynb` - Python notebook containing the data preprocessing, NN architecture, and training.
* [cite_start]`operational_schedule_output.png` - Example of the automated weekly staffing recommendation[cite: 34].
* [cite_start]`training_loss_plot.png` - Visualization of the model's learning progress[cite: 30].

## Key Business Insights
* [cite_start]**Cost Optimization:** Prevents overstaffing on low-traffic days[cite: 44].
* [cite_start]**Waste Reduction:** Aligns food production with predicted demand[cite: 45].
* [cite_start]**Improved Service:** Ensures sufficient staffing during local events or favorable weather, reducing customer wait times[cite: 42, 46].
