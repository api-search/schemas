---
description: Request body for starting a protected query.
layout: schema
name: StartProtectedQueryRequest
properties_list:
- description: The type of the protected query.
  name: type
  type: string
- description: The parameters for the SQL type protected query.
  name: sqlParameters
  type: object
- description: Contains configuration details for protected query results.
  name: resultConfiguration
  type: object
provider_name: Amazon Clean Rooms
provider_slug: amazon-clean-rooms
schema_file: json-schema/clean-rooms-start-protected-query-request-schema.json
slug: clean-rooms-start-protected-query-request
source_filename: clean-rooms-start-protected-query-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-start-protected-query-request-schema.json\",\n  \"title\": \"StartProtectedQueryRequest\",\n  \"description\": \"Request body for starting a protected query.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SQL\"\n      ],\n      \"description\": \"The type of the protected query.\"\n    },\n    \"sqlParameters\": {\n      \"type\": \"object\",\n      \"description\": \"The parameters for the SQL type protected query.\",\n      \"properties\": {\n        \"queryString\": {\n          \"type\": \"string\",\n          \"description\": \"The query string to be submitted.\"\n        }\n      }\n    },\n    \"resultConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Contains configuration details\
  \ for protected query results.\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"resultConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-start-protected-query-request-schema.json
tags:
- AWS
- Clean Rooms
- Data Collaboration
- Privacy
- Analytics
- Marketing
title: StartProtectedQueryRequest
---
