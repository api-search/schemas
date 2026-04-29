---
description: ''
layout: schema
name: update-options
properties_list:
- description: ''
  name: query
  type: object
- description: ''
  name: update
  type: object
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-update-options-schema.json
slug: oneatlas-update-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-update-options-schema.json\",\n  \"title\": \"update-options\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"$ref\": \"#/components/schemas/search-options\"\n    },\n    \"update\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"expirationDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Date of deletion of the data in the platform and deletion of the\\nmetadata item if no other production status is defined.\\n\",\n          \"example\": \"2017-08-29T00:00:00Z\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-update-options-schema.json
tags:
- Imagery
- Satellites
title: update-options
---
