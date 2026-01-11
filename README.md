# Coffee shop demand forecasting (neural network)
## Why I built this
Working in a coffee shop, I quickly noticed how unpredictable the rush can be. Some days you’re overstaffed and bored, other days, you're overwhelmed and running out of products, time alongside with staff. I wanted to see if I could use data to move away from intuitive management to predicting how many customers would walk through the door in coming 7 days.

## How it works
A regression model was built in Python using TensorFlow. The goal was to take external factors and turn them into a headcount.

<center>
|Number| Input variable| Description|
|------|---------------|-------------|
| 1 |day of the week| numerical representation (0-6) of the weekday |
| 2 |weekend/holiday| binary flag (0 or 1) for non-working days |
| 3 |temperature| forecasted temperature in Celsius |
| 4 |precipitation | rain or snow presence (0 or 1) |
| 5 |local events| nearby concerts, matches, markets |
| 6 |sales trends| avg sales from the last 3 days, short-term trend |
</center>

The Sequential Neural Network has two hidden layers (32 and 16 neurons). I used ReLU activation to help the model catch the tricky non-linear patterns (like how a little rain might not matter, but a downpour definitely does). I ran the training for 100 epochs. You can see in the loss plots how the error drops off sharply as the model starts "getting it".

## Real-world impact
The best part isn't the code, it's the output. The model produces a clear 'Operational schedule' for the week.
- Smart staffing: It flags high-traffic days (like a busy Wednesday) so the manager knows to bring in a third person.
- Less waste: By knowing the guest count, we can prep exactly the right amount of food, which keeps costs down and reduces waste.
- Developed this one in Google Colab.

## Author: Gabriela Kozubal
