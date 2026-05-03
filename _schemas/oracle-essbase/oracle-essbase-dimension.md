---
description: A dimension in an Oracle Essbase database outline. Dimensions define the axes of a multi-dimensional data model and contain hierarchical members. Common dimension types include accounts, time, scenario, entity, and attribute dimensions.
layout: schema
name: Oracle Essbase Dimension
properties_list:
- description: Dimension name as defined in the database outline.
  name: name
  type: string
- description: Dimension type classification. Accounts dimensions hold numeric measures. Time dimensions represent temporal periods. Attribute dimensions provide alternate categorizations.
  name: type
  type: string
- description: How the dimension data is stored. Dense dimensions have data at most intersections. Sparse dimensions have data at few intersections.
  name: storageType
  type: string
- description: Dimension tag used for categorization and identification within the outline.
  name: tag
  type: string
- description: Total number of members in the dimension hierarchy.
  name: memberCount
  type: integer
provider_name: Oracle Essbase
provider_slug: oracle-essbase
schema_file: json-schema/oracle-essbase-dimension-schema.json
slug: oracle-essbase-dimension
source_filename: oracle-essbase-dimension-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"oracle-essbase-dimension-schema.json\",\n  \"title\": \"Oracle Essbase Dimension\",\n  \"description\": \"A dimension in an Oracle Essbase database outline. Dimensions define the axes of a multi-dimensional data model and contain hierarchical members. Common dimension types include accounts, time, scenario, entity, and attribute dimensions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Dimension name as defined in the database outline.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Dimension type classification. Accounts dimensions hold numeric measures. Time dimensions represent temporal periods. Attribute dimensions provide alternate categorizations.\"\n    },\n    \"storageType\": {\n      \"type\": \"string\",\n      \"description\": \"How the dimension data is stored. Dense dimensions\
  \ have data at most intersections. Sparse dimensions have data at few intersections.\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"Dimension tag used for categorization and identification within the outline.\"\n    },\n    \"memberCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of members in the dimension hierarchy.\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/json-schema/oracle-essbase-dimension-schema.json
tags:
- Analytics
- Budgeting
- Business Intelligence
- Financial Consolidation
- Multi-Dimensional Database
- OLAP
- Planning
title: Oracle Essbase Dimension
---
