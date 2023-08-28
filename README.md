# motor_vehicle_collisions_project
  # Introduction:
Our project aims to create a relational database on motor vehicle collisions based on a database from New York City in a span of 8 years in order to help improve traffic safety as well as help manage large-scale data related to traffic incidents. The dataset that we will be looking at is the “Motor Vehicle Collisions - Crashes” dataset which includes police reports on motor vehicle collisions since July 1st of 2012 meaning that we will be covering data only from 2012 to 2020 since the dataset only goes up to 2021. This also means that the dataset is extremely extensive and will require data clean-up as well as reduction for efficient analysis. In order to clean-up and reduce the dataset for analysis, we will observe key attributes, such as location, time/year, point of impact, vehicle make/model, and contributing factors, along with trends and patterns to make the database include only information that is relevant. This will be able to help make the analysis of certain topics, such as yearly leading causes, high-risk areas, high-risk times, and even high-risk car models, easier so that proper and more efficient traffic safety measures can be made according to the information found.
	Motor vehicle collisions pose a significant risk to public safety not only in New York City but also anywhere where vehicles are commonly used. As our group members all frequently drive others as well as long distances, there is always a concern for everyone’s safety especially with the increasing number of drivers around the country. Being able to efficiently analyze data about motor vehicle collisions will offer extremely valuable insights on improving road safety which can lead to many lives being saved including our own. It is also important to note that crash-related data is very sensitive which underscores the importance of handling traffic safety with utmost care and ensuring privacy and security throughout the analysis process.

# Target Audience:
There are many various groups that will be able to utilize our created database with specific goals in mind. For example, law enforcement agencies, such as NYPD, would be able to use the database in order to monitor and analyze traffic-related incidents to improve overall traffic safety and help create a better understanding of factors contributing to accidents which can also mitigate risks. Another group that would be able to use the database would be traffic engineers and urban planners. This group would be able to utilize the database to assess the effectiveness of existing traffic control measures and improve road infrastructure. Even groups such as the media and the general public will be able to utilize the database in order to increase awareness about traffic accidents through a better understanding of traffic patterns and even for educational purposes.

# Potential Entities/Tables:
-Data that identifies the crash. This will be our main table which will help keep track of information about a specific crash together.
  crash_id (Crash ID number)
  crash_date (The day that the crash occurred)
  crash_time (The time that the crash occurred)
-Data about the location of the crash. This information will give us insight on whether a specific location is more accident prone so we can deduct reasons why.
  location_borough (the area in NYC where the collision occurred)
  location_street (the street where the collision occurred)
  location_cross_street (the street perpendicular to the first street listed)
  location_zipcode (zip code of the crash)
-Data about the car that made the report. This information will tell us what type of car was involved in the crash.
  car_id (Car ID number to identify the specific car involved in the crash)
  car_make (what type of car it was)
  car_year (what year the car was manufactured)
  car_state (the state in which the vehicle was registered in)
  car_people (how many people were in the car)
-Data about the driver. This information will be useful in finding patterns about who operates the vehicles that were involved in crashes.
  driver_sex (What the driver chooses to identify as)
  driver_license_status (Whether they are licenced or not)
  drivers_license_jurisdiction (The state that the driver is licenced in)
-Data about the damage that the vehicle sustained. This information will give us insight on how serious the crash was whether it was on the more damaged side or if it is a small dent.
  vehicle_damage (all the damage taken from the collision)
  vehicle_point_of_impact (the initial point of contact between the cars)
  Data about how many people were hurt in the collision. This will include deaths if there were any.
  people_injured (number of people who got injured)
  people_deaths (number of people who died)
-Data about what might have caused the crash.
  contributing_factor (what the driver or passengers were doing that might have caused a crash)
  pre_crash (what the vehicle was doing before the crash)

# Entities/Tables that will not be Included:
-“Public property damage type” will not be included.
  From scrolling through a few thousand rows, I noticed that there are almost none that have this column filled out, and even if they were filled out this is just extra information that won’t help      our database provide what we want it to.
  The same goes for “Public property damage”. I also noticed that the great majority of rows have it filled with ‘N’ or have it blank, so it seems like public property damage isn’t an issue, and it’s    not one of the agendas our database will be working on.
-Travel direction will be left out. I’m sure it’s a useful point of data in other studies, but not in our database. Knowing if a car was traveling north or south isn’t useful for determining patterns    because traveling a certain direction doesn’t impose any harm on its own. 
  As stated in the introduction, we’re only including data from 2012 to 2020. 
  We’ll likely exclude any rows that have 16/25 of its columns empty, since they don’t give any useful information other than “there was a crash somewhere”.

# Sample Data:
	As our topic is listed as one of the three main topics we are allowed to choose from for the summer session of this class, we are using the data set provided on Canvas to survey the information about vehicle collisions. The URL to the list of topics as well as the download link for the database itself is https://umd.instructure.com/courses/1346198/pages/project-topic-areas. However, as this dataset is incredibly large and not yet normalized, it is highly unlikely and rather ineffective to include every single column within the database, and as such we will be filtering and normalizing the data based on the essential pieces of information first. For example, including vehicle and collision information within the database is an absolute must, while extraneous information such as vehicle travel direction can be left out. A more detailed description on what tables we plan to include within the database can be found in the potential tables section of the proposal.

# Questions that the database will answer:
	Some questions our database will be able to answer include, but are not limited to: 
-What are the leading causes of motor vehicle collisions?
-Which vehicle types (make and model) are the most pertinent in motor vehicle collisions?
-Is there a certain time frame where collisions are more likely to occur?
-Is it possible that collisions are more likely to occur at a specific time of year?
-Are older vehicles more prone to collisions than newer vehicles?
-Does the amount of occupants or passengers inside the vehicle affect the likelihood of a collision?
-Does the gender of the driver play a role in the likelihood of collisions?
-Is it possible that license registration of the driver can play a role in defining the cause of vehicle collisions?
-Are vehicles involved in collisions more likely to be hit when stationary or already moving?
-What does the vehicle damage tell us about the nature of the collision?

# Diversity, Equity, and Inclusion Considerations:
	Our database design and sample data plan to be inclusive because it will come from resources that will not involve any biases. As we are collecting data from key attributes, we are looking at features such as location, car makes, etc. We are looking at a dataset that spans from 2012 to 2020 to ensure that the data that we are using is large enough to provide accurate insights into what we are looking for in motor vehicle collisions. In terms of diversity, we are also looking at making sure our data model includes different types of categories involved in the motor vehicle collisions such as pedestrians, cyclists, trucks, and much more. Factors such as gender, race, etc. will also affect traffic safety and traffic collision patterns. With equity, we’ll also be looking at the location and we understand that different locations have a variety of policing practices. Some locations have strict enforcements while others may have less, so we will make sure to look at that and create efforts to validate the reported data.
 
# Data Privacy, Fair Use, Other Ethical Considerations:
	Our design will ensure that data privacy, fair use, and others will be considered. When we are dealing with the data, we will ensure the privacy/security of others such as victims involved within the incident or bystanders that were also involved. We are also aware of the data elements that contain features such as license plate numbers, names of people, along with addresses as well. To also ensure fair use, we will be using and collecting data from police reports and making sure we have the legal right to be able to use that information. We will only be using the data collected from police reports exclusively for education and research purposes. To finalize everything with our design, we will make any of the information that we gather from individuals anonymous and consider data that come from ethical considerations. 
