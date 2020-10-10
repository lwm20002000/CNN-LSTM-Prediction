# CNN-LSTM-Prediction
使用CNN-LSTM模型对天气数据进行分析，从而预测发病率。The CNN-LSTM model is used to analyze the weather data and predict the incidence rate.  
## 需求
- Tensorflow >= 1.8.0  
- Keras >= 2.1.6  
## 任务
进行发病人数的时间序列预测。可以选择使用BP/LSTM/CNN-LSTM算法。  
含有decomposed的文件是将要预测的标签序列进行信号分解后再进行预测。具体做法是，先根据信号分解得到8个标签，对每个标签分别进行预测，最后再进行求和操作。  
## 文件结构
- CNN_LSTM.ipynb：不对标签序列进行分解。  
- CNN_LSTM_decomposed_Aotu.ipynb：对标签序列进行分解后**自动**进行8次预测并求和，对比得到评估指标。  
- CNN_LSTM_decomposed_Manual.ipynb：对标签序列进行分解后**手动**进行8次预测并求和（手动效果可能更好），对比得到评估指标。  
