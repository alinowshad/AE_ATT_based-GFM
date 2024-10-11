## Autoencoder Attention-based Global Forecasting Model
#### Abstract:
In several industries, such as retail, tourism, and energy, vast amounts of time series data are generated. Global forecasting models (GFMs) have been successfully employed to train a single model by exploiting a set of time series. However, the performance of global models might diminish when confronted with heterogeneous time series datasets of varying lengths. This study proposes an autoencoder-based clustering approach that initially identifies clusters of homogeneous time series and subsequently trains a separate GFM for each cluster, leveraging the similarities across time series. The proposed autoencoders for time series featurization are designed by combining Long Short-Term Memory (LSTM), convolutional neural network (CNN), and attention mechanisms, with a masking layer incorporated to handle variable lengths in time series. Attention mechanisms facilitate the identification of the most significant features within the input by dynamically weighing the importance of different temporal features. To evaluate the forecasting accuracy of the proposed approach, extensive experiments are conducted across five time series datasets. The results demonstrate the superior performance of the proposed models compared to benchmark models across most datasets in terms of performance measures. Specifically, the autoencoder-based models consistently outperform several benchmark models, including univariate models as well as deep learning benchmarks such as DeepAR and N-BEATS techniques, and some clustering-based models in the existing literature with forecasting approaches similar to ours.

#### Methodology
The figure outlines the overall method for performing global forecasting, which involves six key steps, as shown in the graphic: 1) using time series datasets to train the designed autoencoders, 2) leveraging the autoencoders to extract features from the time series, 3) clustering the time series based on the extracted feature vectors, 4) preprocessing the time series to build forecasting models, 5) applying the created models to fit the global forecasting models and generate predictions for each time series, and 6) post-processing the forecasts. A detailed explanation of each step follows below.
![Framework](https://github.com/user-attachments/assets/2428dcf4-1919-4091-8884-741df92c6518)

### Installing Dependencies

To install all the dependencies required for this project, ensure you have `pip` installed. Then, run the following command to install the packages listed in `requirements.txt`:

```bash
pip install -r requirements.txt
