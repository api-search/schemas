---
description: Resources related to the API key.
layout: schema
name: APIKeyRelationships
properties_list:
- description: ''
  name: created_by
  type: object
- description: ''
  name: modified_by
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-api-api-key-relationships-schema.json
slug: datadog-api-api-key-relationships
source_filename: datadog-api-api-key-relationships-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-api-api-key-relationships-schema.json\",\n  \"title\": \"APIKeyRelationships\",\n  \"description\": \"Resources related to the API key.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"created_by\": {\n      \"$ref\": \"#/components/schemas/RelationshipToUser\"\n    },\n    \"modified_by\": {\n      \"$ref\": \"#/components/schemas/NullableRelationshipToUser\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-api-api-key-relationships-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: APIKeyRelationships
---
