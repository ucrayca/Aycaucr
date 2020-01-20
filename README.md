# Aycaucr

RULE datasetinin referans çalışması: [blog](https://rrighart.github.io/Gatu/)

bu haftalık blog yazıları: [link](https://hackernoon.com/@karimcmahon)

## Giriş

### 1.1 Introduction Statistics

#### Descriptive Statistics

1- Measures of central tendency
  * mean(average)
  * median (middle term)
  * mode(highest frequency)
    - bimodal : two values appeared same time and more than the rest of the values then the data set
    - multimodel : for n nodes

2- Measures of variability (spread)
  * standard deviation : the measurement of average distance between each quantity and mean
  * mean deviation / mean absolute deviation
  * variance : square of standard deviation
  * range : highest - lowest value
  * percentile : values in data set should always be in ascending order // if k is nth percentile, it implies that n% of the total terms are less than k
  * quartiles : 
    - First quartile (median of upper half of the data) = 25%
    - Second quartile (median ) = 50 %
    - Third quartile (median of lower half of the data) = 75 %
      - Interquartile range (IQR) : Q3 - Q1

3- Skewness " positive - negative - undefined "
  * positive skewness : right-hand side is longer than the tail on the left-hand side // mean > mode
  * negative skewness : left-hand side is longer than the tail on the right hand side // mean < mode
  * mode skewness : (mean - mode)/standard deviation
  * median skewness : 3*(mean - median)/standard deviation

4- Correlation : [ -1.0 , +1.0] // grafik eğimi positive ise r>0 ; negative ise r<0 ; eğim 0 ise r=0

#### Statistical Distributions

1- Continuous : A number within a range of values, usually measured

  > Uniform :  a type of probability distribution in which all outcomes are equally likely; each variable has the same probability that it will be the outcome. 
continuous random variable x has a uniform distribution, denoted U(a, b), if its probability density function is:
            
      f(x) = 1 / (b−a)

  > Nominal : the specific form of the normal distribution depends on 2 parameters: the expectation (µ) and variance (σ^2) - N(m,σ ^2)

 * µ (expectation) : the distribution center, which corresponds to the maximum height of the graph.
 * σ^2 (variance) : characterizes the range of variation, the “spreading” of the data.
    
       f(x) = 1 / (σ√2π) exp (−(x−μ) ^ 2 / 2 σ ^2)

2- Discrete : Only take certain values (can’t be decimal), usually counted

  > Bernoulli (binomial) : the upcoming event (positive outcome) is also called "success."
the ratio of positive outcomes to the total number of tests tends to the probability of the occurrence of this event.

    f(x) = (n x) p ^ x(1−p) ^ (n−x)
    
        n = the number of experiments in the series
        x = a random variable (the number of occurrences of event A)
        p^x = the probability that A happens exactly m times
        q = 1 - p (the probability that A does not appear in the test)

  > Poisson : is obtained as a limiting case of the Bernoulli distribution, if we push p to zero and n to infinity, but so that their product remains constant: np = a. 

f(x) = [(e ^−λ) * (λ^x ) ] / x!
    
    The average number of events in an interval is designated λ.
    λ = the event rate also called the rate parameter. It is also equal to mean and variance.
    
#### Descriptive Analysis

Helps you detect outliers and typos, and enable you identify associations among variables, thus preparing you for conducting further statistical analyses.

There are two types
1. Descriptive analysis for each individual variable

2. Descriptive analysis for combinations of variables

Variable can be classified into quantitative and categorical
1. Quantitative variables : represent quantities or numerical values

2. Categorical variables : describe quality or characteristics of individuals

* Descriptive Analysis for each individual variable

  * Quantitative variables ;

     - create a histogram
     - a box-and-whisker plot to get an idea of the shape of the distribution.
     - the shape is symmetric ; calculate and present mean and standard deviation
     - the shape is skewed ; calculate and present median and quartiles.
     - calculate and present min and max values.
     - help you identify outlying and improbable values so that you can double check data entry errors.

  * Categorical variables ;

    - create frequency tables
    - present them in bar charts, pie charts or doughnut charts

* Descriptive analysis for combination of two variables

     1- Both variables quantitative: Create a scatter plot.

     2- One variable categorical and the other quantitative: Calculate summary statistics and box-and-whisker plots of the quantitative variable classified by the categorical variable.

     3- Both variables categorical: Prepare a contingency table.

### 1.2 Introduction Machine Learning

#### CLUSTERING

* Unsupervised learning method

* The task of dividing the population or data points into a number of groups such that data points in the same groups are more similar to other data points in the same group than those in other groups. In simple words, the aim is to segregate groups with similar traits and assign them into clusters.

* Clustering is very much important as it determines the intrinsic grouping among the unlabeled data present. There are no criteria for a good clustering. It depends on the user, what is the criteria they may use which satisfy their need.

* Divided into two subgroups :

      Hard Clustering: In hard clustering, each data point either belongs to a cluster completely or not.

      Soft Clustering: In soft clustering, instead of putting each data point into a separate cluster, a probability or likelihood of that data point to be in those clusters is assigned.

* Clustering Methods :

      1. Density-Based Methods
      2. Hierarchical Based Methods 
      3. Partitioning Methods
      4. Grid-based Methods

* Clustering Algorithms :

> K-means clustering algorithm : It is the simplest unsupervised learning algorithm that solves clustering problem. K-means algorithm partition n observations into k clusters where each observation belongs to the cluster with the nearest mean serving as a prototype of the cluster .
                  
                   1. Specify the desired number of clusters K
                   2. Randomly assign each data point to a cluster 
                   3. Compute cluster centroids 
                   4. Re-compute cluster centroids 
                   5. Repeat steps 4 and 5 until no improvements are possible 
