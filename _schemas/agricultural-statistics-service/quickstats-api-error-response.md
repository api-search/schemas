---
description: Error response from the QuickStats API.
layout: schema
name: Error Response
properties_list:
- description: Error type or description.
  name: error
  type: string
- description: Human-readable error message.
  name: message
  type: string
provider_name: Agricultural Statistics Service
provider_slug: agricultural-statistics-service
schema_file: json-schema/quickstats-api-error-response-schema.json
slug: quickstats-api-error-response
source_filename: quickstats-api-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agricultural-statistics-service/refs/heads/main/json-schema/quickstats-api-error-response-schema.json\",\n  \"title\": \"Error Response\",\n  \"description\": \"Error response from the QuickStats API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error type or description.\",\n      \"example\": \"too many results\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message.\",\n      \"example\": \"The request would return more than 50,000 records. Please narrow your query.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agricultural-statistics-service/refs/heads/main/json-schema/quickstats-api-error-response-schema.json
tags:
- Agriculture
- Federal Government
- Statistics
- Open Data
- Geospatial
title: Error Response
---
