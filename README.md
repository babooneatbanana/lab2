# Proximity of Public Schools to fast buses and skytrain stops in Vancouver

Map link: https://babooneatbanana.github.io/lab2/lab2-index.html

This map aims to help parents decide where to send their children to school, assuming they value the transit accessibility of the public school in relation to where they live. By helping parents make informed decision, children are more likely to participate in public transportation which is safe and good for the environment. This map was created by me entirely on my own. The map user selects a buffer size and clicks on a location (in theory their home). Then any school, bus, or skytrain within the buffer appears with full opacity. Additionally, the nearest school, bus, and skytrain appear as larger circles. 

### Datasets

This map uses three datasets. The first contains the location public schools in the City of Vancouver. It was accessed from the Vancouver Open Data Portal. The second dataset contains the location of skytrain stops in the City of Vancouver. It was access from the Vancouver Open Data Portal as well. The third dataset contains the location of all R4, R5, and 99 b-line bus stops in the City of Vancouver. To prevent bus stops at the same intersection that go eastward and westward from appearing as two distinct stops, I selected the major street the bus goes to as one stop. For example, both the eastbound and westbound r4 arriving at Cambie St, stop at the same stop. A user will ultimately go to this intersection regardless of the direction they take the R4. I made this dataset in geojson.io. 

### Stylization

The base map is stylized as OpenStreetMap positron. This provides lots of information for users and allows them to easily locate their home. However, it does not stand out too much and remains in the background. 

I chose to stylize the points when initially loaded on the screen with low opacity because before the user as selected a location, no point is particularly important.  
