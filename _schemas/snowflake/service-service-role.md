---
description: ''
layout: schema
name: ServiceRole
properties_list:
- description: Date and time when the service role was created
  name: created_on
  type: string
- description: Service role name
  name: name
  type: string
- description: Comment, if any, for the service role
  name: comment
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/service-service-role-schema.json
slug: service-service-role
source_filename: service-service-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceRole\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the service role was created\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Service role name\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Comment, if any, for the service role\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/service-service-role-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ServiceRole
---
