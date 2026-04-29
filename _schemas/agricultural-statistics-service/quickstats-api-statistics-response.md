---
description: Response from the QuickStats api_GET endpoint.
layout: schema
name: Statistics Response
properties_list:
- description: Array of statistics records matching the query.
  name: data
  type: array
provider_name: Agricultural Statistics Service
provider_slug: agricultural-statistics-service
schema_file: json-schema/quickstats-api-statistics-response-schema.json
slug: quickstats-api-statistics-response
source_filename: quickstats-api-statistics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agricultural-statistics-service/refs/heads/main/json-schema/quickstats-api-statistics-response-schema.json\",\n  \"title\": \"Statistics Response\",\n  \"description\": \"Response from the QuickStats api_GET endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StatisticsRecord\"\n      },\n      \"description\": \"Array of statistics records matching the query.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agricultural-statistics-service/refs/heads/main/json-schema/quickstats-api-statistics-response-schema.json
tags:
- Agriculture
- Federal Government
- Statistics
- Open Data
- Geospatial
title: Statistics Response
---
