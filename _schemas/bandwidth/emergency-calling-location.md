---
description: A validated physical location for E911 emergency routing
layout: schema
name: Location
properties_list:
- description: The unique identifier for the location
  name: locationId
  type: string
- description: A description of the location
  name: description
  type: string
- description: ''
  name: address
  type: object
- description: The validation status of the location
  name: status
  type: string
- description: The latitude coordinate of the location
  name: latitude
  type: number
- description: The longitude coordinate of the location
  name: longitude
  type: number
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/emergency-calling-location-schema.json
slug: emergency-calling-location
source_filename: emergency-calling-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/emergency-calling-location-schema.json\",\n  \"title\": \"Location\",\n  \"description\": \"A validated physical location for E911 emergency routing\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"locationId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the location\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the location\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"houseNumber\": {\n          \"type\": \"string\",\n          \"description\": \"The house or building number\"\n        },\n        \"houseSuffix\": {\n          \"type\": \"string\",\n          \"description\": \"The house number suffix (e.g., A, B, 1/2)\"\n        },\n        \"prefixDirectional\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The street prefix directional (N, S, E, W)\"\n        },\n        \"streetName\": {\n          \"type\": \"string\",\n          \"description\": \"The street name\"\n        },\n        \"streetSuffix\": {\n          \"type\": \"string\",\n          \"description\": \"The street suffix (St, Ave, Blvd, etc.)\"\n        },\n        \"postDirectional\": {\n          \"type\": \"string\",\n          \"description\": \"The street post directional (N, S, E, W)\"\n        },\n        \"addressLine2\": {\n          \"type\": \"string\",\n          \"description\": \"Secondary address line (suite, floor, etc.)\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"The city name\"\n        },\n        \"stateCode\": {\n          \"type\": \"string\",\n          \"description\": \"The two-letter state code\"\n        },\n        \"zip\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The five-digit ZIP code\"\n        },\n        \"plusFour\": {\n          \"type\": \"string\",\n          \"description\": \"The ZIP+4 extension\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"The country code\"\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"VALID\",\n        \"INVALID\",\n        \"GEOCODED\"\n      ],\n      \"description\": \"The validation status of the location\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The latitude coordinate of the location\"\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The longitude coordinate of the location\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/emergency-calling-location-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Location
---
