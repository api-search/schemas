---
description: Constraints define integrity and consistency rules for data stored in tables.
layout: schema
name: Constraint
properties_list:
- description: Name of the Constraint
  name: name
  type: string
- description: ''
  name: column_names
  type: array
- description: Type of the constraint
  name: constraint_type
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/iceberg-table-constraint-schema.json
slug: iceberg-table-constraint
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Constraint\",\n  \"type\": \"object\",\n  \"description\": \"Constraints define integrity and consistency rules for data stored in tables.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Constraint\"\n    },\n    \"column_names\": {\n      \"type\": \"array\"\n    },\n    \"constraint_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the constraint\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/iceberg-table-constraint-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Constraint
---
