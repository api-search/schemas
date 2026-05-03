---
description: A calculation or MDX script associated with an Oracle Essbase database. Calculation scripts (.csc) contain Essbase calculation language statements for aggregating and computing data values. MDX scripts contain MDX queries for data retrieval and manipulation.
layout: schema
name: Oracle Essbase Script
properties_list:
- description: Script name, typically including the file extension (.csc for calculation scripts).
  name: name
  type: string
- description: Full text content of the script including calculation or MDX statements.
  name: content
  type: string
- description: User ID of the person who last modified the script.
  name: modifiedBy
  type: string
- description: Last modification timestamp in milliseconds since Unix epoch.
  name: modifiedTime
  type: integer
- description: HATEOAS navigation links.
  name: links
  type: array
provider_name: Oracle Essbase
provider_slug: oracle-essbase
schema_file: json-schema/oracle-essbase-script-schema.json
slug: oracle-essbase-script
source_filename: oracle-essbase-script-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"oracle-essbase-script-schema.json\",\n  \"title\": \"Oracle Essbase Script\",\n  \"description\": \"A calculation or MDX script associated with an Oracle Essbase database. Calculation scripts (.csc) contain Essbase calculation language statements for aggregating and computing data values. MDX scripts contain MDX queries for data retrieval and manipulation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Script name, typically including the file extension (.csc for calculation scripts).\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Full text content of the script including calculation or MDX statements.\"\n    },\n    \"modifiedBy\": {\n      \"type\": \"string\",\n      \"description\": \"User ID of the person who last modified the script.\"\n    },\n    \"modifiedTime\": {\n      \"\
  type\": \"integer\",\n      \"description\": \"Last modification timestamp in milliseconds since Unix epoch.\"\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"description\": \"HATEOAS navigation links.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Link\"\n      }\n    }\n  },\n  \"required\": [\"name\", \"content\"],\n  \"$defs\": {\n    \"Link\": {\n      \"type\": \"object\",\n      \"description\": \"HATEOAS navigation link.\",\n      \"properties\": {\n        \"rel\": {\n          \"type\": \"string\",\n          \"description\": \"Link relation type.\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Link URL.\"\n        },\n        \"method\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP method for this link.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Media type of the linked resource.\"\n        }\n \
  \     }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/json-schema/oracle-essbase-script-schema.json
tags:
- Analytics
- Budgeting
- Business Intelligence
- Financial Consolidation
- Multi-Dimensional Database
- OLAP
- Planning
title: Oracle Essbase Script
---
