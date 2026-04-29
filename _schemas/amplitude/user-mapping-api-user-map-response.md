---
description: UserMapResponse schema from Amplitude User Mapping API
layout: schema
name: UserMapResponse
properties_list:
- description: The HTTP status code of the response.
  name: code
  type: integer
- description: Whether the mapping operation was successful.
  name: success
  type: boolean
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/user-mapping-api-user-map-response-schema.json
slug: user-mapping-api-user-map-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/user-mapping-api-user-map-response-schema.json\",\n  \"title\": \"UserMapResponse\",\n  \"description\": \"UserMapResponse schema from Amplitude User Mapping API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"The HTTP status code of the response.\",\n      \"example\": 200\n    },\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the mapping operation was successful.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/user-mapping-api-user-map-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: UserMapResponse
---
