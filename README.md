# nosql-challenge

This assignment was split into two different pieces. There was the setup code and then the analysis code. The first thing I did was setup all the information. 

The first thing I did was import the establishments.json file and I named the database uk_food and the collection establishments. The code I used to import the data is below: 

  mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json
  
I made sure that it was imported correctly and I assigned the establishments collection toa variable to prepare the collection to be used. 

After this setup I went on to update the database. The first thing I did was add the new restaurant to the database. The new restaurant code is listed below: 

  <img width="737" alt="SetUp: New Restaurant" src="https://github.com/jgillas/nosql-challenge/assets/125215083/945bfd52-4715-4cf0-8155-3b428f336749">

I then found the BusinessTypeID for "Restaurant/Cafe/Canteen" and then updated the new restaurant with the BusinessTypeID I found. The updated code for the new restaurant is listed below: 

  <img width="725" alt="New Restaurant Updated" src="https://github.com/jgillas/nosql-challenge/assets/125215083/6c0e704c-4a3f-4ece-ba31-5862c3540088">

The thing I did was that I found how many documents contianed the Dover Local Authority. I found that there were 994 documents that contained the Dover Local Authority. I then removed all these doucments which contained Dover Local Authority. I checked and made sure they were all removed and they were. The last thing I did with the setup code is that I needed to update some of the strings to be numbers because they were stored incorrectly. I converted latitude and longitude to decimal numbers and I converted RatingValue to an integer number. 

This completes the setup code and I now moved to the analysis code where I answer four questions using the data I imported and cleaned up in the setup code. 

The first question was Which establishments have a hygiene score equal to 20? The answer to the quesiton is below: 

  <img width="662" alt="Question 1 Output" src="https://github.com/jgillas/nosql-challenge/assets/125215083/dced39a5-93fc-44e0-8646-aa26467fd0db">
