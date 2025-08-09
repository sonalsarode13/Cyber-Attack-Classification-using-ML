# Cyber-Attack-Classification-using-ML

1.Algorithms
Data preprocessing involves loading data into pandas DataFrames for structured handling. Categorical variables such as protocol_type, service, and flag are encoded using LabelEncoder, transforming them into a suitable numeric format for the model. Concurrently, numeric features are scaled and normalized using MinMaxScaler, standardizing data ranges to improve model performance.
Model training utilizes a carefully designed Keras Sequential neural network architecture. This network is composed of multiple dense layers interleaved with Batch Normalization and Dropout layers to mitigate overfitting and enhance generalization. The network is compiled with the Adam optimizer, employing either categorical crossentropy loss for multi-class scenarios or binary crossentropy for binary classification problems. Models are systematically saved in JSON and H5 formats, alongside a unified .keras format, to facilitate easy deployment and future retraining.
Real-time detection procedures leverage the Scapy library to perform live packet capture from network interfaces. Each packet is converted into a standard feature vector, normalized using the pre-fitted scaler, and classified by the trained neural network model. Results from this analysis trigger alerts, initiate detailed 
logging procedures, and, if necessary, automated IP blocking to promptly mitigate threats.


2. Use Cases
The IDS is highly effective in real-time network monitoring, allowing rapid detection and immediate notification to network administrators, thus significantly reducing response times and potential damage. It also supports offline batch analysis, enabling thorough evaluation of network security measures and model performance assessment over historical data. Additionally, the system excels in generating comprehensive threat documentation and reporting, providing detailed insights into detected threats with extensive metadata, which includes IP addresses, geolocations, timestamps, and recommended actions, facilitating efficient incident response and future preventive strategies.

3.Conclusion
This Intrusion Detection System project effectively integrates robust machine learning algorithms, meticulous data preprocessing, and sophisticated real-time analysis to offer advanced network security solutions. Its structured architecture and comprehensive features ensure adaptability and sustained effectiveness in facing evolving cybersecurity threats, making it an essential tool for maintaining network integrity and security.
