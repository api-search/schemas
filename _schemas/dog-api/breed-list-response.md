---
description: Response envelope for the master breed list.
layout: schema
name: BreedListResponse
properties_list:
- description: Map of breed name to a list of sub-breed names.
  name: message
  type: object
- description: ''
  name: status
  type: string
provider_name: Dog API
provider_slug: dog-api
schema_file: json-schema/breed-list-response.json
slug: breed-list-response
source_filename: breed-list-response.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dog-api/refs/heads/main/json-schema/breed-list-response.json\",\n  \"title\": \"BreedListResponse\",\n  \"description\": \"Response envelope for the master breed list.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"object\",\n      \"description\": \"Map of breed name to a list of sub-breed names.\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": { \"type\": \"string\" }\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"success\", \"error\"]\n    }\n  },\n  \"required\": [\"message\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dog-api/refs/heads/main/json-schema/breed-list-response.json
tags:
- Dogs
- Images
- Open Data
- Open Source
title: BreedListResponse
---
