---
description: ''
layout: schema
name: ActivitySearchResponse
properties_list:
- description: ''
  name: data
  type: array
- description: Number of requested items per page
  name: itemsPerPage
  type: number
- description: The index of the first item present in the response
  name: startIndex
  type: number
- description: The total number of activities
  name: totalResults
  type: number
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-activity-search-response-schema.json
slug: oneatlas-activity-search-response
source_filename: oneatlas-activity-search-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-activity-search-response-schema.json\",\n  \"title\": \"ActivitySearchResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Activity\"\n      },\n      \"type\": \"array\",\n      \"uniqueItems\": true\n    },\n    \"itemsPerPage\": {\n      \"description\": \"Number of requested items per page\",\n      \"example\": 100,\n      \"format\": \"integer\",\n      \"minimum\": 1,\n      \"type\": \"number\"\n    },\n    \"startIndex\": {\n      \"description\": \"The index of the first item present in the response\",\n      \"example\": 0,\n      \"format\": \"integer\",\n      \"minimum\": 0,\n      \"type\": \"number\"\n    },\n    \"totalResults\": {\n      \"description\": \"The total number of activities\",\n \
  \     \"example\": 582,\n      \"format\": \"integer\",\n      \"maximum\": 10000,\n      \"minimum\": 0,\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-activity-search-response-schema.json
tags:
- Imagery
- Satellites
title: ActivitySearchResponse
---
