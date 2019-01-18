# nearby

A Map of Restaurants and and other Locations next to the Office.

## Contribution
- Add a Location in [GeoJson Format](http://geojson.org/) (<http://geojson.io>).
- Make a pull request

### Example

```json
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "properties": {
        "Name": "SysEleven GmbH",
        "Address": "Boxhagener Straße 80, 10247 Berlin",
        "Website": "https://www.syseleven.de",
        "Description": "SysEleven Office",
        "Type": "Office",
        "Rating": "10/10 (1 Vote)"
      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          13.467392921447754,
          52.508008383200306
        ]
      }
    }
  ]
}
```

### Properties

| Property      | Description           | Values  |
| ------------- |-------------			| -----|
| Name 			| Name of the Location 	| eg: `SysEleven GmbH` |
| Address      	| Adress 				| eg: `Boxhagener Straße 80, 10247 Berlin` |
| Website      	| Location Website      |   eg: `www.syseleven.de` |
| Description 	| short Description     |    eg: `SysEleven Office, good Coffee nice talks` |
| Type 			| Location Type      	|    `Office`, `Restaurant.*`, `Bank` |
| Rating 		| Rate the Location. From 1 to 10 Points. Increase the number of Votes and calculate the Rating `($old_vote + $your_vote)/2`| `5.5/10 (10 Votes)` |
