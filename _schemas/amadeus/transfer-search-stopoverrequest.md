---
description: ''
layout: schema
name: StopOverRequest
properties_list:
- description: the intermediate stop duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M
  name: duration
  type: string
- description: the intermediate stop airport IATA code, e.g. CDG. Location could be defined either using location code or address (address line, zip code, country code, city, geo code)
  name: locationCode
  type: string
- description: the intermediate stop street address including building number, e.g. 5 Avenue Anatole France
  name: addressLine
  type: string
- description: the intermediate stop country, the location with [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) format (e.g. US)
  name: countryCode
  type: string
- description: the intermediate stop city name, e.g. Paris
  name: cityName
  type: string
- description: the intermediate stop postal/zip code, e.g. 75007
  name: zipCode
  type: string
- description: the intermediate stop google place id only for google address e.g. ChIJL-DOWeBv5kcRfTbh97PimNc.
  name: googlePlaceId
  type: string
- description: the intermediate stop name e.g. Airport Name, Hotel Name etc.
  name: name
  type: string
- description: the intermediate stop internal airport identifier used for private jets and helicopters e.g. IT87100
  name: lfiCode
  type: string
- description: the intermediate stop state code according to [ISO 3166-2](https://en.wikipedia.org/wiki/ISO_3166-2)
  name: stateCode
  type: string
- description: the intermediate stop latitude and longitude of geographical location following the structure {latitude},{longitude} e.g. 48.858093,2.294694
  name: geoCode
  type: string
- description: sequence number of the stop e.g. 3
  name: sequenceNumber
  type: number
- description: UIC code defined by the worldwide railway organization e.g. 8600626
  name: uicCode
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-search-stopoverrequest-schema.json
slug: transfer-search-stopoverrequest
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: StopOverRequest
---
