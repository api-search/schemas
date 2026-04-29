---
description: Schema representing an API available on the APILayer marketplace
layout: schema
name: APILayer API
properties_list:
- description: Unique identifier for the API
  name: id
  type: string
- description: Name of the API
  name: name
  type: string
- description: Description of the API and its capabilities
  name: description
  type: string
- description: Category of the API (e.g., Geolocation, Currency, Weather)
  name: category
  type: string
- description: Base URL for API requests
  name: baseURL
  type: string
- description: URL to the API documentation
  name: documentationURL
  type: string
- description: Authentication details for the API
  name: authentication
  type: object
- description: Available subscription plans for this API
  name: plans
  type: array
- description: Tags describing the API
  name: tags
  type: array
provider_name: APILayer
provider_slug: apilayer
schema_file: json-schema/apilayer-api-schema.json
slug: apilayer-api
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apilayer/main/json-schema/apilayer-api-schema.json\",\n  \"title\": \"APILayer API\",\n  \"description\": \"Schema representing an API available on the APILayer marketplace\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the API\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the API\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the API and its capabilities\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category of the API (e.g., Geolocation, Currency, Weather)\"\n    },\n    \"baseURL\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Base URL for API requests\"\n    },\n    \"documentationURL\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the API documentation\"\n    },\n    \"authentication\": {\n      \"type\": \"object\",\n      \"description\": \"Authentication details for the API\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"apikey\", \"bearer\"],\n          \"description\": \"Authentication type\"\n        },\n        \"headerName\": {\n          \"type\": \"string\",\n          \"description\": \"Header name for API key authentication\"\n        }\n      }\n    },\n    \"plans\": {\n      \"type\": \"array\",\n      \"description\": \"Available subscription plans for this API\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": { \"type\": \"string\" },\n          \"monthlyRequests\": { \"type\": \"integer\" },\n          \"pricePerMonth\": { \"type\": \"number\" }\n        }\n      }\n    },\n    \"tags\": {\n  \
  \    \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Tags describing the API\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"description\", \"category\", \"baseURL\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apilayer/refs/heads/main/json-schema/apilayer-api-schema.json
tags:
- API Catalog
- API Discovery
- API Marketplace
- Developer Tools
- SaaS APIs
title: APILayer API
---
