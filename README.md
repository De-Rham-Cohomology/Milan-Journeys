# Milan-Journeys
How faster is it to travel by car vs public transport in Milan? To try and answer this I created a (relatively small) sample of possible A to B travels and kept track of the time taken.

Each datapoint (A to B travel) is built as following:

1. Draw two random points in a rectangle containing Milan.
2. Reverse geocode the points using the free [Big Data Cloud API](https://www.bigdatacloud.com/), gather information about their location.
3. Keep the points if in Milan.
4. Generate a random departure date and time. The year is 2021.
5. Calculate the fastest drive from A to B using [TomTom API](https://developer.tomtom.com/).
6. Calculate the fastest public transport journey from A to B using [HERE API](https://developer.here.com/).

The usage of different APIs is due to the limited number of daily queries available to a free user (the most limitating being TomTom API with 2500 daily queries).
This method is probably not the fastest out there but gets the job done. More, my hardware at the moment is quite limited, so a few thousands of observations is the maximum I can handle.


