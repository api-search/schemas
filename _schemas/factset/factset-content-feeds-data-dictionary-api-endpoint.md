---
description: ''
layout: schema
name: ApiEndpoint
properties_list:
- description: Unique identifier for the api endpoint
  name: id
  type: string
- description: API endpoint path
  name: name
  type: string
- description: A description of the endpoint
  name: description
  type: string
- description: Developer Portal URL of the endpoint
  name: developerPortalLink
  type: string
- description: Flag indicating if the user is entitled to access the data in their subscriptions
  name: entitled
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-content-feeds-data-dictionary-api-endpoint-schema.json
slug: factset-content-feeds-data-dictionary-api-endpoint
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApiEndpoint\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the api endpoint\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"API endpoint path\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the endpoint\"\n    },\n    \"developerPortalLink\": {\n      \"type\": \"string\",\n      \"description\": \"Developer Portal URL of the endpoint\"\n    },\n    \"entitled\": {\n      \"type\": \"string\",\n      \"description\": \"Flag indicating if the user is entitled to access the data in their subscriptions\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-content-feeds-data-dictionary-api-endpoint-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ApiEndpoint
---
