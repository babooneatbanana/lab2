# Proximity of Public Schools to fast buses and skytrain stops in Vancouver

Map link: https://babooneatbanana.github.io/lab2/lab2-index.html

This map aims to help parents decide where to send their children to school, assuming they value the transit accessibility of the public school in relation to where they live. By helping parents make informed decision, children are more likely to participate in public transportation which is safe and good for the environment. This map was created by me entirely on my own. The map user selects a buffer size and clicks on a location (in theory their home). Then any school, bus, or skytrain within the buffer appears with full opacity. Additionally, the nearest school, bus, and skytrain appear as larger circles. 

### Datasets

This map uses three datasets. The first contains the location public schools in the City of Vancouver. It was accessed from the Vancouver Open Data Portal. The second dataset contains the location of skytrain stops in the City of Vancouver. It was access from the Vancouver Open Data Portal as well. The third dataset contains the location of all R4, R5, and 99 b-line bus stops in the City of Vancouver. To prevent bus stops at the same intersection that go eastward and westward from appearing as two distinct stops, I selected the major street the bus goes to as one stop. For example, both the eastbound and westbound r4 arriving at Cambie St, stop at the same stop. A user will ultimately go to this intersection regardless of the direction they take the R4. I made this dataset in geojson.io. 

### Stylization

The base map is stylized as OpenStreetMap positron. This provides lots of information for users and allows them to easily locate their home. However, it does not stand out too much and remains in the background. 

I chose to stylize the points when initially loaded on the screen with low opacity because before the user as selected a location, no point is particularly important. Public schools were stylized as an orangey brown. Bus stops and skytrain stops were stylized as green and blue because these seem fitting for the sustainable vibe of public transportation. 

To indicate importance, nearest points and points within the buffer receive full opacity. Nearest points also receive a larger circle radius. Indicating importance this way shows which publics and transit stops should be of note for the user given the location they have selected. 

The results of the nearest points and points within the buffer are transferred to the console and then displayed on the html page so that a user can see the output. 

### Learning process

This lab largely drew from coding and cartographic techniques learned in class like buffer, point, nearest point. This used turf.js. I also looked up in a few websites and forum different methods I could use to display the console on the screen. This led me to few websites and forums that showed various methods for display information in html. In total, I spent roughly ten hours on this lab, making constant gradually changes to the display methods. 

There is one big thing I tried to do but failed at doing. That was creating a legend. I made a simply sketch in p5.js and tried to display it over the map window but I could not find a way to prevent it from going below the map. 
This is the legend I created in p5.js.
<img width="718" height="591" alt="image" src="https://babooneatbanana.github.io/lab2/legend.png" />

### Area of Interest


### Critique

