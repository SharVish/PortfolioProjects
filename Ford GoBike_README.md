# Ford GoBike System Data
## by Sharath V


## Dataset

> Ford GoBike System Data includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area.

> The original dataset had 183412 rows and 16 columns. 

> Some of the columns had duplicate data.

> Some of the columns had null values.

> Data types of some columns had to be changed to appropriate ones. 

> A few time-related columns were deduced (newly created) from the 'start_time' and 'end_time' which are useful for the analysis. 

> The following Data Wrangling steps were taken to clean the dataset:

>> Duplicate rows were dropped.
>> Rows with no data (null values) were dropped.
>> Rows with member_birth_year < 1918 (age > 100 years as of 2008) were dropped.
>> Data type of 'start_time' and 'end_time' columns were changed to date-time. 
>> New columns were created: 'Age' (based on the difference between 2008 and user's member_birth_year). Similarly 'hour' and 'day_of_week' were created. 
>> Day of the week was further classified as 'weekday' or 'weekend' in a new column named 'type_of_day'.
>> Finally, the unwanted columns which were not planned to be used in the analysis was dropped. 
>> The clean dataset had 174880 rows and 17 columns. It was saved and exported as a csv file. 



## Summary of Findings

>The following insights were observed from the explorations:

>1. Weekdays appear to be more popular for bike rides compared to weekends. Around 84% of the bike rides fall in the weekdays. Thursday seems to be the most popular weekday for bike rides. 

>2. 7am - 9am and  4pm-6pm seem to be the peak hours based on the no. of rides. The peak hours and more number of rides on weekdays could possibly indicate that working class is the important target customer. However, further data on user's occupation or purpose of ride is necessary to firmly conclude this statement. 

>3. 90% of the bike ride users are subscribers.

>4. Around 75% of the bike ride users are males.

>5. 25-35 Age group contribute to the most no. of bike rides. 

>6. The average duration in minutes is higher for customer user type. Also the maximum and maximum duration ride is higher for customer user type compared with subscriber user type. 

>7. The average duration in minutes seem to be the same across member genders.

>8. The ratio of subscribers to customers seem to be a bit high in females when compared to males.

>9. The no. of rides by customers is almost steady across days of the week, whereas the no. of rides by subscribers tend to be lower in the weekends. The no. of rides drop significantly in the weekend for all genders. 

>10. The distribution of age is similar across member genders and the distribution tends to be skewed to the right.

>11. Higher duration of ride is observed in the 25-45 user age group. 

>12. Overall there appears to be no strong correlation between the variables that were checked in the multivariate exploration. 


## Key Insights for Presentation

>1. Weekdays appear to be more popular for bike rides compared to weekends. 

>2. Peak Hours for bike ride are 7am - 9am and  4pm-6pm. 

>3. Around 75% of the bike ride users are males.

>4. 25-35 Age group contribute to the most no. of bike rides. Additioanally, to finetune this graph, we take a subset of data having duration of ride less than 60 minutes. 