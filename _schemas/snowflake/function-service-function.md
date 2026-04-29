---
description: Service based function
layout: schema
name: ServiceFunction
properties_list:
- description: Function's endpoint
  name: endpoint
  type: string
- description: Function's path
  name: path
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/function-service-function-schema.json
slug: function-service-function
source_filename: function-service-function-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceFunction\",\n  \"type\": \"object\",\n  \"description\": \"Service based function\",\n  \"properties\": {\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"Function's endpoint\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Function's path\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/function-service-function-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ServiceFunction
---
