## API Description
An API for developers to retrieve precise and live Winnipeg Transit information. Including information and location for all nearby bus stops. 

## Endpoints
GET arrival time  
/api/arrivalTime
- Parameters
    - **busNum** (int): The number of the bus (required)
    - **stopNum** (int): The number of the stop (required)

GET available capacity  
/api/availableSeats
- Parameters
    - **plateNum** (String): The bus' registered license plate number (required)

GET number of stops on the route  
/api/numStops
- Parameters
    - **routeNum** (int): The bus' route number (required)

## Resources


GET arrival time  
```
{
    "results": {
        "arrivalTime": "5:35:23 PM"
    },
    "status": "OK"
}
```


GET available capacity  
```
{
    "results": {
        "availableSeats": 10
    },
    "status": "OK"
}
```


GET number of stops on the route  
```
{
    "results": {
        "numStops": 15
    },
    "status": "OK"
}
```

## Sample Request

```
https://ourtransit.wpg/api/arrivaltime?busNum=10&stopNum=50
```

Sample response:
```
{
    "results": {
        "arrivalTime": "1:42:49 PM"
    },
    "status": "OK"
}
```

```
https://ourtransit.wpg/api/numStops?routeNum=75
```

Sample response:
```
{
    "results": {
        "numStops": "28"
    },
    "status": "OK"
}
```
