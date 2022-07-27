# Telco-Customer-Churn-Prediction
Telecom Customer Churn Prediction using Supervised Machine Learning Algorithms


## Introduction

Churn is the measure of how many customers stop using a product. This can be measured based on actual usage or failure to renew (when the product is sold using a subscription model). Often evaluated for a specific period of time, there can be a monthly, quarterly, or annual churn rate.


When new customers begin buying and/or using a product, each new user contributes to a product’s growth rate. Inevitably some of those customers will eventually discontinue their usage or cancel their subscription; either because they switched to a competitor or alternative solution, no longer need to product’s functions, they’re unhappy with their user experience, or they can no longer afford or justify the cost. The customers that stop using/paying are the “churn” for a given period of time.


This dataset is available on Kaggle:https://www.kaggle.com/datasets/blastchar/telco-customer-churn


Our goal here is
* to predict which customer is going to churn with various classification supervised machine learning algorithms
* to evaluate which algorithms perform the best, so they can be used for further prediction on the upcoming data.

## Evaluation

There are four different supervised machine learning algorithms that have been used to predict the customer churn, which are: Logistic Regression, Decision Tree, Random Forest, and K-Nearest Neighbour. Random Forest and KNN have the highest accuracy score, with 81.62% and 77.82& respectively. Here are our observation for each algorithm:


* Logistic Regression: model ini merupakan model yang paling fit antara hasil dari data training dan data testing, dengan masing-masing memberikan akurasi 77.22% dan 77.11%. Artinya model ini merupakan model yang paling sederhana dibandingkan yang lain sehingga mempunyai akurasi paling rendah saat training, namun juga yang paling konsisten.


* Decision Tree: model ini memberikan akurasi paling tinggi pada data training, mencapai 99%. Artinya model yang dipapai sangat cocok dan akurat memprediksi target pada data training. Namun pada data testing, akurasi turun menjadi 80%, lebih rendah dibandingkan Random Forest dan K-Nearest Neighbor. Sedikit overfitting, namun pada nilai yang masih dapat diterima.


* Random Forest: secara teori, model ini merupakan pengembangan dari Decision Tree. Akurasi pada data training memberikan hasil yang sama seperti Decision Tree, yaitu 99%. Cukup kompleks untuk mengikuti pola target. Pada data testing, akurasi turun menjadi 85%, lebih tingi dibandingkan Decision Tree yang artinya berhasil mengurangi noise tanpa mengurangi kompleksitas model. Random Forest juga memberikan nilai akurasi yang paling baik, menjadikan model yang layak digunakan selanjutnya pada dataset ini dibandingkan model lain. Random Forest memberikan hasil yang baik disebabkan model ini dapat mempertimbangkan seluruh feature yang paling berpengaruh terhadap Churn pada root, sehingga hasil yang diperoleh lebih baik dari Decision Tree.


* K-Nearest Neighbor: model ini melibatkan perhitungan jarak, sehingga menghabiskan waktu pemodelan paling lama. Akurasi pada data training memberikan hasil yang impresif, yaitu 99% sedikit di bawah Decision Tree dan Random Forest. Pada data testing, akurasi yang dihasilkan adalah 82%, di atas Decision Tree. Artinya waktu pemodelan yang lama dan model yang lebih sederhana dibandingkan yang lain namun memberikan hasil yang cukup akurat dan bisa diandalkan. Bersama Random Forest, model KNN bisa digunakan selanjutnya pada dataset ini.  


Based in the evaluation, we can use Random Forest algorithm to predict the customer churn for the upcoming dataset!
