# Airport-Crashes-and-Fatalities-since-1908
This is a Capstone project for Microsoft #NG30DAYSOFLEARNING. 

# Project objective : Problem statement
- The aim of this project is to analyze and develop visualization for the dataset which shows the trends of Airplane Crashes and number of Fatalities. We have considered answering some of the questions below:
- What is the Total number of Airplane Crashes from 1908 to 2009?
- what is the Total number of Fatalities from 1908 to 2009?
- What is the Total number of Passengers involved in the Crashes from 1908 to 2009?
- What is the Fatality rate?
- How many planes crashed per Year? how many people were on board? how many survived? how many died?
- What is the highest number of crashes by operator and Type of aircrafts?
# Data sourcing
The Dataset was culled from https://github.com/theoyinbooke/30Days-of-Learning-Data-Analysis-Using-Power-BI-for-Students/blob/main/Airline%20Project/Airplane_Crashes_and_Fatalities_Since_1908.csv. The dataset contains data of airplane accidents involving civil, commercial and military transport worldwide from 1908-09-17 to 2009-06-08.

# Data Transformation
- Expanded necessary column's width to prevent text overflow.
- Used the Date column to create new Year, Month and Day columns.

- Used the Aboard and Fatality column to get survial column.

# Data Modelling
- Calculated a Dax measure to ascertain the Total number of Crashes, by Counting the Total number of rows using the following formula : Total crashes = Count((Airplane_Crashes_and_Fatalities_since_1908[).
-  Calculated a Dax measure to ascertain the Total number of Fatalities, by summing the Fatalities column using the formula: Total fatalities = sum(Airplane_Crashes_and_Fatalities_since_1908[Fatalities])
-  Calculated a new Dax measure to ascertain the Total number of Passengers, by summing the Passengers column using the formula: Total passengers = sum(Airplane_Crashes_and_Fatalities_since_1908[Passengers])
-  Calculated the Fatality rate using the formula: Fatality rate = Divide([Total Fatalities],[Total passengers]×100

# Data Visualization/Analysis.
Visualization was done using simple visuals such as bar charts, line graphs, e.t.c. for easy comprehension

# Total Crashes
Total crashes There is a Total of 5,268 crashes
![IMG_5992](https://user-images.githubusercontent.com/68191668/179905982-2f513b46-ecc4-485b-b638-97ff9982df28.jpeg)

# Total fatalities
Total fatalities  There is a Total of 105,479 Fatalities
![IMG_5993](https://user-images.githubusercontent.com/68191668/179905919-8fdf13a3-0372-47e2-9946-958c6b9d3f4b.jpeg)

# Fatality Rate
Fatality rate There is a Fatality rate of 72.97%
![IMG_5989](https://user-images.githubusercontent.com/68191668/179905842-2583614e-05eb-4e83-8289-3e92f01f28bb.jpeg)


# Slicers
Year, Month, Route and Location slicers to filter visuals slicers.
![IMG_5990](https://user-images.githubusercontent.com/68191668/179907893-61c4ee1e-2586-4717-8a88-1117d3b1c91e.jpeg)


# Top 5 years with most fatalities
Top 5 years with most fatalities  1972 has the highest number of Fatalities with a Total of 2,937 Fatalities
![IMG_5991](https://user-images.githubusercontent.com/68191668/179906122-f9a97272-15aa-4ca1-98be-f7ed17294334.jpeg)

# Top 5 operators with highest fatalities
Top 5 operators with highest fatalities  Aeroflot has the highest number of crashes with a Total of 7156 deaths.
![IMG_5994](https://user-images.githubusercontent.com/68191668/179907554-cbfe7d6a-4432-43ed-8051-6495a2e0ac72.jpeg)


# Top 5 operators with highest crashes
Top 5 operators with highest crashes  Aeroflot has the highest number of crashes with a Total of 179 crashes.
![IMG-5997](https://user-images.githubusercontent.com/68191668/179907626-e0314ea8-7242-4617-bbb0-537da5873e53.jpg)

# Top 5 Airplane Types with most Crashes
Top 5 Airplane types with most crashes Douglas DC-3 has the highest number of crashes with a Total of 334 crashes.
![IMG-5996](https://user-images.githubusercontent.com/68191668/179904806-b17b3a9d-f2ba-4fc0-9fb3-f23fcca82bc6.jpg)

# Top 5 Airplane Operators with the least Crashes
Southwest Airlines tops the chart.
![IMG_5995](https://user-images.githubusercontent.com/68191668/179904059-3e75eda5-303e-4b0d-8180-02da3da2c640.jpg)

# Conclusion.
- The 1972 has the highest number of Fatalities and highest number of crashes.
- Douglas Airplanes have the highest number of crashes as the planes took first,third,fourth and fifth places in number of Crashes.
- Years with high crashes might not have the highest Fatalities as one as to factor in the size of the craft.
- Aerofloat wins as the operator with the highest number of crashes and fatalities. There is reason to believe that because Aerofloat came into existence in 1923, they obviously would have a high number of crashes under their belt,chalk it up to experience.
