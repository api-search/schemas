---
description: ''
layout: schema
name: BaseLanguage
properties_list:
- description: Packages to include with the function/procedure
  name: packages
  type: array
- description: List of imports
  name: imports
  type: array
- description: Fully qualified method name including the package and the class
  name: handler
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/user-defined-function-base-language-schema.json
slug: user-defined-function-base-language
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BaseLanguage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"packages\": {\n      \"type\": \"array\",\n      \"description\": \"Packages to include with the function/procedure\"\n    },\n    \"imports\": {\n      \"type\": \"array\",\n      \"description\": \"List of imports\"\n    },\n    \"handler\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified method name including the package and the class\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/user-defined-function-base-language-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: BaseLanguage
---
