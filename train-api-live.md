
## TRAIN API ROUTES & URI 


## BASE URI 

[https://trainbackend.cooliewale.in/api/]([https://trainbackend.cooliewale.in/api/])

## PNR

To get details about Passengers PNR use 

Usage 

https://trainbackend.cooliewale.in/api/getPNRinfo?={pnr} 

Example 

SAMPLE PNR : 6137174078

[https://trainbackend.cooliewale.in/api//getPNRinfo?pnr=6137174078](https://trainbackend.cooliewale.in/api/getPNRinfo?pnr=6137174078)


will retrive details like Pnr,TrainNo,TrainName,Date of journey,Coach position of passenger,train coach arrangement

```
 "Pnr": "6137174078",
  "TrainNo": "15232",
  "TrainName": "GONDIA BJU EXP",
  "InformationMessage": null,
  "Doj": "01-07-2024",
  "BookingDate": "12-06-2024",
  "Quota": "GN",
  "DestinationDoj": "02-07-2024",
  "SourceDoj": "30-06-2024",
  "From": "USL",
  "To": "MFP",
  "ReservationUpto": "MFP",
  "BoardingPoint": "USL",
  "Class": "2A",
  "ChartPrepared": false,
  "BoardingStationName": "Usalapur",
  "TrainStatus": "",
  "TrainCancelledFlag": false,
  "ReservationUptoName": "Muzaffarpur Junction",
  "PassengerCount": 4,
  "PassengerStatus":{},
  "coachposition",
"DepartureTime": "02:40",
  "ArrivalTime": "05:00",
  "ExpectedPlatformNo": "2",
  "BookingFare": "8100",
  "TicketFare": "8100",
  "CoachPosition": "L SLR GS GS S11 S10 S9 S8 S7 S6 S5 S4 S3 S2 S1 B3 B2 B1 A1 AB1 GS GS GS SLR",
  "Rating": 2.8,
  "FoodRating": 2.6,
  "PunctualityRating": 2.9,
  "CleanlinessRating": 2.9,
  "SourceName": "Bilaspur",
  "DestinationName": "Muzaffarpur",
  "Duration"

```


## LIVE TRAIN 

To obtain Live Train  STatus 

USAGE 

https://trainbackend.cooliewale.in/api/liveTrainInfo?trainNo?={train_number}&date{date-of-journey}

[https://trainbackend.cooliewale.in/api/liveTrainInfo?trainNo=12382&date=28-06-2024](https://trainbackend.cooliewale.in/api/liveTrainInfo?trainNo=12382&date=28-06-2024)

or

[https://trainbackend.cooliewale.in/api/liveTrainInfo?trainNo=12382&date=28-JUN-2024](https://trainbackend.cooliewale.in/api/liveTrainInfo?trainNo=12382&date=28-JUN-2024)

will retrive LIve Train STatus for TRain number : 12382, Train Name : Poorva Express   of 28th June with 

```
route:{},
current :{},
live status:{}

```
where route displays the route of the train,current  displays where the train is presently at and live status which station  it will pass,when, haspassed or not, time , arrival,departure,delay and intermediate stations in between   



If a train doesnt run that day it will be unable to retrive the live train status 



## TRAIN ROUTE 

To get the TRain Route of a particular Train 

USAGE 
https://trainbackend.cooliewale.in/api/getRoute?trainNo={train_number}

Example 

[https://trainbackend.cooliewale.in/api/getRoute?trainNo=18612](https://trainbackend.cooliewale.in/api/getRoute?trainNo=18612)

will retrive the train route 


## Train Info 

To get a general information about a train use 

USAGE 
https://trainbackend.cooliewale.in/api/getTrainInfo?trainNo={train_number}

Example 

[https://trainbackend.cooliewale.in/api/getTrainInfo?trainNo=18612](https://trainbackend.cooliewale.in/api/getTrainInfo?trainNo=18612)

will retrive trainnumber,trainname,duration,fromstation,to station




## Train Between Station 

To get Trains running from STATION to Station 

USAGE 

https://trainbackend.cooliewale.in/api/getTrainOnDate?from={from}&to={to}


Example 

[https://trainbackend.cooliewale.in/api/getTrainOnDate?from=NDLS&to=BSBS](https://trainbackend.cooliewale.in/api/?from=NDLS&to=BSBS)

will retrieve all trains  running between NEW DELHI (NDLS) & BANARAS (BSBS)


## Train On Date 

To get Trains running between stations on a particular day 


USAGE 

https://trainbackend.cooliewale.in/api/getTrainOnDate?from={from}&to={to}&date=date


Example 

[https://trainbackend.cooliewale.in/api/getTrainOnDate?from=NDLS&to=BSBS&date=30-06-2024](https://trainbackend.cooliewale.in/api/?from=NDLS&to=BSBS&date=30-06-2024)

will retrieve all trains  running between NEW DELHI (NDLS) & BANARAS (BSBS) on date 30-06-2024










****
