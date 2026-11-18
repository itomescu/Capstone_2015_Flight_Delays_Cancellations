# **2015 US Domestic Flights Analysis: Delays and Cancellations (Capstone 2)**

*<p style='text-align: left;'> Iulia Tomescu (October, 2021)</p>*
<a href="https://www.linkedin.com/in/iuliatomescu-m/" style="float:left"> Iulia's LinkedIn profile</a><br>
<a href="https://public.tableau.com/app/profile/iulia.tomescu" style="float:left"> Iulia's Tableau portfolio</a> <br>
<a href="https://www.springboard.com/" style="float:left"> Discover Springboard</a>



#### **General note**
>The goal of this Capstone2 project is multifold: **1)** to incorporate all the learnings (technical & analytical skills) acquired throughout the Data Analytics Career Track course offered by Springboard, **2)** to demonstrate & strengthen technical skills and computer literacy such as Python, Tableau, statistics, predictive analytics & modeling, **3)** document the full workflow, from cleaning a large dataset to modeling, in reusable notebooks


#### **Acknowledgments**
>I would like to offer my thanks to my Springboard advisor Akshay Jhawar and all other mentors that gave me support throughout this project (Wayne Ang, Chris Hui, Chris Young)

**Why this data set**
>I chose this data set based of specific analysis targets I aimed to achieve:
>* Rich in dimensions such as categorical, numerical data, geographic data, and time series
>* Prediction potential
>* High potential business impact
>* Interesting subject

**Context**
>* The U.S. Department of Transportation's (DOT) Bureau of Transportation Statistics tracks the on-time performance and the causes of delays and cancellation of domestic flights operated by large air carriers since 2003. Summary information on the number of on-time, delayed, canceled, and diverted flights is published in DOT's monthly Air Travel Consumer Report. It covers nonstop scheduled-service flights between points within the United States (including territories) by the fourteen (14) U.S. air carriers that have at least one percent of total domestic scheduled-service passenger revenues.
>* The current analysis focuses on the 2015 historical daily data of domestic flights operated by large air carriers, which includes specs on airlines, flights, airports, dates, time, and causes of delays and cancellations

**Goals**
>* Identify major drivers for delays and cancellations
>* Build a model to predict overall flight delays

**Data and scope**
>* 5.8 million US domestic flights in 2015 (main file: 29 columns, 592 MB), 14 airlines, 322 airports
>* Cleaning: optimized data types for memory, converted times to timestamps, fixed October airport codes, merged 4 files

**Methods**
>* Python (pandas, Scikit-Learn, Statsmodels), Jupyter notebooks, Tableau
>* Descriptive and inferential statistics; temporal, spatial and airline analysis
>* Multivariate linear regression of delay magnitude, with three models compared (all data; below and above the 99th percentile)

**Key findings**
>* Weather (54%) and carrier issues (28%) caused 82% of cancellations; the top 5 airlines accounted for 75% of cancellations
>* 1.5% of flights were cancelled, most often in winter and on Mondays and Tuesdays
>* Large delays (over 45 minutes) were rare but made up 55% of total delay time; delay propagation (late-arriving aircraft) cost the most time
>* Airlines recovered about half of departure delays in flight; Hawaiian and Alaska performed best on delay time, Spirit and United worst
>* The top 3 airlines carried about 50% of domestic flights (Southwest alone 22%)

**Model**
>* The all-data regression model reached 87% accuracy (based on MAPE) on delay magnitude, using month, day, scheduled time, distance and the five delay causes
>* Because delay causes are recorded after the flight, this model explains delay magnitude rather than forecasting it in advance

**Files**
>* 01 PDF: data examination and cleaning
>* 02 to 03b notebooks: exploratory analysis (cancellations, delays, temporal patterns)
>* 04 notebooks: modeling
>* Presentation PDF: summary presentation (26 slides)


**Sources**
>* Kaggle: https://www.kaggle.com/usdot/flight-delays?select=flights.csv  
>* US Department of Transportation: https://www.transportation.gov/airconsumer
>* Bureau of Transportation Statistics: https://www.transtats.bts.gov
