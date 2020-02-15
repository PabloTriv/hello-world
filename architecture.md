Program Organization
===
First Two Levels of the C4 Diagram Model:

![](https://www.ucf.edu/files/2016/08/florida-gold-ucf-pin.png)




In the first level of the diagram, the user, highlighted in green, accesses the website to view parking availability and travel times from the garage the user desires to park in to his or her class. The website, represented by a blue square, indicating it is software being developed, uses two existing software systems: Google Maps and UCF Parking Services. The user is able to view parking availability on the website when that information is retrieved from UCF Parking Services. Additionally, the user is able to view travel times on the website, which uses Google Maps to provide that information.
The second level of the diagram, the user, highlighted in green, visits http://my.ucfparkingmap.wtf/ to view park space and travel times. The software, which is represented by the large, square outline, is represented at this level by two parts. Firstly, the Web Application portion, which is made in HTML, is where the user views parking availability and travel times. This portion also retrieves information from UCF Parking Services. The Web Application makes calls to the Google Maps API, which provides travel times and a route to class.


[Relation to User Stories](https://docs.google.com/spreadsheets/d/1M_ln6ihm26gYYpeJPvi5UznOYSBsz13smrJnPS2PgDU/edit?usp=sharing) based
on the Level 2 of the C4 Diagram above.

Major Classes
===
[Filter and Building class diagram](https://www.lucidchart.com/invitations/accept/ca94d761-6e0c-4333-9405-95fb87ec8580)
This diagram shows the links between the filter that is put over the UCF map and the buildings, garages, and route that users will be able to see.

[Class Descriptions](https://docs.google.com/document/d/1QSI1F7FovfD75h76nOl4Rfxur2yqmRN8nwEtyDUsk1o/edit?usp=sharing)

| ID | User Story | Related Class | Explanation |
|----|------------|--------|----------|
| 000 | As someone who parks at UCF, I want to see parking availability so I know which garage to park in. | Garage | Garage has a field that says how many spots are full and a method that calculates the percentage of spots taken.|
| 001 | As someone who parks at UCF, I want to see the walk time to my class so that I know when to leave. | Route, Building | Building  has a field that describes its location. Route then uses this information to give a walk time estimate.|
| 002 | As someone who parks at UCF, I want to know the bike time to class so that I know when to leave. | Route, Building | Building has a field that describes its location. Route then uses this information to give a bike time.|
| 003 | As someone who parks at UCF, I want to see a garage's peak hours so I know the best time to park. | Garage | Each garage will keep track of its peak hours. |
| 004 | As someone who parks at UCF, I want to know a route to my classroom so I can reduce my travel time. | Route | The Route class gives finds a route between to locations. |
| 005 | As someone who parks at UCF, I want to see a map of campus that shows me the buildings and garages so I can navigate the campus. | Filter, Building | Filter and Building contribute to what you see on the map. Filter shows how full a garage is by color-coding it and displays the route. Building highlights classrooms on the map which is part of the HTML code. |
| 006 | As someone who parks at UCF, I want to be able to tell a garage's fullness from a color label so that it's more clear from a glance. | Filter | The Filter class is what displays the colors that dictate how full a garage is.|
| 007 | As someone who parks at UCF, I want to know where I parked so that I don't forget. | Garage | The Garage class can store information about where the user parked.|
| 008 | As someone who parks at UCF, I want to know how many spots are left in a garage so I can determine if I can find a spot. | Garage | The Garage class keeps track of how many spots are open and how many spots are occupied, as well as the percentage of spots taken.|
| 009 | As someone who parks at UCF, I want to know which garages I can park in with my specific parking pass so that I don't get a parking ticket. | Garage | The Garage class keeps track of which parking passes are required to park in it. |
| 010 | As someone who parks at UCF, I want to be able to load the website in a web browser so I can check parking from any device. | - | This functionality is dependent on the website and HTML code.|
| 011 | As someone who uses the parking map, I want to be able to select a building or parking garage so that I can see more information and potential interactions | Building, Garage | The Building and Garage classes provide information about themselves, such as how full it is if it is a garage, and where it is if it is a building.|
| 012 | As someone who uses the parking map, I want to be able to contact the developer so that improvements can be made to the application (or to express my deepest gratitude) | - | This feature will be controlled by the website.|

Data Design
===
Data will be stored in a database using Firebase, if needed.

Business Rules
===

User Interface Design
===
[User Interface Diagram](https://docs.google.com/drawings/d/16DPH29ViC9o1byNa-bV2rYDFJ4SD3fNrLsuwYscEsiA/edit?usp=sharing)

[User Interface Description](https://docs.google.com/document/d/1NbHeXcBzvRX_gwZu9qL7QONij4zAqkXUbm0EJtyyrIs/edit?usp=sharing)

[Related User Stories](https://docs.google.com/spreadsheets/d/176kv5p055fJC5ESXw7EtPdeijBrr9F2iLoWR1RY9rsE/edit?usp=sharing)

Resource Management
===

Security
===

Performance
===

Scalability
===

Interoperability
===

Internationalization/Localization
===

Input/Output
===

Error Processing
===

Fault Tolerance
===

Architectural Feasibility
===

Overengineering
===

Build-vs-Buy Decisions
===

Reuse
===

Change Strategy
===
