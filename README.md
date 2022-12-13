# School_District_Analysis
PyCitySchools with Pandas

## Main Objective
Open Jupyter Notebook files from local directories using a development environment.
Read an external CSV file into a DataFrame.
Format a DataFrame column.
Determine data types of row values in a DataFrame.
Retrieve data from specific columns of a DataFrame.
Merge, filter, slice, and sort a DataFrame.
Apply the groupby() function to a DataFrame.
Use multiple methods to perform a function on a DataFrame.
Perform mathematical calculations on columns of a DataFrame or Series.

## Purpose
A school district asked for a snapshot of several key metrics by each school campus and by the district level. The main analysis focused on the performance of math and reading scores disaggregated several ways in preparation for a board meeting. However, after the school board reviewed the data, it was determined that the data from Thomas High School's 9th grade class was suspect of cheating. The school board asked for the data to be removed and analyzed again for a comparison.
# Results
## How is the district summary affected?
Original Analysis:
<img width="700" alt="Original_Analysis" src="https://user-images.githubusercontent.com/109055148/207220981-b220ab8a-ab9f-432a-91d5-bccec6965cea.png">
The testing data of 461 9th graders at Thomas High School was turned into null data, which recalculated the percentages of passing math, passing reading, and the overall passing. The total count of students did not change as that was run on the count of the student ids, which was not turned into null data.
Adjusted Analysis:<img width="699" alt="Adjusted_Analysis" src="https://user-images.githubusercontent.com/109055148/207221112-cad33d84-7cfb-4074-8080-37439c960fe3.png">
When comparing the two charts, removing less than 500 test scores had a nominal impact on the almost 40,000 student data set. The change was less than a 1% difference and the numbers would still round to the same whole number.
# How is the school summary affected?
In the original analysis, Thomas High School started with a 91% overall passing rate, which was a concern to the school board as being too high. After calculating the total number of 10th - 12th grade students as the new denominator, the rest of the testing data was adjusted accordingly.
Removing the 9th grade students from the data set had a huge impact by dropping from 91% to 65% for the overall passing rate.

## How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
In the original analysis, Thomas High School ranked 2nd in the district raising red flags with the school board.
Original Version
<img width="748" alt="1_top_5_schools" src="https://user-images.githubusercontent.com/109055148/207221443-a13a4a40-f28d-4272-8a38-6edda6bac5b9.png">
Adjusted Analysis
<img width="743" alt="2_bottom_8_schools" src="https://user-images.githubusercontent.com/109055148/207221547-022e1fb6-e7c0-4745-9cea-e2a455537ebd.png">


