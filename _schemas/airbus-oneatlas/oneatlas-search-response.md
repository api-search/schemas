---
description: ''
layout: schema
name: SearchResponse
properties_list:
- description: ''
  name: error
  type: boolean
- description: ''
  name: features
  type: array
- description: Number of requested items per page
  name: itemsPerPage
  type: integer
- description: The index of the first item present in the response
  name: startIndex
  type: integer
- description: The total number of items present in the catalog
  name: totalResults
  type: integer
- description: ''
  name: type
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-search-response-schema.json
slug: oneatlas-search-response
source_filename: oneatlas-search-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-search-response-schema.json\",\n  \"title\": \"SearchResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"example\": false,\n      \"type\": \"boolean\"\n    },\n    \"features\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CatalogItem\"\n      },\n      \"type\": \"array\"\n    },\n    \"itemsPerPage\": {\n      \"description\": \"Number of requested items per page\",\n      \"example\": 100,\n      \"minimum\": 1,\n      \"type\": \"integer\"\n    },\n    \"startIndex\": {\n      \"description\": \"The index of the first item present in the response\",\n      \"example\": 0,\n      \"minimum\": 0,\n      \"type\": \"integer\"\n    },\n    \"totalResults\": {\n      \"description\": \"The total number of items present in the catalog\",\n   \
  \   \"example\": 956126,\n      \"maximum\": 10000,\n      \"minimum\": 0,\n      \"type\": \"integer\"\n    },\n    \"type\": {\n      \"example\": \"FeatureCollection\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-search-response-schema.json
tags:
- Imagery
- Satellites
title: SearchResponse
---
