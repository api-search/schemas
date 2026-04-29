---
description: PublicAccessTokenResponse schema from Airbyte API
layout: schema
name: PublicAccessTokenResponse
properties_list:
- description: ''
  name: access_token
  type: string
- description: ''
  name: token_type
  type: object
- description: ''
  name: expires_in
  type: integer
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-public-access-token-response-schema.json
slug: airbyte-public-access-token-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-public-access-token-response-schema.json\",\n  \"title\": \"PublicAccessTokenResponse\",\n  \"description\": \"PublicAccessTokenResponse schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\"\n    },\n    \"token_type\": {\n      \"enum\": [\n        \"Bearer\"\n      ]\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  },\n  \"required\": [\n    \"access_token\",\n    \"token_type\",\n    \"expires_in\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-public-access-token-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: PublicAccessTokenResponse
---
