# flags_and_religion

<h2>About</h2>
For this project, we used machine learning to 
explore the potential predicitability of a country's religion based on the design of their flag. We then summarized our project and outcomes on <a href="https://zpoeschl.github.io/flags_and_religion/">this website</a> which we encourage you to explore.
<br>
<br>
We used the <a
href="https://archive.ics.uci.edu/ml/datasets/Flags" target="_blank">
flags data set</a> available through the <a
href="https://archive.ics.uci.edu/ml" target="_blank">
UCI Machine Learning Repository</a>. This data set is not large, consisting
of only 194 instances (countries/flags) and 30 attributes (descriptors), making
the size of our experiments simultaneously manageable and limited.
<br>
<br>
To explore this data set and apply machine learning, we performed tests using a jupyter notebook. 
Within our notebook we used scikit-learn to test a neural network, the most successful of our tests, as well as 
a support-vector machine. Pandas and Matplotlib were also used to support the processing and visualization of 
our data.

## Summary
In this section, we wanted to provide further explanation into the various machine learning techniques that were used to test our data. Those machine learning techniques would be:

* Multiple Linear Regression
* K-Nearest Neighbors
* Suport Vector Machines
* Neural Network
* Deep Neural Network

Knowing that these are the classification models that we would be using, we will now need to:

1. Preprocess the Data
1. Train the Model
1. Test the Model
1. Make Improvements

### Preprocess the Data
This step will be covered alone and the rest of the steps will be address in the models below. Using the dataset about, we loaded this into Python Pandas. We then created our "X" & "y" values. The "X" values (independent values) will be all of the attributes used to define the flag and origin of those that represent it (i.e. landmass, population, bars, stripes, colors, etc.) and the dependent variable would be religion. The "y" value (dependent value) will be religion.

### Multiple Linear Regression

![Mulit-line-acc](https://user-images.githubusercontent.com/75814760/121753107-3cb1d980-cad7-11eb-9811-6b4e4783f481.jpg)

![mlt-lin-train-graph](https://user-images.githubusercontent.com/75814760/121753146-5b17d500-cad7-11eb-95cb-23e85bfccb4a.png)


![mlt-lin-test-graph](https://user-images.githubusercontent.com/75814760/121753138-53f0c700-cad7-11eb-8ce5-eafdd4bfa2b8.png)

![mlt-lin-r2](https://user-images.githubusercontent.com/75814760/121753162-64a13d00-cad7-11eb-9a47-8115e5788e2f.png)


### Improvements
After testing one machine learning technique with less than stellar results we looked to see if there were any improvements within the data that could be made.
The three areas we looked to improve on were by consolidating religion, adding population density and area by square miles for each country. Originally we used the
following 8 religions: 

![religion_screenshot](https://user-images.githubusercontent.com/75814760/121786415-46921600-cb85-11eb-9dd6-c543a5eca755.png)

### K-Nearest Neighbors

![KNN](https://user-images.githubusercontent.com/75968440/122225788-fcf24580-ce7a-11eb-958a-2846e2b764e9.png)

![KNNClassification](https://user-images.githubusercontent.com/75968440/122225957-227f4f00-ce7b-11eb-9102-41bf8fd9acf1.png)


### Support Vector Machines

![SVMClassification](https://user-images.githubusercontent.com/75968440/122226045-32972e80-ce7b-11eb-90cc-cb46073a0de1.png)

### Neural Network

![neural-net-summary](https://user-images.githubusercontent.com/75814760/121786327-ce2b5500-cb84-11eb-86e2-2d64562309f6.png)

![neural-net-acc](https://user-images.githubusercontent.com/75814760/121786342-e1d6bb80-cb84-11eb-958a-acaea7b58a87.png)

### Deep Neural Network

![deep-neural-net-summary](https://user-images.githubusercontent.com/75814760/121786346-ec915080-cb84-11eb-8272-3b1505ac06bd.png)

![deep-neural-net-acc](https://user-images.githubusercontent.com/75814760/121786352-fc109980-cb84-11eb-93e3-958953995ef1.png)

## Further Improvements

The models have continued to improve in terms of accuracy, however the last improvements that we can look to make would be by removing similar information and 
consolidating further. This was accomplished by removing the population desity as well as the square area. Lastly we improved the religion column further.
With further tweaking we were able to look within the "Other" religions and look at what religion is practiced by the majority of the population. The majority 
were moved to Christianity and Muslim (Islam). We also increased the hidden layers to 18.

### Improved Artifical Neural Network

![neural-net-combined-summary](https://user-images.githubusercontent.com/75814760/121753627-60295400-cad8-11eb-98f1-3078ccde53b9.png)

![combined-neural-net-acc](https://user-images.githubusercontent.com/75814760/121753651-6a4b5280-cad8-11eb-8143-2504ca10c0c1.png)

### Improved Artifical Deep Neural Network

![deep-neural-net-combined-summary](https://user-images.githubusercontent.com/75814760/121753667-7a633200-cad8-11eb-8104-7869b90e8149.png)

![combined-deep-neural-net-acc](https://user-images.githubusercontent.com/75814760/121753683-84853080-cad8-11eb-8e30-12117ba9f4dc.png)

## Built With

* Pandas
* Jupyter Notebook
* Visual Studio Code
* Machine Learning

## Languages

* Python
* Javascript
* CSS
* HTML
