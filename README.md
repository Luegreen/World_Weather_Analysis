# World_Weather_Analysis
Using Google Places API, Open Weather API, Jupyter notebook, Python, Pandas make hotel recommendations for >500 global cities

## Using the various APIs to collect random cities from around the world, then parse them into weather patterns, and then decide, based on weather, what hotel is nearest to the city and ultimattely plan a route. 

Collect random cities from random lat/long and then tap into cityPy, then gather the city's weather form OpenWeatherMap: 
<img width="792" alt="Screen Shot 2021-05-25 at 11 23 40 AM" src="https://user-images.githubusercontent.com/14239715/119524921-11479480-bd4c-11eb-8497-b9c63006bfdf.png">


Next step: Find a hotel that is close to the city...
<img width="811" alt="Screen Shot 2021-05-25 at 11 24 00 AM" src="https://user-images.githubusercontent.com/14239715/119525370-713e3b00-bd4c-11eb-8d78-04ebf299ddba.png">



And then, pick some weather that you enjoy


<img width="568" alt="Screen Shot 2021-05-25 at 11 30 18 AM" src="https://user-images.githubusercontent.com/14239715/119525571-9cc12580-bd4c-11eb-8ad7-bce5bebc84d2.png">



and map the available hotels within that weather frame:
<img width="787" alt="Screen Shot 2021-05-25 at 9 02 24 AM" src="https://user-images.githubusercontent.com/14239715/119525613-a5196080-bd4c-11eb-81e4-d19038b568d7.png">


Finally; To chose a trip and chart the route. I chose Sierra Lionne... for a nice bike trip. <img width="790" alt="WeatherPy_travel_map" src="https://user-images.githubusercontent.com/14239715/119525978-f75a8180-bd4c-11eb-9020-05670eae46fe.png">

And, here is where I'll stay:
<img width="774" alt="WeatherPy_travel_markers" src="https://user-images.githubusercontent.com/14239715/119526017-00e3e980-bd4d-11eb-8009-f95cfaae8e96.png">


## Challenges
There are maximum call volume to various APIs so after having been locked out of OpenWeatherMap I was warry to try new code to that api. Unfortunately, when my code threw errors I assumed it was my getting locked out again. Finally after a couple of days of still not getting through, I disabled my Try: Except: clause and began to find the code errors that were stopping me the second time around. 

Each next ten or so steps held a challenge, one of the final ones was my series for lat, long for my four Sierra Lionne destination hotels was not reading correctly into the mapping function. The print of the series looked fine but the error code was a TraitError, ([[ #### ####]])not a valid location. Locations have length of 2. I noticed that the comma was disappearing. I finally realized after taking away the double brackets and receiving a 'cannot unpack non-iterable numpy.float64 object that the problem was that I needed to call the index value. After trying this in the lists themselves, I finally called the index value in the code and it worked. 


