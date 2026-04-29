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
- description: 'Specifies the Python version to use. The supported versions of Python are: * 3.8 * 3.9 * 3.10 * 3.11'
  name: runtime_version
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/user-defined-function-python-function-schema.json
slug: user-defined-function-python-function
source_filename: user-defined-function-python-function-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PythonFunction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"external_access_integrations\": {\n      \"type\": \"array\",\n      \"description\": \"List of external access integrations attached to this function/procedure\"\n    },\n    \"secrets\": {\n      \"type\": \"object\",\n      \"description\": \"Secrets to be used with this function/procedure for external access\"\n    },\n    \"runtime_version\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the Python version to use. The supported versions of Python are:\\n                        * 3.8\\n                        * 3.9\\n                        * 3.10\\n                        * 3.11\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/user-defined-function-python-function-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: PythonFunction
---
