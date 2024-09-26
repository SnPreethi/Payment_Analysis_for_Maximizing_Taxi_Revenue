# MAXIMIZING REVENUE FOR TAXI CAB DRIVERS THROUGH PAYMENT TYPE ANALYSIS

### INTRODUCTION
<p align="justify">Maximizing revenue in the taxi service industry is essential for both sustained business success and driver satisfaction. This project aims to analyze the impact of different payment methods on taxi fare pricing and draw business insights to optimize revenue. Using statistical techniques and Python, the goal is to determine if a significant difference exists and explore whether this information can be used to encourage payment methods that lead to higher revenue for drivers while still ensuring a positive customer experience.</p>

### DATASET
<p align="justify">The dataset used for this analysis consists of various trip record submissions made by Yellow Taxi. The dataset used in this project contains 18 different columns. It consists of the following fields:

<ol>
<li><b>Vendor ID</b> - Code 1 stands for Creative Mobile Technologies, LLC. Code 2 for VeriFone Inc.</li>

<li><b>Pickup Datetime</b> - The date and time when the meter was engaged.</li>

<li><b>Dropoff Datetime</b> - The date and time when the meter was disengaged.</li>

<li><b>Passenger Count</b> - The number of passengers in the vehicle (value entered by the driver).</li>

<li><b>Trip Distance</b> - The elapsed trip distance in miles reported by the taximeter.</li>

<li><b>Pickup Location ID</b> - TLC Taxi Zone in which the taximeter was engaged.</li>

<li><b>Dropoff Location ID</b> - TLC Taxi Zone in which the tximeter was disengaged.</li>

<li><b>Rate Code ID</b> - The final rate code in effect at the end of the trip.<br>
<ul>
<li>1 = Standard rate</li>
<li>2 = JFK</li>
<li>3 = Newark Airport trips</li>
<li>4 = Nassau or Westchester</li>
<li>5 = Negotiated fare</li>
<li>6 = Group ride</li>
</ul>
</li>

<li><b>Store and Forward Flag</b> - This flag indicared whether the trip record was held in vehicle memory before sending to the vendor because the vehicle did not have a connection to the server.</li>
<li><b>Payment Type</b> - A numeric code signifying how the passenger paid for the trip.<br>
<ul>
<li>1 = Credit Card</li>
<li>2 = Cash</li>
<li>3 = No charge</li>
<li>4 = Dispute</li>
<li>5 = Unknown</li>
<li>6 = Avoided Trip</li>
</ul>
</li>

<li><b>Fare Amount</b> - The time and distance fare calculated by the meter.</li>

<li><b>Extras and Surcharges</b> - Miscellaneous extras and surcharges. Currently, this only includes the $0.50 and $1 rush hour and overnight charges.</li>

<li><b>MTA Tax</b> - $0.50 MTA tax that is automatically triggered based on the metered rate in use.</li>

<li><b>Improvement Surcharge</b> - $0.50 improvement surcharge that is automatically triggered based on the metered rate in use.</li>

<li><b>Tip Amount</b> - Automatically populated for credit card tips. Cash tips are not included.</li>

<li><b>Tolls Amount</b> - Total amount of all tolls paid in trip.</li>

<li><b>Total Amount</b> - The total amount charged to passengers. Does not include cash tips.</li>

<li><b>Congestion Surcharge</b> - Total amount collected in trip for NYS congestion surcharge.</li>
</ol>
<br>
Download Dataset - https://data.world/vizwiz/nyc-taxi-jan-2020/workspace/file?filename=yellow_tripdata_2020-01.csv
</p>

### METHODOLOGY
Following are the steps involved while performing statistical analysis.<p align="justify">
<ol>
<li>Data Cleaning - Removing the inconsistencies from the raw data. It involved dropping unncessary columns, handling missing values, correcting data types, dealing with duplicates, and outlier removal.</li>
<li>Distribution Analysis - How the important features are distributed and studying their characteristics.</li>
<li>Visualizations & Interpretation of Results - Plotting various graphs and plots to visually confirm the interpretations of distribution analysis.</li>
<li>Hypothesis Testing - Testing the correctness of the claims made from distribution analysis and visualizations by formulating hypothesis on dependencies of revenue.</li>
<li>Key Business Insights - Drawing conclusions from various tests to improve the revenue of taxi drivers.</li>
<li>Story Telling</li>
</ol></p>

### FURTHER INVESTIGATIONS
<ol>
<li>During the investigation of relationship between fare amount and duration using regression analysis, 24% of non-linearity was observed. This can be further addressed using polynomial or other non-linear models.</li>
<li>Analysing the impact of performance on addition of more features to the dataset.</li>
<li>Investigating heteroscedasticity (non-constant variance) in all the trip durations, and applying transformations to handle non-constant variance. This can involve transforming variables or using a different model.</li>
</ol>

### NOTE
<ul>
<li>The dataset is a sample of 2020 Yellow Taxi Trip Data, January-June. The findings are based on historical data, and results may vary with different datasets.</li>
<li>This analysis assumes that external factors such as traffic conditions, time of day, or other factors are not considered, and the primary focus is on the relationship between payment type and fare amount. But for further study, few points are noted under the section - "Further Investigations".
<li>Further enhancements such as incorporating real-time data (e.g., traffic patterns, peak hours) or customer demographics could improve the prediction accuracy.</li>
</ul>
