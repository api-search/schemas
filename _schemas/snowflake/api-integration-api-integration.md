---
description: A Snowflake API integration object.
layout: schema
name: ApiIntegration
properties_list:
- description: Name of the API integration.
  name: name
  type: string
- description: A comma-separated list of endpoints and resources that Snowflake can access.
  name: api_allowed_prefixes
  type: array
- description: A comma-separated list of endpoints and resources that are not allowed to be called from Snowflake.
  name: api_blocked_prefixes
  type: array
- description: Whether the API integration is enabled.
  name: enabled
  type: boolean
- description: Comment for the API integration.
  name: comment
  type: string
- description: Date and time when the API integration was created.
  name: created_on
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/api-integration-api-integration-schema.json
slug: api-integration-api-integration
source_filename: api-integration-api-integration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApiIntegration\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake API integration object.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the API integration.\"\n    },\n    \"api_allowed_prefixes\": {\n      \"type\": \"array\",\n      \"description\": \"A comma-separated list of endpoints and resources that Snowflake can access.\"\n    },\n    \"api_blocked_prefixes\": {\n      \"type\": \"array\",\n      \"description\": \"A comma-separated list of endpoints and resources that are not allowed to be called from Snowflake.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the API integration is enabled.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Comment for the API integration.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Date and time when the API integration was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/api-integration-api-integration-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ApiIntegration
---
