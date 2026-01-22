# Data Processing and Simple Analyses


Welcome to the last session of the 2025/2026 Python for Psychologists course!



### Introduction to Experimental Work in Python Part 2 - Data Analysis, first steps

In this session, we will jointly go through a tutorial that shows us how to read in data using pandas, and do some simple corrections and first descriptive statistics.
     

### Materials 📓

You find the code for this session in the following [notebook](https://github.com/cfiebach/Python_For_Psychologists_25-26/blob/main/lecture/experiments/intro_psychopy_2_data_analysis.ipynb).

You can download the data we need for this [here](https://github.com/cfiebach/Python_For_Psychologists_25-26/blob/main/lecture/experiments/pfp25_psychopy_data.zip). Please download them, put them into a convenient place on your computer, so that you can access them from jupyter by specifying the path to the data.


### Final Assignment: Modulpruefung

If you choose to do the `Modulpruefung` in this course, you have to complete a final assignment to get a grade! Please note that you also have to register formally for the exam (Pruefungsanmeldung)!

You have already programmed an experiment and submitted a dataset ... this will count as one part of the exam. And you have all done a great job here!

The second part will be to take the data that you generated and that we worked with today and: 

- test them for the presence of outlier(s) and - if present - exclude those outliers from the remainder of the data analysis, 
- define a new variable that separates the words into two experimental conditions: abstract vs. concrete words. 
- When done with this, use this variable first to plot mean and standard deviation for each condition, then
- compare the ratings and the response times between abstract and concrete words using a t test.
- Last but not least, please report what you did and the results in a jupyter notebook that you hand in as your exam.


#### Author Guide Notebook
The notebook should have a nice structure with headlines, text sections and code and results of your code. You should read in the data, describe how you test for outlier(s) and implement this test, exclude outliers if necessary. Then, you should describe how you generate the condition variable (abstract vs. concrete) and implement this. Following this, please (a) visualizee and describe mean differences between abstract and concrete words (don't forget errorbars!), describe the statistical test and implemnt it and report its results. 
Please also don't forget to include your name and Matrikelnumber into the document when you submit.

#### Testing for Outliers
There are many ways to test for outliers. A frequently used approach is to test whether a subject's dependent values (e.g., ratings, RTs) are beyond 3 standard deviations from the mean of the remaining sample. So you might want to iterate over participants and calculate, on every iteration, the mean and std across all but one participant and compare that participant's mean to the mean of the others.

This would be tested for each dependent variable. If you want to be more sophisticated, you could even test this separately for every condition. 

#### Abstract vs. Concrete Words
It should be quite obvious which are which, but just to make sure: 
Abstract words: Ehre, Frieden, Hoffnung, Klugheit, Liebe, Ruhm, Seele, Tragik, Wahrheit, Weisheit
Concrete words: Anker, Apfel, Bagger, Besen, Felsen, Gabel, Hammer, Pfanne, Stuhl, Toaster

### Comparing Abstract and Concrete Words
To plot a mean for comparing experimental conditions, you would calculate it in a way to first calculate a mean within each participant (e.g., a mean across all concrete words within every participant) and then calculate a mean across participants. This 'grand mean' is the mean value you want to plot.

The first t test (rating) will have more the character of a manipulation check - it would be really weird if abstract words would not be rated as more abstract in our sample ... However, it is not unplausible to assume that these ratings take longer for abstract words. We would like to test this assumption with a t test. 

To calculate the t test, you can use scipy or statsmodels packages. I think we have done a t test before!?!

#### Data 
You can get the data from here: TBD



#### Submission of Assignment
Please e-mail the final notebook to fiebach[ at ]psych.uni-frankfurt.de.

**Deadline is March 15, 2026!**


