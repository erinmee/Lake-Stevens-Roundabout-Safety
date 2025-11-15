# Data retrieval process

## Washington State Patrol Collision Analysis tool
https://fortress.wa.gov/wsp/collisionanalysistool/

Individual collision reports are filled out by state patrol officers. The collision location is described by a primary and secondary trafficway. Since the data comes from reports filled out by individuals there are various ways a trafficway is named, i.e. highway 9 is called *SR 9*, *SR 009*, *SR 9 NE*, etc... 

In order to query the database for all accidents at the roundabouts, the variations in naming need to be accounted for so that all accidents are included.

The collision analysis tool has a map feature I used to explore the various namings for the trafficways of interest. I queried for crashes in Lake Stevens from 1/1/2015 to 11/15/2025 to find the following variations on naming.

### State Route 9 Variations
* SR 9
* SR 9 NE
* SR9
* SR9 NE
* SR N9 NE
* STATE ROUTE 9 NE
* STATE ROAD 9
* SR-9 NE
* SR-9
* HWY 9

### State Route 204 Variations
* SR 204
* SR204
* STATE ROUTE 204
* SR-204
* HWY 204
* SR 204 NE

### Vernon Road Variations
* VERNON
* VERNON RD
* VERNON ROAD

### N Davies Road Variations
* N DAVIS RD
* NORTH DAVIS ROAD
* N. DAVIES RD
* N DAVIES ST

### Frontage Road Variations
* FRONTAGE RD

### 7th Pl NE Variations
* 7TH PL NE
* 7TH ST NE

| Trafficway pairs |  |
| --- | --- |
| SR 9 | SR 204 |
| SR 9 | N Davies Rd |
| SR 9 | Vernon Rd |
| SR 9 | 7th Pl NE |
| SR 9 | Frontage Rd |
| SR 204 | Vernon Rd |
| N Davies Rd | Frontage Rd |
| N Davies Rd | Vernon Rd |
| 900 BLK* | SR 9 NE |

## Queries used to generate the dataset

For all of these queries start date was 1/1/201 12:00AM and end date was 11/15/2025 12:00AM. County was Snohomish and City was Lake Stevens.

|Primary trafficway | Secondary trafficway |
| --- | --- |
| SR 9 | SR 204 |
| 

![WSDOT map of roundabout plan](https://wsdot.wa.gov/sites/default/files/styles/max_650x650/public/2021-06/SR9-SR204-Project-Map-Overview.png?itok=yv8xhW5Y)

![Image of ](https://wsdot.wa.gov/sites/default/files/2024-01/SR9SR204Project-Photo-FinalRoundabouts_0.PNG)
