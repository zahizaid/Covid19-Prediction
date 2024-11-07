COVID-19 Daily Case Prediction in Malaysia Using LSTM

Overview 

This project aims to predict daily COVID-19 cases in Malaysia using a Long Short-Term Memory (LSTM) neural network. Due to the absence of AI-assisted systems during the initial outbreak of COVID-19, this deep learning model was proposed to assist in making data-driven decisions, such as imposing or lifting travel bans based on predicted cases. By training on past case data, this model forecasts new cases for the upcoming days, enabling better pandemic response planning.

Project Goal 

To create an LSTM-based deep learning model to predict COVID-19 cases in Malaysia using the last 30 days of cases data. The model meets the following specifications:

The architecture includes only LSTM, Dense, and Dropout layers. LSTM nodes are limited to 64, though the model depth is flexible. A window size of 30 days is used for predictions. Mean Absolute Percentage Error (MAPE) on the testing dataset is aimed to be less than 1%. Training progress is visualized using TensorBoard. Dataset The dataset includes daily COVID-19 cases reported in Malaysia, sourced from the Ministry of Health Malaysia’s official data repository (MoH Malaysia COVID-19 Public Data). The data used for training and testing can be found in the dataset folder of this repository.

Model Architecture

The model architecture consists of:

One or more LSTM layers, each with up to 64 nodes. Dropout layers to prevent overfitting. Dense layers to produce final output predictions.

Requirements 

The project requires the following Python libraries:

TensorFlow: For building and training the neural network 

Pandas and NumPy: For data manipulation 

Matplotlib: For plotting and visualizations 

TensorBoard: For tracking training progress Install the dependencies using:

Model Training: The model uses a 30-day sliding window of past cases as input to predict the next day’s case count. 

Training is done on the provided dataset, with MAPE set as the primary metric.

Loss Tracking: The training loss is visualized using TensorBoard, providing insight into the model’s convergence. 

MAPE Target: The model aims for a MAPE below 1% on the testing dataset.

Results Predicted vs. Actual COVID-19 Cases The plot below shows the predicted and actual cases, demonstrating the model's performance.

Model Performance MAPE: The model achieved a MAPE of less than 1% on the testing dataset, meeting the project’s accuracy criteria. 

Training Loss: The model’s training loss declined steadily, as shown in the TensorBoard plot.

Credits Data Source: Ministry of Health Malaysia COVID-19 Public Data

Model Architecture:

<img width="662" alt="Model_architecture" src="https://github.com/user-attachments/assets/8a2e8be7-980f-412e-87ce-81f8f7af3380">
<img width="281" alt="Model_architecture1" src="https://github.com/user-attachments/assets/21305dde-cb01-49f0-99ba-22c13d69c831">

Results:

<img width="591" alt="Prediction_graph" src="https://github.com/user-attachments/assets/6ed8ec5b-d6b7-422e-81e1-e05d177cefaf">
