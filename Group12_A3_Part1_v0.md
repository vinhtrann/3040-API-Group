## API Description
An API for developers to retrieve Winnipeg Transit information

## Endpoints
GET arrival time
/api/arrivalTime
- Parameters
    - Bus Number
    - Bus stop number

GET available capacity
/api/availableSeats
- Parameters
    - License plate

GET number of stops on the route
/api/numStops
- Parameters
    - Route number 

## Resources

## Sample

```
{
    "results": {
        "arrivalTime": "VAL"
    },
    "status": "OK"
}
```

```
{
    "results": {
        "availableSeats": "VAL"
    },
    "status": "OK"
}
```

```
{
    "results": {
        "numStops": "VAL"
    },
    "status": "OK"
}
```