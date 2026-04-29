---
description: Standard error response.
layout: schema
name: ErrorResponse
properties_list:
- description: Error code.
  name: cod
  type: integer
- description: Error message.
  name: message
  type: string
provider_name: Agromonitoring
provider_slug: agromonitoring
schema_file: json-schema/agromonitoring-errorresponse-schema.json
slug: agromonitoring-errorresponse
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.agromonitoring.com/schemas/ErrorResponse.json\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Standard error response.\",\n  \"properties\": {\n    \"cod\": {\n      \"type\": \"integer\",\n      \"description\": \"Error code.\",\n      \"example\": 401\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message.\",\n      \"example\": \"Invalid API key.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agromonitoring/refs/heads/main/json-schema/agromonitoring-errorresponse-schema.json
tags:
- Agriculture
- Satellite Imagery
- Vegetation Indices
- Weather
- Precision Agriculture
- Remote Sensing
title: ErrorResponse
---
