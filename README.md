Developed a deep learning-based stock price prediction system using PyTorch LSTM networks to forecast daily closing prices of Google stock.
•	Collected and analyzed 7 years of historical Google stock data (2018–2024) containing 1,761 trading records with Open, High, Low, Close, and Volume attributes.
•	Performed data preprocessing, including date parsing, missing value handling, dataset inspection, and statistical analysis.
•	Conducted Exploratory Data Analysis (EDA) by visualizing stock price trends and generating correlation heatmaps to understand feature relationships.
•	Selected the Closing Price as the target variable and created supervised learning sequences using a 60-day sliding window approach, where 60 consecutive closing prices were used to predict the 61st day's price.
•	Split the generated sequences into 80% training and 20% testing datasets, resulting in 1,360 training samples and 341 testing samples.
•	Applied Min-Max Normalization to scale the data and converted the processed datasets into PyTorch tensors for model training.
•	Implemented efficient batch processing using PyTorch DataLoader.
•	Designed and compared three LSTM architectures:
o	Simple LSTM: 1 LSTM layer, Hidden Size = 50
o	Medium LSTM: 2 LSTM layers, Hidden Size = 100, Dropout = 0.2
o	Complex LSTM: 3 LSTM layers, Hidden Size = 150, Dropout = 0.3
•	Used Mean Squared Error (MSE) Loss and the Adam Optimizer for model training.
•	Trained all models for 100 epochs utilizing Google Colab GPU acceleration to improve training efficiency.
•	Evaluated model performance by generating predictions on the test dataset and applying inverse scaling to restore original stock price values.
•	Visualized Actual vs Predicted Closing Prices to compare forecasting accuracy across all architectures.
•	Identified the Simple LSTM model as the best-performing architecture.
•	Implemented 10-day future stock price forecasting beyond the available dataset using recursive prediction techniques.
