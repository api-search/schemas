---
description: ''
layout: schema
name: HotelSentiment
properties_list:
- description: Amadeus Hotel Ids are found in the Hotel Search response (parameter name is 'hotelId')
  name: hotelId
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: overallRating
  type: object
- description: ''
  name: numberOfRatings
  type: integer
- description: ''
  name: numberOfReviews
  type: integer
- description: Dictionary containing scores for all the available categories. If a property does not have any category this object will not be present in the response.
  name: sentiments
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-ratings-hotelsentiment-schema.json
slug: hotel-ratings-hotelsentiment
source_filename: hotel-ratings-hotelsentiment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelSentiment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hotelId\": {\n      \"type\": \"string\",\n      \"description\": \"Amadeus Hotel Ids are found in the Hotel Search response (parameter name is 'hotelId')\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"overallRating\": {\n      \"$ref\": \"#/definitions/Score\"\n    },\n    \"numberOfRatings\": {\n      \"type\": \"integer\"\n    },\n    \"numberOfReviews\": {\n      \"type\": \"integer\"\n    },\n    \"sentiments\": {\n      \"type\": \"object\",\n      \"description\": \"Dictionary containing scores for all the available categories.  If a property does not have any category this object will not be present in the response.\",\n      \"properties\": {\n        \"sleepQuality\": {\n          \"$ref\": \"#/definitions/Score\"\n        },\n        \"service\": {\n          \"$ref\": \"#/definitions/Score\"\n\
  \        },\n        \"facilities\": {\n          \"$ref\": \"#/definitions/Score\"\n        },\n        \"roomComforts\": {\n          \"$ref\": \"#/definitions/Score\"\n        },\n        \"valueForMoney\": {\n          \"$ref\": \"#/definitions/Score\"\n        },\n        \"catering\": {\n          \"$ref\": \"#/definitions/Score\"\n        },\n        \"swimmingPool\": {\n          \"$ref\": \"#/definitions/Score\"\n        },\n        \"location\": {\n          \"$ref\": \"#/definitions/Score\"\n        },\n        \"internet\": {\n          \"$ref\": \"#/definitions/Score\"\n        },\n        \"pointsOfInterest\": {\n          \"$ref\": \"#/definitions/Score\"\n        },\n        \"staff\": {\n          \"$ref\": \"#/definitions/Score\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"hotelId\",\n    \"overallRating\",\n    \"avgHotelAvailabilityResponseTime\",\n    \"numberOfRatings\",\n    \"numberOfReviews\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-ratings-hotelsentiment-schema.json
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
title: HotelSentiment
---
