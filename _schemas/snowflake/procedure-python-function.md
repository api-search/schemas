---
description: ''
layout: schema
name: PythonFunction
properties_list:
- description: List of external access integrations attached to this function/procedure
  name: external_access_integrations
  type: array
- description: Secrets to be used with this function/procedure for external access
  name: secrets
  type: object
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/procedure-python-function-schema.json
slug: procedure-python-function
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PythonFunction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"external_access_integrations\": {\n      \"type\": \"array\",\n      \"description\": \"List of external access integrations attached to this function/procedure\"\n    },\n    \"secrets\": {\n      \"type\": \"object\",\n      \"description\": \"Secrets to be used with this function/procedure for external access\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/procedure-python-function-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: PythonFunction
---
