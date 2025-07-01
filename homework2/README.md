## Name: Caroline Jungheim

# Homework 2

## Task 1 – Multi-Model Plotting

In this task, the existing notebook `7_multi_model_plotting` was extended to:
- Automatically read the forecast results from all trained models.
- Plot the predicted and true temperature from different models in a single panel.
- Make the plotting functions reusable for different stations and time periods.

**What I did:**
- Adapted each notebook of the different models to save the forecasts
- Prepared the forecasts and created a function for plotting
- Plotted multiple models' results in one panel
- Ensured flexibility for plugging in new results without modifying the core code.

**What I learned:**
- Visualizing all models together made it easier to see differences in behavior.
- Some models performed significatly better than others

---

## Task 2 – Multivariate Input: Temperature + Ozone

In the second task, one of the models (e.g., MLP) was extended to accept **both past temperature and ozone** as inputs.

**What I did:**
- Loaded dataframe with the to variables
- Had to remove duplicated in the dataframe for further processing
- Adjusted model input layers and training code accordingly.
- Plotted the graph for better comparison of actual and prediction

**What I learned:**
- Multivariat models perform really good in this case.

---

## Task 3 – Using Forecasted Temperature

The final task simulated a realistic forecasting scenario where **future temperature** (from weather forecasts) is available at prediction time.

**What I did:**
- Extended the dataset to append future temperature data to the input features.
- Combined past (temp + o3) and future temp into one input block and adapted code to run the model.
- Compared results with Task 2 using the multi-model plotting function of task 1 (in a lightly updated format).

**What I learned:**
- Using future temperature further improved performance.

---

## Difficulties:
I needed a lot of time at the beginning to run all the models and save the corresponding forecasts for task 1. The reason for this was that it was not entirely clear to me at first and I sometimes had problems understanding where which files (rawdata, normalized data) were being used. It was also not always clear which parts of the code were really needed.
Another problem with tasks 2 and 3 was adapting the data records into the correct shapes. Sometimes I got quite confused about where to reshape and in which way. That cost me a lot of time.

## Additional Information:
In every notebook I marked the parts where I updated the code with an emoji 🦋 for better understanding



