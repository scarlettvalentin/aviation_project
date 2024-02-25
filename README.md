<center><img src="https://miro.medium.com/v2/resize:fit:1400/format:webp/1*4_HaFNNr4Zw-7xuH7kK-8Q.png"></center>

# Aviation Industry Expansion
Author: [Scarlett Valentin](https://www.linkedin.com/in/scarlett-valentin/)

# Business Understanding
Our company is *expanding* by **purchasing and operating airplanes** for commercial and private enterprises. In this analysis, I determine which aircraft are the **lowest risk** for the company to start this new business endeavor. I use the fatal injuries rate, uninjured rate, and total number of injuries as meaures of safety and investigate the effect the make of the aircraft, the number of engines, and the location have on these safety parameters.

I investigate the following three business questions:
1. What **number of engines** is least likely to result in a fatal injury?
2. What is the safest aircraft **make**?
3. What is the safest **location** to operate out of?

# Data Understanding

<center><img src="https://www.datasciencecentral.com/wp-content/uploads/2023/10/AdobeStock_623805808.jpeg" style="height:300px" /></center>

The [Aviation Accident Database & Synopses, up to 2023](https://www.kaggle.com/datasets/khsamaha/aviation-accident-database-synopses/data) from the NTSB (National Transportation Safety Board) aviation accident database contains information about ​**civil aviation accidents and selected incidents** that occurred between 1962 and 2023 within the United States, its territories and possessions, and in international waters. From this database, I analyze the numbers of injuries, the make of the aircrafts, the number of engines on the aircrafts, and the location of the incidents to determine our first step in the expansion of the aviation industry.

## Data Preparation

# Exploratory Data Analysis

# Conclusion

## Results
I began with comparing the top 4 aircraft makes with the **average number of injuries** per accident. Bombardier has the *least* average number of injuries, while the average total fatal injuries is greater than Airbus, but comparable to Boeing and Embraer. Boeing has the *highest* average number of minor, serious, and fatal injuries.
<img src="/images/Average Total Injuries By Make.png/" style="height:400px"/>

Bombardier aircrafts with **2 engines** hold both a significantly *higher* uninjured rate and *lower* fatality ratethan bombardier aircrafts with 1 engine.
<img src="/images/Fatality and Uninjured Rates By Number of Engines.png/" style="height:400px"/>

The **northeast** has the *highest* average fatality rate among **Bombardier** aircrafts and the **south** has the *lowest* fatality rate. 
<img src="/images/Average Fatal Injury Rate By Region_Bombardier.png/" style="height:400px"/>

## Limitations
There are various limitations in this analysis.

1. I could not compute the **proportion of accidents to total number of flights**, as this data includes only records of accidents or incidents. This data does not include clean records of flights with no accidents or incidents. When recommending an aircraft company, aircraft model, or location of operation, I used the basis of which has the lowest number of accidents/incidents, with zero accidents/incidents not being an option.

2. I could *not* narrow the data down to **one specific model** that would be the best purchase for our first aircraft. When comparing 2-engine Bombardier aircrafts, many had an uninjured rate of 100%. These would all be viable options, but many more variables go into purchasing the first aircraft. Safety can be further emphasized when including data of successful, accident-free flights (as mentioned above). Models can be further compared using cost, maintenance issues, and size based on how many passengers we wish to transport at one time.

3. I could *not* narrow the data down to **one specific city** for us to begin operating out of. There were not enough factors that would effect location to determine a safe choice. Additionally, with only 25 data points of Bombardier aircrafts in the south, I do not know if location is a factor of fatal injury rates. Are Bombardier flights safer in the south or are there less Bombardier flights in the south?

## Recommendations
This analysis has led me to conclude the following three recommendations: 
1. **Bombardier** is the aircraft manufacturer that I suggest we purchase. Bombardier has overall the least average number of injuries and the highest unijured rate when compared to Airbus, Boeing and Embraer.

2. I recommend we purchase a Bombardier aircraft with **2 engines**. Bombardier aircrafts only come with 1 or 2 engines. According to the data, 2-engine aircrafts have a *lower* fatality rate and a *higher* uninjured rate that 1-engine aircrafts.

3. To initialize our aviation operation, I recommend we begin in the **south** region of the **United States**, as to operate close to home and not have the added challenges of customs and international flights. I was not able to narrow down a city with the given data. Further analysis is required.

## Next Steps
In order to optimize ***profits*** for this new industry expansion, we must analyze the financial aspects by answering the following three questions: 

1. What **flight schedule** will provide the greatest profit? Consider seasonal, weekly, and daily schedules. 

2. **How many aircrafts** should we initially purchase? Consider *cost* of aircraft and operation of such aircraft.

3. What **city** should we operate out of? Let's plan to narrow this down further. Consider chances of interrupted flight due to *weather*.

# For More Information
See the full analysis in the [Jupyter Notebook](/notebook.ipynb/), review this [presentation](/presentation.pdf/), or review the [interactive dashboard](https://public.tableau.com/app/profile/scarlett.valentin/viz/Aviation_Expansion_Dashboard/AverageTotalInjuriesByMake?publish=yes)

For additional information, contact Scarlett Valentin at scarlettmvalentin@gmail.com.




# Repository Structure


```
├── code
│   ├── __init__.py
│   ├── data_preparation.py
│   ├── visualizations.py
│   └── eda_notebook.ipynb
├── data
├── images
├── __init__.py
├── README.md
├── presentation.pdf
└── analysis.ipynb
```
