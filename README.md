 # Mission to Mars
## Overview of Project
An aerospace company wants to receive information about news about Mars and the climates on Mars. In this direction, a study was conducted by collecting information from open sources.

### Resources
- Python 3. 9. 12
- Jupyter Notebook 6. 4. 8
- Pandas 1. 4. 2
- Numpy 1. 21. 5
- Splinter 0. 18. 1
- Selenium 3. 141. 0
- Beautiful Soup  4. 11. 1
- PyMongo 4. 3. 3

## Overview of the Analysis  
In general, if we explain how we do our work, we use Splinter, Selenium and WebDriverManager to access the desired website with Splinter. Then, with the help of Beautiful Soup, we follow the HTML commands of the page and obtain the information requested from us. For this study, what is requested from us is the Mars News website. It is possible to access this study from the "mars_data_challenge_part_1.ipynb" section. There are articles in the HTML page and these articles can be obtained in lists with their id's, titles and descriptions. Article lists are exported in JSON format. JSON format is used to export to MongoDB database.
In another study, Jupyter Notebook named "mars_data_challenge_part_1.ipynb", Mars temperature data was accessed in two ways using Splinter, Selenium and WebDriverManager, Beautiful Soup and read_html formats. While accessing the data in both ways is simple, read_html is completed in less time. At the beginning of this study, Mars temperature data on the website was shown as DataFrame and pandas library was used to read HTML. In the study, in both methods, data can be obtained as DataFrame and transferred to MongoDB database. Finally, the cleaning process was performed on the MongoDB database, and the study was terminated.

## Results 
In this study, the temperature values obtained with the help of bar charts are visualized on a monthly basis. In this way, the lowest and highest temperature data and monthly differences in atmospheric pressure values can be easily analyzed. 

#### Chart 1. Average Martian Temperatures
<img width="476" alt="Average_Martian_Temperature_by_Month" src="https://user-images.githubusercontent.com/26927158/203912643-26016db8-1235-4bbf-91cc-2e4da5035498.png">
According to the average mars temperature data according to the months, it can be seen that the values are in (-) degrees. While the warmest value was measured as -68.383 in the 8th month, the coldest month was -83.3073 in the 3rd month.

#### Chart 2. Average Atmospheric Pressure by Month
<img width="468" alt="Average_Martian_Pressure_by_Month" src="https://user-images.githubusercontent.com/26927158/203912797-e1a58d52-8684-4adb-a7f6-333f36f83b1a.png">
According to the months, average atmospheric pressure values, while the highest value was 913.306 in the 9th month, the lowest value was 745.054 in the 6th month.

#### Chart 3. Daily Minimum Temperatures by Year
<img width="436" alt="Daily_Min_Temperature_Observed" src="https://user-images.githubusercontent.com/26927158/203912903-410ccac5-398c-4779-9d54-c2c8ae052444.png">
The Daily Minimum Temperature values are included in the above line chart. If a general judgment is made in the table, the peak years are; It can be named as 2013, 2015 and 2017. The coldest year in general in the Terrestrial date dates can be analyzed as 2014 and 2016.

## Summary 

##### 1. How many months exist on Mars?
Mars has 12 months but the scraped dataset spans 1,967 Martian days.

##### 2. Which month, on average, has the lowest temperature? The highest?
The coldest month is Month 3 with an average temperature of -83.3073°C.
The warmest month is Month 8 with an average temperature of -68.383°C.

##### 3. Which month, on average, has the lowest atmospheric pressure? The highest?
Month 6 has the lowest atmospheric pressure with an average pressure of745.054 Pascals.
Month 9 has the greatest atmospheric pressure with an average pressure of 913.306 Pascals.

##### 4. How many terrestrial days exist in a Martian year? A visual estimate within 25% was made.
The plot seems to show about three Martian cycles over about 5.5 terrestrial years. One Martian year would contain about 669.5 terrestrial days. Mars is a little slower, and farther from the sun, so a full circuit takes 687 Earth days - or one Mars year. That longer year means longer seasons too. Because of that, error is  2.55%.








