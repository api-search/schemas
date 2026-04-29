---
description: ''
layout: schema
name: search-deleted-response
properties_list:
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
  name: data
  type: array
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-search-deleted-response-schema.json
slug: oneatlas-search-deleted-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-search-deleted-response-schema.json\",\n  \"title\": \"search-deleted-response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"itemsPerPage\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of requested items per page\",\n      \"example\": 100,\n      \"minimum\": 1\n    },\n    \"startIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"The index of the first item present in the response\",\n      \"example\": 0,\n      \"minimum\": 0\n    },\n    \"totalResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of items present in the catalog\",\n      \"example\": 956126,\n      \"minimum\": 0\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/deleted-item\"\n\
  \      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-search-deleted-response-schema.json
tags:
- Imagery
- Satellites
title: search-deleted-response
---
