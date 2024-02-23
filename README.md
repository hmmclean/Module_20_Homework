# Module_20_Homework
Module 20 - Supervised Machine Learning

# Overview
This dataset delves into the price change percentage in cryptocurrency across various time frames, spanning from as brief as 24 hours to as extensive as 1 year. Employing standard scalar normalization facilitates a unified scale for comprehensive data evaluation. Leveraging the Kmeans model enables us to pinpoint the optimal clustering solution for the data. Subsequently, the Principal Component Analysis (PCA) was performed using three key features, followed by the application of a Kmeans model to contrast using all available features versus scaling down to fewer features using the PCA.

# Navigation
* Resources 
    * crypto_market_data - provided csv dataset.
    * Pictures
         * elbow_plots - png of scatter plot comparison.
         * scatter_plots - png of scatter plot comparison.
* Crypto_Clustering - provided jupyter notebook file that contains the code. 

# Analysis
After executing the principal component analysis with three features, approximately 88% of the variance within the dataset was successfully accounted for. Both the scaled normalized data and the PCA-transformed data demonstrated optimal performance with the application of a 4-cluster Kmeans model.

<p align="center">
<img src="https://github.com/hmmclean/Module_19_Homework/blob/main/Resources/Pictures/elbow_plots.PNG" width="1050">
</p>


Using fewer features seemed to create tighter clusters, suggesting a reduction of noise or a focusing of predicted patterns. Overall, the PCA analysis is similar to the original normalized data, leading to an accurate representation of the data but with fewer principle components.


<p align="center">
<img src="https://github.com/hmmclean/Module_19_Homework/blob/main/Resources/Pictures/scatter_plots.PNG" width="1050">
</p>

# References and Resources
* ChatGPT - https://chat.openai.com/
* Scikit-learn - https://scikit-learn.org/
