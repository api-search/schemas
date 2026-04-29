---
description: ''
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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-search-searchcriteria-schema.json
slug: flight-offers-search-searchcriteria
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"SearchCriteria\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"excludeAllotments\": {\n      \"type\": \"boolean\",\n      \"description\": \"This option allows to exclude the isAllotment flag associated to a booking class in the search response when it exist.\"\n    },\n    \"addOneWayOffers\": {\n      \"type\": \"boolean\",\n      \"description\": \"This option allows activate the one-way combinable feature\"\n    },\n    \"maxFlightOffers\": {\n      \"type\": \"number\",\n      \"description\": \"Maximum number of flight offers returned (Max 250)\"\n    },\n    \"maxPrice\": {\n      \"type\": \"integer\",\n      \"description\": \"maximum price per traveler. By default, no limit is applied. If specified, the value should be a positive number with no decimals\"\n    },\n    \"allowAlternativeFareOptions\": {\n      \"type\": \"boolean\",\n      \"description\": \"This option allows to\
  \ default to a standard fareOption if no offers are found for the selected fareOption.\"\n    },\n    \"oneFlightOfferPerDay\": {\n      \"type\": \"boolean\",\n      \"description\": \"Requests the system to find at least one flight-offer per day, if possible, when a range of dates is specified. Default is false.\"\n    },\n    \"additionalInformation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"chargeableCheckedBags\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, returns the price of the first additional bag when the airline is an \\\"Amadeus Ancillary Services\\\" member.\"\n        },\n        \"brandedFares\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, returns the fare family name for each flight-offer which supports fare family\"\n        }\n      }\n    },\n    \"pricingOptions\": {\n      \"$ref\": \"#/definitions/Extended_PricingOptions\"\n    },\n    \"flightFilters\": {\n      \"$ref\": \"\
  #/definitions/FlightFilters\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-search-searchcriteria-schema.json
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
title: SearchCriteria
---
