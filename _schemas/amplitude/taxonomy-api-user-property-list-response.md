---
description: UserPropertyListResponse schema from Amplitude Taxonomy API
layout: schema
name: UserPropertyListResponse
properties_list:
- description: Array of user properties.
  name: data
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/taxonomy-api-user-property-list-response-schema.json
slug: taxonomy-api-user-property-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/taxonomy-api-user-property-list-response-schema.json\",\n  \"title\": \"UserPropertyListResponse\",\n  \"description\": \"UserPropertyListResponse schema from Amplitude Taxonomy API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of user properties.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"user_property\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the user property.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"A description of the user property.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The data type of the property.\"\
  \n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/taxonomy-api-user-property-list-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: UserPropertyListResponse
---
