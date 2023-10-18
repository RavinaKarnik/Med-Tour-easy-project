# Med-Tour-easy-project

# Analyze Death age difference of right handers with left handers.

In this Project, we will explore this phenomenon using age distribution data to see if we can reproduce a difference in average age at death purely from the changing rates of left-handedness over time, refuting the claim of early death for left-handers. This notebook uses pandas and Bayesian statistics to analyze the probability of being a certain age at death given that you are reported as left-handed or right-handed.

A National Geographic survey in 1986 resulted in over a million responses that included age, sex, and hand preference for throwing and writing. Researchers Avery Gilbert and Charles Wysocki analyzed this data and noticed that rates of left-handedness were around 13% for people younger than 40 but decreased with age to about 5% by the age of 80. They concluded based on analysis of a subgroup of people who throw left-handed but write right-handed that this age-dependence was primarily due to changing social acceptability of left-handedness. This means that the rates aren't a factor of age specifically but rather of the year you were born, and if the same study was done today, we should expect a shifted version of the same distribution as a function of age. Ultimately, we'll see what effect this changing rate has on the apparent mean age of death of left-handed people, but let's start by plotting the rates of left-handedness as a function of age.

This Project uses two datasets: death distribution data for the United States from the year 1999 (source website here) and rates of left-handedness digitized from a figure in this 1992 paper by Gilbert and Wysocki.

# Applying Bayes' rule
The probability of dying at a certain age given that you're left-handed is not equal to the probability of being left-handed given that you died at a certain age. This inequality is why we need Bayes' theorem, a statement about conditional probability which allows us to update our beliefs after seeing evidence.

We want to calculate the probability of dying at age A given that you're left-handed. Let's write this in shorthand as P(A | LH). We also want the same quantity for right-handers: P(A | RH).

Here's Bayes' theorem for the two events we care about: left-handedness (LH) and dying at age A.

P(A|LH)=P(LH|A)P(A)P(LH) 

P(LH | A) is the probability that you are left-handed given that you died at age A. P(A) is the overall probability of dying at age A, and P(LH) is the overall probability of being left-handed. We will now calculate each of these three quantities, beginning with P(LH | A).

To calculate P(LH | A) for ages that might fall outside the original data, we will need to extrapolate the data to earlier and later years. Since the rates flatten out in the early 1900s and late 1900s, we'll use a few points at each end and take the mean to extrapolate the rates on each end. The number of points used for this is arbitrary, but we'll pick 10 since the data looks flat-ish until about 1910.

# Usage :- 
1. Clone the repository:
Git clone :- https://github.com/RavinaKarnik/Med-Tour-easy-project
2. Open the Files which is our dataset.
3. Navigate to the respective reports to access the analysis and insights.
4. Customize the reports as per your requirements by modifying the data sources or adding additional calculations.
5. Analysis the report with the help of visualizing Google colab.

# Contributing :-
Contributions are welcome! If you have any ideas, suggestions, or improvements, please open an issue or submit a pull request.

## Linkeddln Post link :- 
https://www.linkedin.com/feed/update/urn:li:activity:7114526818866462720/

# Acknowledgements :-
1. The Dataset provided by med tour easy company and  is used for this project.
2. Special thanks to the contributors and developers of Excel and google colab and also related tools for enabling powerful data analysis and reporting capabilities.


