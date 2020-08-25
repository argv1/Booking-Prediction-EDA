![logo](https://github.com/argv1/Booking-Prediction-EDA/blob/master/img/logo_reservation_prediction.png)
# Booking-Prediction-EDA
======================

## Business Understanding and Set-up
Analysis of the booking data of a hotel chain/ hotel cooperation with five properties in locations.

### DataSet
The dataset contains bookings made in five different hotels from one hotel chain.
One line corresponds to one person. For example, a double room is usually displayed in two rows with the same booking number. (Could also be two single rooms)
The customer id is also assigned per person and provides information about whether customers book in several houses or more than once in one house.

Dimensions:
- 98 features (57 original + 41 new)
- 245k assignments


### Goal
- Help identify repeating customers, as well as the features used for predition.
- Recognition of guests who are willing to spend above average amounts of money (called VIPs). 
- Predict in which quarter and destination customer will book their next stay.


### Final Deliverables
- Jupyter notebook following PEP8 designed for data science / technical audience.
- Slide deck (pdf / 10min presentation) pushed to GitHub designed for non-technical stakeholders outlining findings and recommendations, as well as future work.


### Key Question
- How to identify repeating customers?
- What distinguishes VIPs from the other guests?
- What do repeating customers/ VIPs have in common?


### Step by step
this notebook:
- Merging the three datasets
- Cleaning
 - handling missing values
 - inconsistency checks
 - change variable types

next notebooks:
- Feature engineering
- EDA
- Basic and advanded modelling
- TimeSeries
- Conclusion


### Outcome/TakeAways
- Columns reise_special_event & flag_old have no value for the analysis
- Columns lkz & sprache_deutsch have low value for the analysis
- Guest of the Viana do Castelo show a different booking behaviour than the rest
- Guest from Linz and Düsseldorf are very similar. 
- Adaboost is best suited for forecasting regular guests.
- To identify solvent customers, a logistic regression with dummie variables turned out to deliver the best result.


### To-Do-List / Outlook
- Adding additional information like:
 - Events at the destination
 - Cancellations
 - Revenue per available room (required capacity for each destination)
 - Feedback from tripadvisor, yelp, etc. as well as from hotel internal surveys


### Files and Folders
- dataset can not be published due to nda
- data/glossary.xlsx: list of all features
- slides/slides.pdf: slide deck visualising the findings (10min.)
- 1-Cleaning.ipynb: Data cleansing for subsequent EDA
- 2-EDA.ipynb: jupyter notebook with Exploratory Data Analysis (EDA), visualizations, further documentation
- 3-Modelling_Repeater.ipynb: predicting repeating customers
- 4-Modelling_VIPs.ipynb: predicting solvent guests


### Python Modules used:
Pandas / NumPy / Matplotlib / Seaborn / sklearn


### License
This code is licensed under the [GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/). 
For more details, please take a look at the [LICENSE file](https://github.com/argv1/Booking-Prediction-EDA/blob/master/LICENSE).

