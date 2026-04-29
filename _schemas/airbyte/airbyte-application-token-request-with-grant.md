---
description: ApplicationTokenRequestWithGrant schema from Airbyte API
layout: schema
name: ApplicationTokenRequestWithGrant
properties_list:
- description: ''
  name: client_id
  type: string
- description: ''
  name: client_secret
  type: string
- description: ''
  name: grant-type
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-application-token-request-with-grant-schema.json
slug: airbyte-application-token-request-with-grant
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-application-token-request-with-grant-schema.json\",\n  \"title\": \"ApplicationTokenRequestWithGrant\",\n  \"description\": \"ApplicationTokenRequestWithGrant schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"client_id\": {\n      \"type\": \"string\"\n    },\n    \"client_secret\": {\n      \"type\": \"string\"\n    },\n    \"grant-type\": {\n      \"enum\": [\n        \"client_credentials\"\n      ]\n    }\n  },\n  \"required\": [\n    \"client_id\",\n    \"client_secret\",\n    \"grant_type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-application-token-request-with-grant-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: ApplicationTokenRequestWithGrant
---
