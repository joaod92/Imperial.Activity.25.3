# Model Card

## Model Description

**Input:** The model takes as input sequences of historical temperature readings from a PT100 resistance temperature sensor. Each input sequence consists of a set of consecutive temperature values sampled over time.

**Output:** The model produces a single continuous value representing the predicted temperature for the next time step in the sequence.

**Model Architecture:** The chosen model architecture is a Long Short-Term Memory (LSTM) neural network. The LSTM model is well-suited for sequence prediction tasks, capturing temporal dependencies in the input data. The architecture includes an LSTM layer with a specified number of units, followed by a dense layer producing the output. The usage of this model was also recommended by the individual contributor on Kaggle that made the data available. 

## Performance

The model's performance is evaluated using Mean Squared Error (MSE) as the primary metric. During training, the dataset is split into training and validation sets, and the model's performance is monitored on the validation set. The final evaluation is done on a separate test set to assess generalization.

## Limitations

The model heavily relies on the characteristics of the PT100 sensor data. Any biases or anomalies present in the sensor readings may impact model predictions.
Limited diversity in the dataset might lead to challenges in generalizing to diverse industrial scenarios.

## Trade-offs

LSTM models' complexity leads to longer training times and more computation requirements - and the model's effectiveness may decrease if deployed in scenarios significantly different from the training data its been exposed to. 
Deep learning models like LSTMs often lack interpretability which can make it difficul to explain the rationale behind predictions. 

