---
description: A query defines a data request against a LookML model. Queries are immutable once created and contain the model, view, fields, filters, sorts, and limit needed to generate SQL and retrieve results.
layout: schema
name: Query
properties_list:
- description: Unique numeric identifier for this query
  name: id
  type: integer
- description: LookML model name
  name: model
  type: string
- description: LookML explore (view) name
  name: view
  type: string
- description: List of field names to include in the query results (e.g. orders.count, users.created_date)
  name: fields
  type: array
- description: List of field names to pivot on
  name: pivots
  type: array
- description: Fields to fill missing date values for
  name: fill_fields
  type: array
- description: Key-value map of filter expressions. Keys are field names and values are Looker filter expressions.
  name: filters
  type: object
- description: Custom filter expression using Looker filter syntax
  name: filter_expression
  type: string
- description: Sort order for results. Each item is a field name optionally followed by asc or desc.
  name: sorts
  type: array
- description: Maximum number of rows to return (as string)
  name: limit
  type: string
- description: Maximum number of columns for pivoted results
  name: column_limit
  type: string
- description: Whether to include row totals
  name: total
  type: boolean
- description: Row total display setting
  name: row_total
  type: string
- description: Fields to subtotal on
  name: subtotals
  type: array
- description: JSON string of dynamic field definitions
  name: dynamic_fields
  type: string
- description: Visualization configuration object
  name: vis_config
  type: object
- description: Timezone for date/time calculations
  name: query_timezone
  type: string
- description: Client-generated hash of the query for caching
  name: client_id
  type: string
- description: Short unique URL slug for this query
  name: slug
  type: string
- description: Shareable URL for this query
  name: share_url
  type: string
- description: Relative URL for this query in the Looker UI
  name: url
  type: string
- description: Whether this query has table calculations
  name: has_table_calculations
  type: boolean
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-query-schema.json
slug: looker-query
source_filename: looker-query-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Query\",\n  \"type\": \"object\",\n  \"description\": \"A query defines a data request against a LookML model. Queries are immutable once created and contain the model, view, fields, filters, sorts, and limit needed to generate SQL and retrieve results.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier for this query\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"LookML model name\"\n    },\n    \"view\": {\n      \"type\": \"string\",\n      \"description\": \"LookML explore (view) name\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"List of field names to include in the query results (e.g. orders.count, users.created_date)\"\n    },\n    \"pivots\": {\n      \"type\": \"array\",\n      \"description\": \"List of field names to pivot on\"\n    },\n  \
  \  \"fill_fields\": {\n      \"type\": \"array\",\n      \"description\": \"Fields to fill missing date values for\"\n    },\n    \"filters\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value map of filter expressions. Keys are field names and values are Looker filter expressions.\"\n    },\n    \"filter_expression\": {\n      \"type\": \"string\",\n      \"description\": \"Custom filter expression using Looker filter syntax\"\n    },\n    \"sorts\": {\n      \"type\": \"array\",\n      \"description\": \"Sort order for results. Each item is a field name optionally followed by asc or desc.\"\n    },\n    \"limit\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum number of rows to return (as string)\"\n    },\n    \"column_limit\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum number of columns for pivoted results\"\n    },\n    \"total\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include row totals\"\n   \
  \ },\n    \"row_total\": {\n      \"type\": \"string\",\n      \"description\": \"Row total display setting\"\n    },\n    \"subtotals\": {\n      \"type\": \"array\",\n      \"description\": \"Fields to subtotal on\"\n    },\n    \"dynamic_fields\": {\n      \"type\": \"string\",\n      \"description\": \"JSON string of dynamic field definitions\"\n    },\n    \"vis_config\": {\n      \"type\": \"object\",\n      \"description\": \"Visualization configuration object\"\n    },\n    \"query_timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone for date/time calculations\"\n    },\n    \"client_id\": {\n      \"type\": \"string\",\n      \"description\": \"Client-generated hash of the query for caching\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"Short unique URL slug for this query\"\n    },\n    \"share_url\": {\n      \"type\": \"string\",\n      \"description\": \"Shareable URL for this query\"\n    },\n    \"url\": {\n   \
  \   \"type\": \"string\",\n      \"description\": \"Relative URL for this query in the Looker UI\"\n    },\n    \"has_table_calculations\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this query has table calculations\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-query-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: Query
---
