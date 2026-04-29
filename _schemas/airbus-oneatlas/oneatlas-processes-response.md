---
description: response to a get processes call.
layout: schema
name: ProcessesResponse
properties_list:
- description: ''
  name: _embedded
  type: object
- description: ''
  name: _links
  type: object
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-processes-response-schema.json
slug: oneatlas-processes-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-processes-response-schema.json\",\n  \"title\": \"ProcessesResponse\",\n  \"type\": \"object\",\n  \"description\": \"response to a get processes call.\",\n  \"properties\": {\n    \"_embedded\": {\n      \"properties\": {\n        \"processes\": {\n          \"items\": {\n            \"$ref\": \"#/components/schemas/processHALCatalog\"\n          },\n          \"type\": \"array\"\n        }\n      },\n      \"type\": \"object\"\n    },\n    \"_links\": {\n      \"properties\": {\n        \"self\": {\n          \"$ref\": \"#/components/schemas/Link\"\n        }\n      },\n      \"type\": \"object\"\n    }\n  },\n  \"required\": [\n    \"_links\",\n    \"_embedded\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-processes-response-schema.json
tags:
- Imagery
- Satellites
title: ProcessesResponse
---
