---
description: A relationship between two tables in a dataset
layout: schema
name: Relationship
properties_list:
- description: The name of the relationship
  name: name
  type: string
- description: The source table name
  name: fromTable
  type: string
- description: The source column name
  name: fromColumn
  type: string
- description: The target table name
  name: toTable
  type: string
- description: The target column name
  name: toColumn
  type: string
- description: The cross-filtering direction
  name: crossFilteringBehavior
  type: string
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-relationship-schema.json
slug: power-bi-rest-relationship
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Relationship\",\n  \"type\": \"object\",\n  \"description\": \"A relationship between two tables in a dataset\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the relationship\"\n    },\n    \"fromTable\": {\n      \"type\": \"string\",\n      \"description\": \"The source table name\"\n    },\n    \"fromColumn\": {\n      \"type\": \"string\",\n      \"description\": \"The source column name\"\n    },\n    \"toTable\": {\n      \"type\": \"string\",\n      \"description\": \"The target table name\"\n    },\n    \"toColumn\": {\n      \"type\": \"string\",\n      \"description\": \"The target column name\"\n    },\n    \"crossFilteringBehavior\": {\n      \"type\": \"string\",\n      \"description\": \"The cross-filtering direction\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-relationship-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: Relationship
---
