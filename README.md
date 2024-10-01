# Architecture Challenge
Flightaware24 provides a free iOS and Android application tracking all of the airplane flights in the world.

For this assignment, let's reverse engineer two features in particular on the main view.
* The first is showing a live view of all flights within the bounds of the home screen.
* For the second feature, once selecting a flight, a timeseries history of the route (location, altitude, and airspeed) can be shown, along with some metadata about the flight (Airline, Flight Number, Departing Airport, Arriving Airport, etc.).  Further windows can also show a graph of the timeseries data.

![Home screen](/images/global_view.png)
![Specific flight map](/images/flight_route_map.png)
![Timeseries Graph](/images/timeseries_graph.png)

Please design/reverse engineer how the data pipeline flow works for these two features.  As an input, assume a stream of live data is available for every flight airborne around the world and is providing a sample per flight once every 5 seconds.  All of the data needed is in those streams.  As the output, an HTTP API that the UI polls/pulls from is sufficient.  External customers/clients must be able to access the data without much lag (return in 100's of milliseconds).

The output of this exercise is a design document.  No specific code is required.  Use any methods to convey your design, including any diagrams and/or pseudocode.  Most importantly, please enumerate the reasoning behind specific design, data model, and data storage/query engine choices.  How do you store the data to best match ingest and access patterns?

An important part of the engineering process at Saildrone is a fleshed out design doc that gets reviewed by the team before starting a large project.  This assignment helps us understand your data architecture skills and how you would work/communicate in this environment. 

# Submission
Please submit a pull request to Github with your completed code submission and design document to the private repository set up for you.
