<h3>Michael Ippolito<br />
CUNY DATA621<br />
Blog #5</h3>
<br />
<h3>Background</h3>
<br />
Since I'm spending the fall in Toulouse, France, I wanted to get a sense of what kind of city I'm living in. Tolouse is the fourth largest city in France (after Paris, Marseille, and Lyon), with a population of about 433,000 in 2022. It is home to Airbus and has a significant industrial and technical community, as well as many expatriates. As an urban center, it isn't surprising that it is overwhelminingly democratic in terms of politics. For this blog post, I wanted to investigate this quantitatively. The city of Toulouse maintains an excellent and extensive collection of data sets about a range of topics, many of which I found useful for this post (https://data.toulouse-metropole.fr/explore/).<br />
<br />
To put some boundaries on scope, I focussed on trying to predict percentage of votes during the second round of the 2022 presidential elections for the Toulouse metropolitan area. In France, the presidential elections are held in two rounds, akin to the primary and general elections in the United States. For predictors, I used a subset of this data, along with fifty other data sets I downloaded from the same site:<br />
<br />

| Predictor |
|-----------|
| accelerators_incubators |
| agricultural_zones |
| art_galleries |
| bicycle_parking |
| bicycle_rentals |
| bowling_alleys |
| business_centers |
| cafe_concert_venues |
| canal_sites |
| carpool_stations |
| cemeteries |
| community_fitness_centers |
| cultural_centers |
| dog_parks |
| dog_waste_bags |
| dumps |
| elementary_schools |
| flood_zones_1875 |
| game_libraries |
| green_spaces |
| gymnasiums |
| institutes_of_cultural_instruction |
| lakes |
| libraries |
| markets |
| museums |
| park_and_rides |
| pedestrian_zones |
| playgrounds |
| pools |
| presidential_election_billboards |
| public_toilets |
| recharging_stations |
| regulation_offices |
| scooter_rentals |
| senior_restaurants |
| skate_parks |
| skating_rinks |
| social_centers |
| sociocultural_centers |
| speed_displays |
| stadiums |
| taxi_zones |
| tennis)courts |
| theaters |
| tramway_stations |
| vaccination_centers |
| wifi_zones |
| workers_rights_centers |

<br />
Each data set includes geographic coordinates (latitude and longitude) that I used to calculate how far each entity is away from each polling station. Then I took the median distance of all the entites in each category to feed into a binary logistic regression model to predict the percentage of the vote each candidate would get.<br />

[Link to full PDF](https://github.com/mmippolito/cuny_data621_blog5/blob/main/blog5.pdf)
