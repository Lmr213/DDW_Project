# DDW_Project

Task 1

Find appropriate datasets (at least 30 ~ 50 20 countries because no need to split data here)
Predict number of deaths / death rates within a certain period of time
Predictor variables: percentage of population 65+, percentage of vaccinated people (people fully vaccinated per hundred), number of icu cases, stringency index. 

We need countries which have data for: ICU Patients , GDP per capita PPP  (2018), people fully vaccinated per hundred (Nov 1 2021), and death cases (weekly or biweekly over a specific period)

Fully vaccinated (Percent), ICU Patients (Per Million), Weekly Confirmed Deaths (8 Nov)

Algeria: 10.83   0.31  0.58
Austria: 62.30   34.06   16.15
Belgium: 73.82   27.85   17.71
Bulgaria: 22.03   98.60   159.35    
Canada: 74.39    15.58    25.92 (I checked this, it's 4.44)
Cyprus: 63.70    10.04   2.23
Czech Republic: 56.91  27.13  25.92
Denmark: 75.90   4.99   4.64
Estonia: 57.50   39.99   58.1
Finland: 70.02   4.87   5.41
France: 68.01   15.82    4.32
Germany: 66.18   24.48   10.64
Ireland: 75.33   18.26   11.24
Israel: 61.75   16.04   2.26
Italy: 71.84    6.03   5.02
Luxembourg:EXCLUDED BECAUSE CLOSEST DATA IS AT 7 NOV
Malaysia: 74.59   17.36   11.41
Malta: 83.05   4.40 (Why's this 4.4?)   1.94
Netherlands: 72.80   13.74   9.49
Portugal: 87.41   5.90   4.62
Romania: 33.12   98.08   152.81
Serbia: 43.76    41.98   66.07
Slovenia: 53.81   68.31   41.85
Spain: 79.86   8.69 (Were these 2 interpolated?)   4.07
Sweden: 68.05   2.56   3.15
Switzerland: 63.56   12.74   4.59
United Kingdom: 67.05    15.10   17.52
United States: 57.16   36.37   24.58

Task 2

Justification: We wish to help the countries of the world find out if their vaccination efforts are up to par by predicting the percentage of unvaccinated people getting their first jabs during a certain period, based on factors such as the GDP per capita, number of cases and death cases about 2 weeks before our predicted period.

Row: Country

target column(s)
number of new vaccinations in the following certain period
7-day rolling average (8 Nov)
affected by population size (raw value/population size gives %)


features columns
GDP per capita by year and country (dataset)
Represents economy
Represents education
Number of covid cases in the month before measurement (for trend of people wanting to vaccine) (number of cases in i.e Nov 21) (if possible death cases and normal cases) (Perhaps use a 2 week duration that occurs 1 month before our target) 
Weekly confirmed cases (25 Oct)
Weekly confirmed deaths (25 Oct)
Represents severity of covid in country
