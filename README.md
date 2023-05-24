# nosql-challenge

This assignment was split into two different pieces. There was the setup code and then the analysis code. The first thing I did was setup all the information. 

The first thing I did was import the establishments.json file and I named the database uk_food and the collection establishments. The code I used to import the data is below: 

  mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json
  
I made sure that it was imported correctly and I assigned the establishments collection toa variable to prepare the collection to be used. 

After this setup I went on to update the database. The first thing I did was add the new restaurant to the database. The new restaurant code is listed below: 

  <img width="737" alt="SetUp: New Restaurant" src="https://github.com/jgillas/nosql-challenge/assets/125215083/945bfd52-4715-4cf0-8155-3b428f336749">

I then found the BusinessTypeID for "Restaurant/Cafe/Canteen" and then updated the new restaurant with the BusinessTypeID I found. The updated code for the new restaurant is listed below: 

  <img width="725" alt="New Restaurant Updated" src="https://github.com/jgillas/nosql-challenge/assets/125215083/6c0e704c-4a3f-4ece-ba31-5862c3540088">

