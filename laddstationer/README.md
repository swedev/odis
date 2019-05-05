# Mockup, formulär för input av laddstationer

Motsvarar data i följande spreadsheet:

https://drive.google.com/file/d/1ezMOBtLGCt_CvUrlYoz2OeArOfb8_C2O/view

#### Förslag på dataformat, JSON
Detta är Work In Progress.

```json
{
  "name": "Min station",
  "owner": "Elentusiasterna AB",
  "email": "matte@elentusiasterna.se",
  "location": {
    "address": "Elgatan 12 B",
    "postalCode": "123 45",
    "type": "Publik",
    "description": "Genom porten, till höger.",
    "gps": {
      "latitude": 81.2307,
      "longitude": 21.9302
    }
  },
  "hoursOpen": {
    "from": 7,
    "to": 21,
    "description": "Helgfria vardagar"
  },
  "hasTimeLimit": true,
  "timeLimitDescription": "max 2 h",
  "payment": {
    "hasChargingFee": true,
    "chargingFeeDescription": "2kr/kwh",
    "methods": [
      "Kort",
      "SMS",
      "App"
    ]
  },
  "hasParkingFee": false,
  "other": {
    "hasRealTimeInfo": true,
    "realTimeInfoDescription": "Vattenfalls InCharge",
    "subsidy": "Klimatklivet",
    "general": "För support ring 0701-234567"
  }
}
```
