---
description: SearchCriteria schema
layout: schema
name: SearchCriteria
properties_list:
- description: This option allows to exclude the isAllotment flag associated to a booking class in the search response when it exist.
  name: excludeAllotments
  type: boolean
- description: This option allows activate the one-way combinable feature
  name: addOneWayOffers
  type: boolean
- description: Maximum number of flight offers returned (Max 250)
  name: maxFlightOffers
  type: number
- description: maximum price per traveler. By default, no limit is applied. If specified, the value should be a positive number with no decimals
  name: maxPrice
  type: integer
- description: This option allows to default to a standard fareOption if no offers are found for the selected fareOption.
  name: allowAlternativeFareOptions
  type: boolean
- description: Requests the system to find at least one flight-offer per day, if possible, when a range of dates is specified. Default is false.
  name: oneFlightOfferPerDay
  type: boolean
- description: ''
  name: additionalInformation
  type: object
- description: ''
  name: pricingOptions
  type: object
- description: ''
  name: flightFilters
  type: object
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-search-search-criteria-schema.json
slug: flight-offers-search-search-criteria
source_filename: flight-offers-search-search-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-search-criteria-schema.json\",\n  \"title\": \"SearchCriteria\",\n  \"description\": \"SearchCriteria schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"excludeAllotments\": {\n      \"description\": \"This option allows to exclude the isAllotment flag associated to a booking class in the search response when it exist.\",\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"addOneWayOffers\": {\n      \"description\": \"This option allows activate the one-way combinable feature\",\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"maxFlightOffers\": {\n      \"description\": \"Maximum number of flight offers returned (Max 250)\",\n      \"type\": \"number\",\n      \"default\": 250,\n      \"example\": 250\n    },\n    \"maxPrice\"\
  : {\n      \"description\": \"maximum price per traveler. By default, no limit is applied. If specified, the value should be a positive number with no decimals\",\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"allowAlternativeFareOptions\": {\n      \"description\": \"This option allows to default to a standard fareOption if no offers are found for the selected fareOption.\",\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"oneFlightOfferPerDay\": {\n      \"description\": \"Requests the system to find at least one flight-offer per day, if possible, when a range of dates is specified. Default is false.\",\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"additionalInformation\": {\n      \"title\": \"AdditionalInformation\",\n      \"type\": \"object\",\n      \"properties\": {\n        \"chargeableCheckedBags\": {\n          \"description\": \"If true, returns the price of the first additional bag when the airline is an \\\
  \"Amadeus Ancillary Services\\\" member.\",\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"brandedFares\": {\n          \"description\": \"If true, returns the fare family name for each flight-offer which supports fare family\",\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      }\n    },\n    \"pricingOptions\": {\n      \"$ref\": \"#/definitions/Extended_PricingOptions\"\n    },\n    \"flightFilters\": {\n      \"title\": \"FlightFilters\",\n      \"$ref\": \"#/definitions/FlightFilters\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-search-criteria-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: SearchCriteria
---
