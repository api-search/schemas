---
description: ''
layout: schema
name: Securable
properties_list:
- description: Database name of the securable if applicable.
  name: database
  type: string
- description: Schema name of the securable if applicable.
  name: schema
  type: string
- description: Service name of the securable if applicable.
  name: service
  type: string
- description: Name of the securable if applicable.
  name: name
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/role-securable-schema.json
slug: role-securable
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Securable\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"database\": {\n      \"type\": \"string\",\n      \"description\": \"Database name of the securable if applicable.\"\n    },\n    \"schema\": {\n      \"type\": \"string\",\n      \"description\": \"Schema name of the securable if applicable.\"\n    },\n    \"service\": {\n      \"type\": \"string\",\n      \"description\": \"Service name of the securable if applicable.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the securable if applicable.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/role-securable-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Securable
---
