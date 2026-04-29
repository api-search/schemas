---
description: A USDA AMS market news office.
layout: schema
name: Office
properties_list:
- description: Unique identifier for the office.
  name: office_id
  type: string
- description: Name of the market news office.
  name: name
  type: string
- description: City where the office is located.
  name: city
  type: string
- description: State where the office is located.
  name: state
  type: string
- description: List of commodities covered by this office.
  name: commodities
  type: array
provider_name: Agricultural Marketing Service
provider_slug: agricultural-marketing-service
schema_file: json-schema/mars-api-office-schema.json
slug: mars-api-office
source_filename: mars-api-office-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/json-schema/mars-api-office-schema.json\",\n  \"title\": \"Office\",\n  \"description\": \"A USDA AMS market news office.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"office_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the office.\",\n      \"example\": \"NAT\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the market news office.\",\n      \"example\": \"National\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City where the office is located.\",\n      \"example\": \"Washington\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State where the office is located.\",\n      \"example\": \"DC\"\n    },\n    \"commodities\": {\n      \"type\": \"\
  array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of commodities covered by this office.\",\n      \"example\": [\n        \"Cattle\",\n        \"Hogs\",\n        \"Dairy\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/json-schema/mars-api-office-schema.json
tags:
- Agriculture
- Federal Government
- Market News
- Livestock
- Dairy
- Fruits And Vegetables
- Cotton
- Tobacco
title: Office
---
