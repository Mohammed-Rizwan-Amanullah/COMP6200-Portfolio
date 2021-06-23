![ScreenShot](https://github.com/MQCOMP6200/portfolio-s1-2021-mohrizwan1993/blob/main/data/Images/logo.png)
  </a>

  <h3 align="left">Portfolio-S1-2021</h3>

  <p align="left">
    This repository holds portfolio submission for the unit <b>COMP6200 Data science</b>		<br>
    <b><i>Student id : 46277404</i></b><br>
    <b><i>Student Name : Mohammed Rizwan Amanullah</i></b>
    <br />
  </p>

<!-- TABLE OF CONTENTS -->

<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li>
      <a href="#about-the-portfolio-assignment">About The Portfolio</a>
    </li>
    <li>
      <a href="#portfolio-one">Portfolio 1</a>
      <ul>
        <li><a href="#1.1 Data Source">1.1 Data Source</a></li>
        <li><a href="#1.2 Analysis to be performed">1.2 Analysis to be performed</a></li>
        <li><a href="#1.3 Summary">1.3 Summary</a></li>
      </ul>
    </li>
    <li>
      <a href="#portfolio-two">Portfolio 2</a>
      <ul>
        <li><a href="#2.1 Data Source">2.1 Data Source</a></li>
        <li><a href="#2.2 Analysis to be performed">2.2 Analysis to be performed</a></li>
        <li><a href="#2.3 Results obtained">2.3 Results obtained</a></li>
      </ul>
    </li>
    <li>
      <a href="#portfolio-three">Portfolio 3</a>
      <ul>
        <li><a href="#3.1 Data Source">3.1 Data Source</a></li>
        <li><a href="#3.2 Analysis to be performed">3.2 Analysis to be performed</a></li>
        <li><a href="#3.3 Summary">3.3 Summary</a></li>
      </ul>
    </li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



# About The Portfolio Assignment

This repository holds three portfolios. 

- Portfolio 1 is **Analysis of cycling data** where we analyse data from strava and cheetah database
- Portfolio 2 is **Data driven prediction models of energy use of appliances in a low-energy house** where we reproduce some work on predicting energy use of household appliances based on IoT measurement of temperature, humidity and weather observations
- Portfolio 3 is **Analysis of CMU Book summary dataset ** where we use machine learning model to predict the genre of the book based on its summary

Lets look at each portfolio in detail in below sections.

<!-- GETTING STARTED -->

# Portfolio one

![ScreenShot](https://github.com/MQCOMP6200/portfolio-s1-2021-mohrizwan1993/blob/main/data/Images/bike.jpg)

#### <a name="1.1 Data Source">1.1 Data Source</a>

​	The data is a set of  Professor Steve's cycling history over the last couple of years exported from a couple of different systems. We have data provided from Strava and cheetah along with the weather data for the year 2018 and 2019.

The data files are available in the folder **/data/portfolio_1**.

**strava** :- Strava is an internet service for tracking human exercise which incorporates social network features. It is mostly used for cycling and running using GPS data. 

#### <a name="1.2 Analysis to be performed">1.2 Analysis to be performed</a>

- Join the strava and cheetah database and remove rides that has no measured power
- Distributions of some key variables: time, distance, average speed, average power, TSS. Check whether they are normally distributed.
- Explore the relationship between variables and check the correlation between them.
- Explore the difference between three workout type: Ride, Race and workout
- Join the weather dataset and explore the relationship between ride and weather.
  - Find relationship between distance travelled and the temperature
  - Find relationship between average speed and temperature

#### <a name="1.3 Summary">1.3 Summary</a>

In this portfolio, we have performed analysis on some key variables and found the relationship between them. Additionally, with the help of weather data we analysed and found there is a relationship between temperature and distance covered.

<!-- USAGE EXAMPLES -->

# Portfolio two
![ScreenShot](https://github.com/MQCOMP6200/portfolio-s1-2021-mohrizwan1993/blob/main/data/Images/bulb.jpg)

The aim of this portfolio is to reproduce some work on predicting energy usage of a house appliances based on IoT measurement of temperature, humidity and weather observations.

### <a name="2.1 Data Source">2.1 Data Source</a>

The dataset is obtained from the research paper below.

**Data driven prediction models of energy use of appliances in a low-energy house**. Luis M. Candanedo, Véronique Feldheim, Dominique Deramaix. Energy and Buildings, Volume 140, 1 April 2017, Pages 81-97, ISSN 0378-7788, http://dx.doi.org/10.1016/j.enbuild.2017.01.083.

The data files are available in the folder **/data/portfolio_2/**.

Data used include measurements of temperature and humidity sensors from a wireless network, weather from a nearby airport station and recorded energy use of lighting fixtures. 

The data has been split into train and test data. As the dataset contains several features and the airport weather station is not at the same location as the house, we have to figure out the important parameter that helps to improve the prediction of appliances energy. RFE and RFECV algorithm is used to find the optimal number of features in train and test datset.

### <a name="2.2 Analysis to be performed">2.2 Analysis to be performed</a>

- Measure the appliances energy consumption for the whole period and plot the graph
- Plot a graph representing appliances energy consumption for one specific week
- Analyse the distribution using histogram and boxplot
- Produce heatmap showing hourly consumption of energy for four consecutive weeks
- Produce pairgrid plot showing the relationship between the appliances energy and the temperature measured in various part of the house.
- Perform linear regression on train and test data. Use RFECV (Recursive Feature Elimination and Cross-Validation Selection) and RFE. 

### <a name="2.3 Results obtained">2.3 Results obtained</a>

Overall,  in this portfolio I have reproduced work that was part of the research paper and performed Linear regression using REFCV and RFE on train and test data respectively.

Comparing the values obtained in train and test data.

#### Train data

#### Research paper

- **RMSE - 93.21**
- $R^2 = 0.18$
- **MAE = 53.13**
- **MAPE = 61.32**

#### Reproduced in portfolio - RFECV

- **RMSE - 93.29**
- $R^2 = 0.17$
- **MAE = 53.21**
- **MAPE = 61.40**

#### Test data

#### Research paper

- **RMSE - 93.18**
- $R^2 = 0.16$
- **MAE = 51.97**
- **MAPE = 59.93**

#### Reproduced in portfolio - RFE

- **RMSE - 93.24**
- $R^2 = 0.15$
- **MAE = 51.59**
- **MAPE = 59.36**

<!-- Portfolio three -->

## Portfolio three
![ScreenShot](https://github.com/MQCOMP6200/portfolio-s1-2021-mohrizwan1993/blob/main/data/Images/book.jpg)

### <a name="3.1 Data source">3.1 Data source</a>

Aim of this portfolio is to predict the genre of the book based on the book summary. The data files are available in the folder **/data/portfolio_3/booksummaries.txt**.

### <a name="3.2 Analysis performed">3.2 Analysis performed</a>

At first, I performed **data cleaning**(removing empty spaces, remove backslash and apostrophe) and then **removed the stop words(common words like a, an, the, etc.)**. After that, performed **Lemmatization** to group the different version of the same word into one single word.

Once data cleaning was performed, I did data data mapping for genre column. This portfolio involves feature extraction and performing five machine learning models. The model with the higest accuracy score is used to perform model inference. Below mentioned models are built as part of this portfolio

- Logistic Regression
- SVM(Linear)
- SVM(kernal)
- Gaussian Naive Bayes
- Multinomial Naive Bayes

### <a name="3.3 Summary">3.3 Summary</a>

After performing the five machine learning algorithms the results are as below

##### Logistic regression

```
Logistic regression time is 6.959456920623779
Accuracy score on test data is 0.7107761027359017
Accuracy score on train data is 0.8856624319419237

```

##### SVM (Linear)

```
SVM linear time is 89.08458495140076
Accuracy score on test data is 0.7152428810720268
Accuracy score on train data is 0.9396900739913444
```

##### SVM (Kernal)

```
SVM rbf time is 116.97084188461304
Accuracy score on test data is 0.7051926298157454
Accuracy score on train data is 0.9801759039508586
```

##### Gaussian Naive Bayes

```
Gaussian naive bayes time is 9.047112226486206
Accuracy score on test data is 0.5002791736460078
Accuracy score on train data is 0.9420633812648331

```

##### Multinomial Naive Bayes

```
Multinomial naive bayes time is 0.961712121963501
Accuracy score on test data is 0.6901172529313233
Accuracy score on train data is 0.9128856624319419

```

 As the **SVM Linear** had the high accuracy score, I used it to perform model inference. Please refer the jupyter notebook file for reference



## <a name="Contact">Contact</a>

Mohammed Rizwan Amanullah - [@email](mohrizwan1993@gmail.com)

Portfolio Link: [Portfolio Assignment](https://github.com/MQCOMP6200/portfolio-s1-2021-mohrizwan1993)




