---
description: Array of unique account identifiers.
layout: schema
name: AccountIdentifiers
properties_list:
- description: ''
  name: accounts
  type: array
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/database-account-identifiers-schema.json
slug: database-account-identifiers
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccountIdentifiers\",\n  \"type\": \"object\",\n  \"description\": \"Array of unique account identifiers.\",\n  \"properties\": {\n    \"accounts\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/database-account-identifiers-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: AccountIdentifiers
---
