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

[Related User Stories](https://docs.google.com/spreadsheets/d/1k7q2BV7jlDt9QNjrzUYfFlQOx1ptZoENrk4T_eiTI3E/edit?usp=sharing)

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
