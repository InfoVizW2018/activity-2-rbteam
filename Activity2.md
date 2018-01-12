# InfoViz Activity 2
By Randy Cho, Baylee Munro

## Design
**As per the activity description, Seaspan desires…**
* The ability to adapt their schedule based on current load information
* Manual control over the schedule
* A visual way to examine possible schedules

![Design](https://i.imgur.com/de2Yz9y.png)

We have designed a 2D “Live Map” interface with mouse-over functionality that provides information. Our design includes a map encompassing all Seaspan routes, as included in the data package. In our sample, we have provided two sample berths as well as a ferry en route.

**With this design, we can see:**
* What each vessel is doing, and when
* How full each vessel is
* When each berth is occupied / free

We assume that what was categorized as “most important” as per the activity description should be most clearly highlighted. We are assuming that this LiveMap could be dynamically generated based on a table of Sailings (like what we were provided) and that this data could be modified to produce effective visualizations of scheduling through our tool. Additionally, routes could be “moved” using our program to generate a new table document. This allows manual control of the schedule, while examining possible new schedules using visual methods and existing data.

The map of Vancouver Island and the mainland was drawn using the following image as a reference: http://seniors101.ca/wp-content/uploads/2011/05/island_map.gif

## What-Why-How
### What
The initial dataset used for this design is a ferry schedule consisting of multiple weekly tables categorized by two locations: Surrey and Tilbury. The dataset also includes three routes: Surrey-Nanaimo, Tilbury-Swartz Bay, and Tilbury-Nanaimo. The dataset includes a categorical attribute type such in the vessel identifier and a sequentially ordered, cyclic, attribute type in departure/arrival times. Through our LiveMap design, we have taken these attributes and combined them with a linear measure of time to create a rich, spatial representation of our information.

### Why
The purpose of the design is to provide users at Seaspan a flexible design that encompasses the key requirements previously described in activity description. Users intending to analyze data in this visualization are primarily going to be consuming existing information provided by the design. The LiveMap aims to present an otherwise originally static schedule to a dynamic and interactive tool that communicates the dataset to the end user. With this design, it is also possible to produce new data by editing routes and generating new schedules. Another action which a user may take is searching; each location in the the LiveMap is a known factor, which simply requires a user to browse or lookup a specific route/vessel in the visualization. Succeeding the search action, the user needs to identify arrival and departure times of a given route, determine remaining capacity of a vessel at a berth, or compare times between them. Finally, actions must correspond to targets; illustrated by paths or routes taken by a vessel, or the vessel/berth itself. 

### How
Actions are achieved by arranging data in a way where elements are indicated as separate entities on the LiveMap. Differentiation between categorical data such as routes, berths, and vessels are identified by mapping them to their individual colors. Vessels are given a distinct shape, and routes are represented in motion with dotted lines.

## Design Study Methodology
To put the Design Study Methodology into practice for this task, the first step would be to analyze the domain in further detail in order to design a relevant visualization solution that solves a real world problem. To do this, direct interaction with Seaspan and potential users who would be interacting with the visualization will be necessary in order to have a clearer understanding and context on the broad requirements provided in this activity. Considering various alternative solutions to visualizing Seaspan’s schedule is important as we don’t know whether or not the “Live Map” interface is the most optimal solution for visualizing the current dataset. Collaboration with users to test the visualization is necessary in validating the solution and ensuring it meets key criteria such as capacity load, and displaying what each vessel is doing at a given time. Iterations of the design ties into reflection; making improvements over various aspects to fit these requirements better.

## Study Pitfalls

A few potential pitfalls that we could encounter are:
* **(PF-3) Premature commitment to collaboration**  
In the winnowing step, collaborating with too many users early may cause confusion in the design stage

* **(PF-14) Mistaking fellow tool builders for real end users**  
In the activity description, it isn’t clear as to who the design is for: employees at Seaspan or passengers looking to board a vessel. Need to make sure that the audience is well-established.

* **(PF-17) Experts focusing on visualization design vs domain problem**  
The design is currently very focused around the visualization more so than the domain problem itself; this requires more communication with Seaspan  

* **(PF-23) Usability too much/ too little**  
There may be too large of a focus on usability and less on practicality and effectiveness of the visualization

