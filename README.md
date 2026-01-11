# Coffee shop demand forecasting (neural network)
## Why I built this
Working in a coffee shop, I quickly noticed how unpredictable the rush can be. Some days you’re overstaffed and bored, other days, you're overwhelmed and running out of products, time alongside with staff. I wanted to see if I could use data to move away from intuitive management to predicting how many customers would walk through the door in coming 7 days.

## How it works
A regression model was built in Python using TensorFlow. The goal was to take external factors and turn them into a headcount.
|The data; the model was fed with 6 main variables|
| 1 |the day of the week|
| 2 |whether it’s a weekend or holiday|
| 3 |the temperature|
| 4 |precipitation (rain/snow)|
| 5 |any local events happening nearby|
| 6 |the average sales from the last 3 days to catch short-term trends|
The Sequential Neural Network has two hidden layers (32 and 16 neurons). I used ReLU activation to help the model catch the tricky non-linear patterns (like how a little rain might not matter, but a downpour definitely does). I ran the training for 100 epochs. You can see in the loss plots how the error drops off sharply as the model starts "getting it".

## Real-world impact
The best part isn't the code, it's the output. The model produces a clear 'Operational Schedule' for the week.
- Smart Staffing: It flags high-traffic days (like a busy Wednesday) so the manager knows to bring in a third person.
- Less Waste: By knowing the guest count, we can prep exactly the right amount of food, which keeps costs down and reduces waste.
- Developed this one in Google Colab to keep the training fast and efficient.

- # Author: Gabriela Kozubal
