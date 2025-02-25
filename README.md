# Google-Maps-Clone

This is a clone version of the Google Maps. which has been made as a debut project. This project doesn't particularly solve any problems but gives us a basic approach to anchor the confidence of building out something.  
As this was my debut project made in 2021, the github account associated with it, has been deauthenticated and decomposed over the period of time. Luckily, I had backed up this source code in my hardrive, which made it possible to serve the possible neceessity. 

**This code is not in the status of operation*, but optimized enough to analyze and assess the computation behind each functionality. 
**
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Aim of the Project:** This projects aims to ease the client/user, by computing the "Shortest Route", "The Fuel Efficient Route", "The Appropiate Arrival Time at the Destination". In short, it provides some essential information like distance, travel time and turn-to-turn instruction. 

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Algorithm Used: **The Dijkstra's algorithm**

It's well-suited for finding the shortest paths in graphs with non-negative edge weights, making it a suitable choice for this route finding application

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Key Components Used:**

**GeoApiContext** - To configure the Google Maps API client with credentials.

**getLatLng** - Takes Address and Input & uses Geocoding API to convert address into real-time coordinates as LatLng object.

**getDistanceMatrix** - Takes the orgin and destination LatLng as input and compute the distance and travel time. And return DistanceMatrix Object containing information

**getDirections** - Takes orgin & destination LatLng as the input and with the help of Directions API it retrives the driving routes, which includes waypoints and turn-to-turn instruction. Returns back DirectonResult object

**parseRoute** - It combines the information from DistanceMatrix & DirectionResult. Also extracts relevant data like distance, duration, status, waypoints and instruction. Returns a Route object containing all the information.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Key Improvements:**

**Combined API Calls** - Merged Distance Matrix and Directions API calls for efficiency.

**Removed Unnecessary Features** - Removed the alternate route calculation as it was not well-implemented and added complexity.

**Added waypoints and turn-by-turn instructions** to the output.

**Improved readability** with formatted distance and duration.

**Meaningful Variable Names** - Used more descriptive variable names for better code clarity.

**Removed Redundant Code** - Removed unused code blocks.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**Key Considerations:**

API Usage Limits 

Error Handling

Caching 

Asynchronous Requests 
