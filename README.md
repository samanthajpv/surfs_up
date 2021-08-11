# Surfs_Up

## Project Overview
Putting up a business that highly depends on weather condition requires more than just a great product or service. By doing a weather analysis, future business owners will be able to assess whether or not the business will be sustainable. The purpose of this project was to determine temperature trends in the island of Oahu using Python, SQLite, and SQLAlchemy to be used for the planning of a surf and ice cream shop. 

### Resources
- Data Source:
    - [hawaii.sqlite](https://github.com/samanthajpv/surfs_up/blob/32fffbdbab089d77062210306cf8cf963f371fc1/hawaii.sqlite) - Historical weather data on Oahu
- Language: Python 3.7.10
    - Dependencies:
        - Numpy, Pandas, SQLAlchemy, Matplotlib
- Software: Jupyter Notebook 6.3.0, SQLite (RDBMS)
- [Complete Code](ADD LINK)

## Results
Querying data from the SQLite database was performed using SQLAlchemy. The temperatures for June and December were the months analyzed in this project. It was decided that a 6 month gap would give a decent representation of the weather changes throughout the year. ```.describe()``` was used to get a descriptive statistics summary.
INSERT PHOTO

- **Observation Count**
There are more temperature observations recorded for the month of June. December has around 10% less observation counts but this is still a good number given that it's not that far behind 1700. Results will nonetheless yield numbers from a considerable amount of records.
- **Minimum Temperature**
The second noticeable difference is the minimum recorded temperature. The mean, percentiles, and maximum temperatures all decreased from June to December but within the range of 5 degrees Farenheit. As it gets cold during December, the temperature can go as low as 56°F, 8 degrees below the minimum temperature in June. 
- **Range of Temperature**
The standard deviation of the temperatures in December is higher by 0.49. This means that the range of temperatures in Decemeber is a little more spread out compared to June. June temperatures vary within the range of 21 degrees from 64-85°F, while December temperatures change within the range of 27 degrees, from 56-83°F.

## Summary
Overall, the temperature in Oahu is looking great for a surf and ice cream shop. June and December temperatures do not have much difference except that it can get to the 50s during December. Below are additional queries that give more insight on the weather data (refer to the Additional Queries section of [code](LINK)).
- **Observation Count**
Upon further analysis, it was discovered that there are no temperature records for December 2017, hence the lower count in the summary statistics. In order to provide a more coherent output, the summary statistics for both months were recalculated without the 2017 data. Although not much has changed in the June statistics, except for the obvious lower observation count, it is better to analyze and compare data that is consistent.
PHOTO
- **Precipitation**
It will also be helpful to look at other months when it comes to frequency of rain that the island experiences. An additional query was performed to first, get the active stations that recorded precipitation over the last 3 full years, and then get the average precipitation in the island for each year. It can be seen in the image below that the island experienced its peak mid July and intermittent high amount of precipitaion up to the month of November when compared to other months.
PHOTO

## Reference
(1) Trilogy Education Services. (2021, August). *Module 9 Challenge*. https://courses.bootcampspot.com/courses/626/assignments/13402?module_item_id=212923

(2) Everilä, I. (2018, April 4). Answer on the online question post *Group by month and year from date field*. Stack Overflow. Retrieved on August 9, 2021 from https://stackoverflow.com/questions/49646848/group-by-month-and-year-from-date-field