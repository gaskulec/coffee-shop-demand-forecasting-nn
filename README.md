# Coffee shop demand forecasting (neural network)
## Why I built this
Working in a coffee shop, you quickly notice how unpredictable the rush can be. Some days you’re overstaffed and bored; other days, you're overwhelmed and running out of sandwiches. I wanted to see if I could use data to move away from "gut feeling" management and actually predict how many people would walk through the door.

## How it works
I built a regression model in Python using TensorFlow. The goal was to take external factors and turn them into a headcount.

- The Data: I fed the model 6 main variables: the day of the week, weather (temp/rain), whether there was a local event (like a concert), and recent sales trends.
- The Brain: I went with a Sequential Neural Network with two hidden layers (32 and 16 neurons). I used ReLU activation to help the model catch those tricky non-linear patterns—like how a little rain might not matter, but a downpour definitely does.
- Training: I ran the training for 100 epochs. You can see in the loss plots how the error drops off sharply as the model starts "getting it".

## Real-world impact
The best part isn't the code, it's the output. The model produces a clear Operational Schedule for the week.
- Smart Staffing: It flags high-traffic days (like a busy Wednesday) so the manager knows to bring in a third person.
- Less Waste: By knowing the guest count, we can prep exactly the right amount of food, which keeps costs down and reduces waste.
- Developed this one in Google Colab to keep the training fast and efficient.

- # Author: Gabriela Kozubal
