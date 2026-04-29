---
description: ''
layout: schema
name: Location
properties_list:
- description: Location identifier
  name: id
  type: string
- description: Facility name
  name: name
  type: string
- description: Facility type
  name: type
  type: string
- description: Country code (ISO 3166-1 alpha-2)
  name: country
  type: string
- description: State or region
  name: state
  type: string
- description: City
  name: city
  type: string
- description: Geographic latitude
  name: latitude
  type: number
- description: Geographic longitude
  name: longitude
  type: number
provider_name: Archer Daniels Midland
provider_slug: archer-daniels-midland
schema_file: json-schema/archer-daniels-midland-commodity-data-api-location-schema.json
slug: archer-daniels-midland-commodity-data-api-location
source_filename: archer-daniels-midland-commodity-data-api-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Location identifier\",\n      \"example\": \"ADM-DEC-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Facility name\",\n      \"example\": \"Decatur Processing Complex\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Facility type\",\n      \"enum\": [\n        \"processing-plant\",\n        \"grain-elevator\",\n        \"distribution-center\",\n        \"port\"\n      ],\n      \"example\": \"processing-plant\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country code (ISO 3166-1 alpha-2)\",\n      \"example\": \"US\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State or region\",\n      \"example\": \"IL\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City\",\n      \"example\": \"\
  Decatur\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"description\": \"Geographic latitude\",\n      \"example\": 39.8403\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"description\": \"Geographic longitude\",\n      \"example\": -88.9548\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/json-schema/archer-daniels-midland-commodity-data-api-location-schema.json\",\n  \"title\": \"Location\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/json-schema/archer-daniels-midland-commodity-data-api-location-schema.json
tags:
- Agriculture
- Food Processing
- Commodities
- Supply Chain
- Fortune 100
- Nutrition
title: Location
---
