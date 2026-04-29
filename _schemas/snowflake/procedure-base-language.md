---
description: ''
layout: schema
name: BaseLanguage
properties_list:
- description: Runtime version of the function's/procedure's specified language
  name: runtime_version
  type: string
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
schema_file: json-schema/procedure-base-language-schema.json
slug: procedure-base-language
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BaseLanguage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"runtime_version\": {\n      \"type\": \"string\",\n      \"description\": \"Runtime version of the function's/procedure's specified language\"\n    },\n    \"packages\": {\n      \"type\": \"array\",\n      \"description\": \"Packages to include with the function/procedure\"\n    },\n    \"imports\": {\n      \"type\": \"array\",\n      \"description\": \"List of imports\"\n    },\n    \"handler\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified method name including the package and the class\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/procedure-base-language-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: BaseLanguage
---
