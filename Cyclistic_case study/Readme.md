# About the company
In 2016, Cyclistic launched a successful bike-share offering. Since then, the program has grown to a fleet of 5,824 bicycles that
are geotracked and locked into a network of 692 stations across Chicago. The bikes can be unlocked from one station and
returned to any other station in the system anytime.

Until now, Cyclistic’s marketing strategy relied on building general awareness and appealing to broad consumer segments.
One approach that helped make these things possible was the flexibility of its pricing plans: single-ride passes, full-day passes,
and annual memberships. Customers who purchase single-ride or full-day passes are referred to as casual riders. Customers
who purchase annual memberships are Cyclistic members.

Cyclistic’s finance analysts have concluded that annual members are much more profitable than casual riders. Although the
pricing flexibility helps Cyclistic attract more customers, Moreno believes that maximizing the number of annual members will
be key to future growth. Rather than creating a marketing campaign that targets all-new customers, Moreno believes there is a
very good chance to convert casual riders into members. She notes that casual riders are already aware of the Cyclistic
program and have chosen Cyclistic for their mobility needs.

Moreno has set a clear goal: Design marketing strategies aimed at converting casual riders into annual members. In order to
do that, however, the marketing analyst team needs to better understand how annual members and casual riders differ, why
casual riders would buy a membership, and how digital media could affect their marketing tactics. Moreno and her team are
interested in analyzing the Cyclistic historical bike trip data to identify trends.

# Ask

You will produce a report with the following deliverables:
1. A clear statement of the business task
2. A description of all data sources used
3. Documentation of any cleaning or manipulation of data
4. A summary of your analysis
5. Supporting visualizations and key findings
6. Your top three recommendations based on your analysis

## Business task
### Analyze historical bike trip data to identify trends in how annual members and casual riders use Cyclistic bikes differently.

Three questions will guide the future marketing program:
1. How do annual members and casual riders use Cyclistic bikes differently?
2. Why would casual riders buy Cyclistic annual memberships?
3. How can Cyclistic use digital media to influence casual riders to become members?

# Prepare

#### Where is your data located?
You will use Cyclistic’s historical trip data to analyze and identify trends. Download the previous 12 months of Cyclistic trip data
here(https://divvy-tripdata.s3.amazonaws.com/index.html)
#### How is the data organized?
The data is organized from primary search,It is completely secure and governed.

#### Are there issues with bias or credibility in this data? Does your data ROCCC?
1.Reliable: The data contains 12 months of previous(annual) previous data to analyze the future.The data is completely reflect the overall population
2.Original : we are using an original data source.
3.Current : this dataset is updated monthly. It was last updated jan 4th 2023.
4.Comprehensive : The data contains necessary and important information to find the answers to the questions
5.Cited:these sources are publicly available data provided by Cyclistic and the City of Chicago. Governmental agency data and vetted public data are typically good sources of data.

#### How are you addressing licensing, privacy, security, and accessibility?
The data has been made available by Motivate International Inc. under this license(https://www.divvybikes.com/data-license-agreement).The data is Prohobit to use m using riders’ personally identifiable information.

# Process
* What tools are you choosing?
Microsoft Excel: initial data cleaning and manipulation
#### Data profiling
 The dataset contains the following fields
* ride_id               #Ride id - unique
* rideable_type         #Bike type - Classic, Docked, Electric
* started_at            #Trip start day and time
* ended_at              #Trip end day and time
* start_station_name    #Trip start station
* start_station_id      #Trip start station id
* end_station_name      #Trip end station
* end_station_id        #Trip end station id
* start_lat             #Trip start latitude  
* start_lng             #Trip start longitute   
* end_lat               #Trip end latitude  
* end_lat               #Trip end longitute   
* member_casual         #Rider type - Member or Casual 

#### What steps have you taken to ensure that your data is clean?

1.Cleaning duplicate data:
I removed duplicate records in each individual csv file ,make sure there is no more errors in data to cause false analysis.

2.Null values:
The dataset contains 5667717 rows × 16 columns
eliminating 1941227 rows of bad data is null (34% of the raw dataset).

#### Manupulating the data:
--> Created a column called ride_length
Calculated the length of each ride by subtracting the column started_at from the column ended_at (example: =D2-C2)
Formatted as TIME
Format > Cells > Time > HH:MM:SS (37:30:55) 

--> Create a column called “day_of_week,” 
calculate the day of the week that each ride started using the “WEEKDAY” command (for example, =WEEKDAY(C2,1)) in each file. 
Format as General or as a number with no decimals, noting that
1 = Sunday and 7 = Saturday.
#### Now the data is completely clean , Now that your data is stored appropriately and has been prepared for analysis, start putting it to work.









