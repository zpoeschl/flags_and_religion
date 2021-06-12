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
* Neural Network
* Deep Neural Network
* Additional 
* Additional

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

### Neural Network

![neural-net-summary](https://user-images.githubusercontent.com/75814760/121753219-90bcbe00-cad7-11eb-9712-4f22bed865be.png)

![neural-net-acc](https://user-images.githubusercontent.com/75814760/121753237-9a462600-cad7-11eb-8db4-17d695ba0d0d.png)

### Deep Neural Network

![deep-neural-net-summary](https://user-images.githubusercontent.com/75814760/121753272-aa5e0580-cad7-11eb-9ced-18d199bc8e0a.png)

![deep-neural-net-acc](https://user-images.githubusercontent.com/75814760/121753288-b3e76d80-cad7-11eb-9c5a-38159f82514b.png)


### Improvements
We originally used 8 outputs (religions). However, with a bit of tweaking you will notice that there may be room to consolidate. By combining "Catholic" with "Other Christian", looking at the "Ethnic" countries and utilizing the majority religion of that country and combining "Marxist" and "Other" due to Marxism not being a religion we were able to narrow our religions to 5.

![religion_screenshot](https://user-images.githubusercontent.com/75814760/121753472-0de83300-cad8-11eb-8ceb-069ec3f3bcd0.png)

We then repeated our steps for the neural and deep neural technique.

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
