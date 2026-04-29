---
description: Writable fields for creating a new query
layout: schema
name: WriteQuery
properties_list:
- description: LookML model name
  name: model
  type: string
- description: LookML explore (view) name
  name: view
  type: string
- description: List of field names to include
  name: fields
  type: array
- description: Fields to pivot on
  name: pivots
  type: array
- description: Fields to fill missing values for
  name: fill_fields
  type: array
- description: Filter expressions keyed by field name
  name: filters
  type: object
- description: Custom filter expression
  name: filter_expression
  type: string
- description: Sort order for results
  name: sorts
  type: array
- description: Maximum rows to return
  name: limit
  type: string
- description: Maximum columns for pivoted results
  name: column_limit
  type: string
- description: Include row totals
  name: total
  type: boolean
- description: Row total setting
  name: row_total
  type: string
- description: Fields to subtotal on
  name: subtotals
  type: array
- description: JSON string of dynamic field definitions
  name: dynamic_fields
  type: string
- description: Visualization configuration
  name: vis_config
  type: object
- description: Timezone for date/time calculations
  name: query_timezone
  type: string
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-write-query-schema.json
slug: looker-write-query
source_filename: looker-write-query-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WriteQuery\",\n  \"type\": \"object\",\n  \"description\": \"Writable fields for creating a new query\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"LookML model name\"\n    },\n    \"view\": {\n      \"type\": \"string\",\n      \"description\": \"LookML explore (view) name\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"List of field names to include\"\n    },\n    \"pivots\": {\n      \"type\": \"array\",\n      \"description\": \"Fields to pivot on\"\n    },\n    \"fill_fields\": {\n      \"type\": \"array\",\n      \"description\": \"Fields to fill missing values for\"\n    },\n    \"filters\": {\n      \"type\": \"object\",\n      \"description\": \"Filter expressions keyed by field name\"\n    },\n    \"filter_expression\": {\n      \"type\": \"string\",\n      \"description\": \"Custom filter expression\"\
  \n    },\n    \"sorts\": {\n      \"type\": \"array\",\n      \"description\": \"Sort order for results\"\n    },\n    \"limit\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum rows to return\"\n    },\n    \"column_limit\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum columns for pivoted results\"\n    },\n    \"total\": {\n      \"type\": \"boolean\",\n      \"description\": \"Include row totals\"\n    },\n    \"row_total\": {\n      \"type\": \"string\",\n      \"description\": \"Row total setting\"\n    },\n    \"subtotals\": {\n      \"type\": \"array\",\n      \"description\": \"Fields to subtotal on\"\n    },\n    \"dynamic_fields\": {\n      \"type\": \"string\",\n      \"description\": \"JSON string of dynamic field definitions\"\n    },\n    \"vis_config\": {\n      \"type\": \"object\",\n      \"description\": \"Visualization configuration\"\n    },\n    \"query_timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone\
  \ for date/time calculations\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-write-query-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: WriteQuery
---
