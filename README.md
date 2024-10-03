# Banknote Authentication

### Scenario
You are a shop owner, and you do not want to lose money getting fake banknotes. However, you do not have enough budget for an advanced instrument that verifies banknotes directly through images, which is probably fast and accurate. The only instrument you can use is an old black-box like machine. This old black box contains an industrial camera taking low-resoulution grey-scale images. The machine will output a rough analysis on the grey-scale images after the camera takes image of a banknote, providing some numerical values about banknote imaging features. Exploiting the numerical values of the banknote grey-scale imaging features, you want to make this old black-box like machine to work as a true-or-fake banknote exminator.

### Data
Data can be downloaded from https://archive.ics.uci.edu/dataset/267/banknote+authentication

### Methods and results
[Logistic regression](https://github.com/danicychao/banknote_authentication/blob/main/banknote_logistic.ipynb): we are a bit more lucky that we have a sample of verified banknotes, which enable us to train this machine as a logistic regression model. Our trained logistic regression model have **98% accuracy** in verifying banknotes - with the machine, we can verify almost all the fake banknotes and do not mis-verify true banknote as fake ones. **Your shop will get more five-star reviews without the risk of losing money!**

[K-Means clustering](https://github.com/danicychao/banknote_authentication/blob/main/banknote_clustering.ipynb): we do not even have budget to get a sample of verified banknotes. We try to train this machine as an unsupervised K-Means clustering model. Our trained K-Means clustering model is stable. If we keep running the business with this K-Means model machine for a while, we will find out our trained K-Means clustering model achieves **86% accuracy** when we go to the bank to save the received banknotes. It is not as good as logistic regression, but it is not terrible at all.
