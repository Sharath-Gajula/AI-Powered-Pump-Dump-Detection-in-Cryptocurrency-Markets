# AI-Powered-Pump-Dump-Detection-in-Cryptocurrency-Markets

# Problem Statement
In the highly volatile cryptocurrency market, pump-and-dump schemes occur when prices are artificially inflated and then quickly deflated, leading to significant losses for investors. These manipulative practices are difficult to detect in real time due to the decentralized and unregulated nature of crypto markets. Traditional methods often fall short in identifying the subtle yet rapid shifts in price and volume that signal these fraudulent activities, especially when analyzing multiple cryptocurrencies simultaneously.

# Solution
To address this challenge, our project employs machine learning-based anomaly detection to accurately identify potential pump-and-dump events. The approach involves collecting historical price and volume data from sources like Binance, CoinGecko, and Kaggle, followed by preprocessing the data to handle missing values and standardize timestamps. We engineer key features such as Price Surge Ratio, Volume Surge Ratio, Relative Strength Index, moving averages, and Bollinger Bands to capture essential market dynamics. By applying an Isolation Forest model across multiple cryptocurrency datasets, anomalies are detected effectively and evaluated using metrics like precision, recall, F1-score, and ROC AUC. Visualizations such as confusion matrices and ROC curves further assist in comparing model performance, resulting in a robust, scalable solution that enhances market transparency and protects investors.

#Tools 
  Python
  Pandas & NumPy
  Scikit-learn
  TensorFlow / Keras
  PyTorch
  Jupyter Notebook
  Git / GitHub
  Matplotlib / Seaborn

#Methodology
  1. Data Collection
  •	Sources: Data is collected from cryptocurrency exchanges including Binance and CoinGecko.
  •	Preprocessing: The data is cleaned by handling missing values and standardizing timestamps to ensure consistency.
  2. Feature Engineering
  •	Surge Ratios: Calculate Price and Volume Surge Ratios to capture abrupt market movements.
  •	Trend Analysis: Compute moving averages to highlight trends over time.
  •	Technical Indicators: Derive the RSI and other relevant technical metrics to enhance the feature set.
  3. Anomaly Detection Models
  •	Isolation Forest: Utilizes a tree-based approach to effectively detect rare anomalies.
  •	DBSCAN: A density-based clustering algorithm that identifies anomalies by grouping data points with similar characteristics.
  •	Autoencoders: Neural network models that learn complex patterns and are used for detecting subtle anomalies in the data.
  4. Model Evaluation
  •	Metrics: Evaluate model performance using Precision, Recall, F1 Score, and ROC AUC Score.
  •	Visualization: Employ confusion matrices and ROC curves to visualize the trade-offs between true positives and false positives, and to compare the models' effectiveness.
  Model Comparison
  •	Isolation Forest: Proves effective in isolating rare anomalous events through its tree-based structure.
  •	DBSCAN: Offers competitive performance with density-based clustering, though it requires careful parameter tuning.
  •	Autoencoders: Excel in learning intricate data patterns but necessitate a well-curated set of normal data for training.
