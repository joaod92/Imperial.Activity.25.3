# LSTM Neural network and bayesian optimisation of an industrial temperature sensor

## NON-TECHNICAL EXPLANATION OF YOUR PROJECT
**100 words to explain what your project is about to a general audience.** 

My project revolves around optimizing a predictive model tailored for an industrial scenario, specifically utilizing data from a PT100 resistance temperature sensor. Employing advanced machine learning techniques and Bayesian optimization, I fine-tune the model's parameters for enhanced accuracy in time series analysis. This tailored approach ensures robust performance across diverse industrial conditions, making it a valuable tool for predicting future outcomes. The project's focus on an industrial setting, particularly involving PT100 sensors, aims to contribute to the development of reliable predictive models with applications in industrial processes, providing valuable insights for decision-making and efficiency improvements.


## DATA
**A summary of the data you’re using, remembering to include where you got it and any relevant citations.**

The data used was taken from Kaggle 'https://www.kaggle.com/datasets/arashnic/sensor-fault-detection-data' and it concerns sensor fault detection data in an industrial facility. In this data, a temperature senosr of PT100 resistance type was used and the the temperature readings it took were recorded over time. 

## MODEL 
**A summary of the model you’re using and why you chose it.** 

The model employed in this project is a Long Short-Term Memory (LSTM) neural network, specifically designed for time series prediction. LSTM networks excel at capturing sequential patterns and long-term dependencies, making them well-suited for analyzing temporal data. The choice of LSTM is motivated by its ability to effectively handle the intricate dynamics inherent in time series datasets, which is crucial for tasks such as predicting sensor readings. The model's architecture, featuring LSTM layers followed by a dense layer, facilitates learning intricate patterns within the industrial data. This selection aligns with the project's goal of optimizing predictive performance in an industrial context, specifically utilizing data from PT100 resistance temperature sensors.


## HYPERPARAMETER OPTIMSATION
**Description of which hyperparameters you have and how you chose to optimise them.** 

In the project, the key hyperparameters include:

Learning Rate: Controlling the step size during optimization.
Number of LSTM Units: Determining the memory capacity of the LSTM layer.
Number of Epochs: Defining the number of complete passes through the entire training dataset.
Batch Size: Specifying the number of samples processed in each training iteration.
To optimize these hyperparameters, Bayesian optimization was employed. Bayesian optimization is a probabilistic model-based approach that explores the hyperparameter space intelligently, considering both exploration and exploitation. This method efficiently balances the trade-off between exploring new hyperparameter configurations and exploiting known configurations, leading to the discovery of optimal settings for enhanced model performance.


## RESULTS
**A summary of your results and what you can learn from your model** 

The model, trained on industrial data from a PT100 resistance temperature sensor, was optimized using Bayesian optimization. The best hyperparameters were found to be a learning rate of 2.492235483180375e-05, 104 LSTM units, 5 epochs, and a batch size of 50. The final model exhibited improved performance compared to initial configurations, with a mean squared error of 30.429 on the test set. The results suggest the model's ability to capture patterns in the temperature sensor data, offering a promising approach for predicting sensor values in an industrial setting. Continued refinement and evaluation on diverse datasets could further enhance its robustness and generalizability.



