---
description: location information
layout: schema
name: Location
properties_list:
- description: date and time specified in the [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-DDThh:mm:ss format e.g. 2017-11-10T10:00:00 not supported for stopOvers object
  name: dateTime
  type: string
- description: airport code from [IATA table codes](http://www.iata.org/publications/Pages/code-search.aspx), e.g. CDG.
  name: locationCode
  type: string
- description: internal airport identifier used for private jets and helicopters e.g. IT87100
  name: lfiCode
  type: string
- description: ''
  name: address
  type: object
- description: Place name e.g. Airport Name, Hotel Name etc.
  name: name
  type: string
- description: Google place id only for google address e.g. ChIJL-DOWeBv5kcRfTbh97PimNc.
  name: googlePlaceId
  type: string
- description: UIC code defined by the worldwide railway organization e.g. 8600626
  name: uicCode
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-search-location-schema.json
slug: transfer-search-location
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Location\",\n  \"description\": \"location information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dateTime\": {\n      \"type\": \"string\",\n      \"description\": \"date and time specified in the [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-DDThh:mm:ss format e.g. 2017-11-10T10:00:00\\nnot supported for stopOvers object\\n\"\n    },\n    \"locationCode\": {\n      \"type\": \"string\",\n      \"description\": \"airport code from [IATA table codes](http://www.iata.org/publications/Pages/code-search.aspx), e.g. CDG.\"\n    },\n    \"lfiCode\": {\n      \"type\": \"string\",\n      \"description\": \"internal airport identifier used for private jets and helicopters e.g. IT87100\"\n    },\n    \"address\": {\n      \"$ref\": \"#/definitions/Address\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Place name e.g. Airport Name, Hotel Name etc.\"\
  \n    },\n    \"googlePlaceId\": {\n      \"type\": \"string\",\n      \"description\": \"Google place id only for google address e.g. ChIJL-DOWeBv5kcRfTbh97PimNc.\"\n    },\n    \"uicCode\": {\n      \"type\": \"string\",\n      \"description\": \"UIC code defined by the worldwide railway organization e.g. 8600626\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-search-location-schema.json
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
title: Location
---
