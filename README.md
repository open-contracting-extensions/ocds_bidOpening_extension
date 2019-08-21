# Bid opening

Adds a bid opening object to describe the date, time, place and details of the bid opening.

## Guidance

## Legal context

In the European Union, this extension's fields correspond to [eForms BT-132, BT-133, BT-134](https://github.com/eForms/eForms). See [OCDS for the European Union](http://standard.open-contracting.org/profiles/eu/master/en/) for the correspondences to Tenders Electronic Daily (TED).

## Example

```json
{
  "tender": {
    "bidOpening": [
      {
        "dateTime": "2019-10-16T15:00:00+01:00",
        "address": {
          "postalCode": "OX1 1BX",
          "countryName": "United Kingdom",
          "streetAddress": "Town Hall, St Aldate's",
          "region": "Oxfordshire",
          "locality": "Oxford"
        },
        "location": {
          "geometry": {
            "type": "Point",
            "coordinates": [51.751944, -1.257778]
          },
          "gazetteer": {
            "scheme": "GEONAMES",
            "identifiers": ["2640729"]
          },
          "description": "Central Oxford",
          "uri": "http://www.geonames.org/2640729/oxford.html"
        },
        "details": "We recommend that people who wish to attend the opening register on this page: https://wwww.example.org/register"
      }
    ]
  }
}
```

## Issues

Report issues for this extension in the [ocds-extensions repository](https://github.com/open-contracting/ocds-extensions/issues), putting the extension's name in the issue's title.
