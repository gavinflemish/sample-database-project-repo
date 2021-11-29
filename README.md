# sample-database-project-repo
## Team Name
### Catawba Crave
## Team Members
### Gavin Fleming, Dawson Brown
## Project Introduction
### With the threat of the Corona virus, food delivery services are more important than ever. Local restaurants are eager to find easy ways to have food delivered to customers without having to hire delivery employees. We will create a database for a campus controlled food delivery service similar to craveoncampus.com. The database will serve as an important data collection source providing valuable information about nutrition and eating habits of campus community members.
## Business Rules
  ### 1)Persons (campus faculty, staff, students) contain personid (PK), name, email, cell, etc.  Faculty conatins title, highest degree, and degreecollege. Staff conatins Position and AdminYorN. Students conatins GradYear and major plus type (undergraduate, graduate). Only faculty, staff and students are included.
  ### 2)Locations for delivery is limited (dorms, student center, and some class buidings). LocationID, LocationName, LocationAddress and (optional) Latitude and Longitude are maintained in the database. The food delivery drop-off point is included with a brief description.
  ### 3)	Persons (may be limited to Students only) can also be drivers (must be approved). Drivers have licensenumber and datehired in the subtype. You may also keep vehicle information (relative to the vehicle that the driver uses).
  ####  a)	Catawba College will start with 8 approved delivery personnel – the system is in test mode.  You can assume all individuals have been cleared and they can be included in the database.
  ####  b)	All delivery personnel are students.
  ### 4)	There is a flat fee of $5 for each delivery. A person orders food one to many times. An individual delivery is tied to one and only one person for the order. The order is for one and only one restaurant. For the items on the order we will only need to keep the total price and delivery charge, along with the driver and delivery times. There should also be a unique identifier (ID) that ties to the id for the order at the individual restaurant. You can assume that the actual items on the order need to come from the restaurant database.
  ### 5)	Food providers must be approved to be included in the database. Ten local restaurants or more will be included for the test database. Information will include an ID, location, schedule, and a link to the restaurant web or social media site along with other possible attributes.
  ### 6)	A rating system will be included in the database. Users will have the choice to rate restaurants and drivers. The rating system will show supertypes and subtypes – an overall rating for the supertype, and subtypes restaurant and driver for ratings for these categories.
  ### 7)	The database will serve as an important data collection source providing valuable information about nutrition and eating habits of campus community members.

## EERD
![EERD2](https://user-images.githubusercontent.com/93001035/141513372-cc781314-e8b3-4175-8456-24249cb9059a.png)


## Data Dictionary
## SQL Code for Queries, Stored Procedures, Views (screen shots)
## Future Work

## UPDATE `campus_eats_fall2021`.`restaurant` SET `location` = '902 E Innes St', `restaurant_name` = 'Chick-fil-A', `schedule` = '6am -10pm', `website` = 'https://www.chick-fil-a.com/' WHERE (`restaurant_id` = '1');
UPDATE `campus_eats_fall2021`.`restaurant` SET `location` = '1020 E Innes St', `restaurant_name` = 'Outback Steakhouse', `schedule` = '11am - 10pm', `website` = 'https://www.outback.com/' WHERE (`restaurant_id` = '2');
UPDATE `campus_eats_fall2021`.`restaurant` SET `location` = '1030 Jake Alexander Blvd W', `restaurant_name` = 'Zaxby\'s Chicken Fingers & Buffalo Wings', `schedule` = '10:30am - 10pm', `website` = 'https://www.zaxbys.com' WHERE (`restaurant_id` = '3');
UPDATE `campus_eats_fall2021`.`restaurant` SET `location` = '1510 W Innes St', `restaurant_name` = 'Romano\'s Italian Cuisine', `website` = 'https://romanos-italian-cuisine.business.site/?m=true' WHERE (`restaurant_id` = '4');
UPDATE `campus_eats_fall2021`.`restaurant` SET `location` = '119 N Link Ave', `restaurant_name` = 'Monterrey Mexican Restaurant', `website` = 'https://monterreymexicanrestaurantnc.com/' WHERE (`restaurant_id` = '5');
UPDATE `campus_eats_fall2021`.`restaurant` SET `location` = '1532 W Innes St', `restaurant_name` = 'L A Murph\'s Fine Cooking', `schedule` = '7am–5:30pm', `website` = 'http://lamurphs.com/' WHERE (`restaurant_id` = '11');
UPDATE `campus_eats_fall2021`.`restaurant` SET `location` = '1804 W Innes St', `restaurant_name` = 'Subway', `schedule` = '9am -7:30pm', `website` = 'https://restaurants.subway.com' WHERE (`restaurant_id` = '12');
UPDATE `campus_eats_fall2021`.`restaurant` SET `location` = '1601 W Innes St', `restaurant_name` = 'Domino\'s Pizza', `schedule` = '10:30am-12am', `website` = 'https://www.dominos.com' WHERE (`restaurant_id` = '13');
UPDATE `campus_eats_fall2021`.`restaurant` SET `location` = '1939 Jake Alexander Blvd W', `restaurant_name` = 'Bojangles', `schedule` = '5am -10pm', `website` = 'https://locations.bojangles.com' WHERE (`restaurant_id` = '14');
