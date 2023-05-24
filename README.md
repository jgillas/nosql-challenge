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

That was the output of my code which shows one of the documents with a hygiene score equal to 20. The next picture is the output of the Pandas DataFrame I created to show the data easier: 

  <img width="1075" alt="Question 1 Panada DF" src="https://github.com/jgillas/nosql-challenge/assets/125215083/3375fa2d-e593-4dec-9564-3027bf6b2e11">

There are 41 rows of data which means that there are 41 different establishments which have a hygiene score equal to 20. 

The second question is which establishments in London have a RatingValue greater than or equal to 4? The answer to the question is below: 

  <img width="723" alt="Question 2 Find One" src="https://github.com/jgillas/nosql-challenge/assets/125215083/5ddfb4a1-a92f-4425-b312-b94506438428">

That was the output of my code which shows one of the documents with a RatingValue greater than or equal to 4. In this case this output has a RatingValue of 4. The next picture is the output of the Pandas DataFrame I created to show the data easeir: 

  <img width="1070" alt="Question 2 Pandas DF" src="https://github.com/jgillas/nosql-challenge/assets/125215083/7855950a-c969-49bd-bbca-e29a05ed0368">

There are 33 rows of data which means there are 33 different establishments in London with a RatingValue greater than or equal to 4. 

The third question is What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"? The answer to the question is below: 

  <img width="630" alt="Question 3 Output" src="https://github.com/jgillas/nosql-challenge/assets/125215083/086bf7d7-79d7-4d26-9925-61323ea1b816">

This output is just one of the top 5 establishments with a RatingValue of 5 nearest to the new restaurant which was added. The rest of the establishments are listed below below but could not all be fit into the photo. Please see the code itself for all 5 of the establishments. The next picture is the output of the Pandas DataFrame I created so that all 5 establishments could be seen easier: 

  <img width="1075" alt="Question 3 Pandas DF" src="https://github.com/jgillas/nosql-challenge/assets/125215083/54e20b9e-1713-45f2-bd6b-e6af7db85772">

Here you can see all 5 establishments listed out. These are the top 5 establishments with a RatingValue of 5 sorted by lowest hygiene score and nearest to the new restaurant added, "Penang Flavours". 

The forth and final question is How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas. The answer to this question is below: 

  <img width="365" alt="Question 4 Output" src="https://github.com/jgillas/nosql-challenge/assets/125215083/354d6a72-937b-422c-98aa-0655d6ab7506">

There are 55 rows in this results which means there are 55 Local Authority areas with establishments that have a hygiene score of 0. Next to each Local Authority there is a count of how many establishments have a hygiene score of 0 in that Local Authority. The next picture shows the output of the Pandas DataFrame I created so that you can see the top 10 Local Authorties with the count of establishments which have a hygiene score of 0 next to them: 

  <img width="397" alt="Question 4 Pandas DF" src="https://github.com/jgillas/nosql-challenge/assets/125215083/dbd1372e-7c67-488b-9d97-3e38b7b69f54">

This completes the module 12 challenge. 
