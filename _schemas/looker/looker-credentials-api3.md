---
description: API3 client credentials for a user
layout: schema
name: CredentialsApi3
properties_list:
- description: Unique identifier
  name: id
  type: integer
- description: API3 client ID
  name: client_id
  type: string
- description: Timestamp when these credentials were created
  name: created_at
  type: string
- description: Whether these credentials are disabled
  name: is_disabled
  type: boolean
- description: Credential type
  name: type
  type: string
- description: Relative URL
  name: url
  type: string
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-credentials-api3-schema.json
slug: looker-credentials-api3
source_filename: looker-credentials-api3-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CredentialsApi3\",\n  \"type\": \"object\",\n  \"description\": \"API3 client credentials for a user\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier\"\n    },\n    \"client_id\": {\n      \"type\": \"string\",\n      \"description\": \"API3 client ID\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when these credentials were created\"\n    },\n    \"is_disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether these credentials are disabled\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Credential type\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Relative URL\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-credentials-api3-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: CredentialsApi3
---
