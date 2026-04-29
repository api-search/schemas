---
description: A Boltic Table is a no-code database entity for storing and managing structured data with a defined column schema.
layout: schema
name: Boltic Table
properties_list:
- description: Unique identifier for the table
  name: id
  type: string
- description: Human-readable name for the table
  name: name
  type: string
- description: Description of the table's purpose
  name: description
  type: string
- description: Schema definition of the table columns
  name: columns
  type: array
- description: Number of rows in the table
  name: rowCount
  type: integer
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Boltic
provider_slug: boltic
schema_file: json-schema/boltic-table.json
slug: boltic-table
source_filename: boltic-table.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/json-schema/boltic-table.json\",\n  \"title\": \"Boltic Table\",\n  \"description\": \"A Boltic Table is a no-code database entity for storing and managing structured data with a defined column schema.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"columns\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the table\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the table\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the table's purpose\"\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/column\"\n      },\n      \"description\": \"Schema definition of the table columns\"\
  \n    },\n    \"rowCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of rows in the table\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$defs\": {\n    \"column\": {\n      \"type\": \"object\",\n      \"required\": [\"name\", \"type\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Column name\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"text\",\n            \"number\",\n            \"boolean\",\n            \"date\",\n            \"datetime\",\n            \"email\",\n            \"url\",\n            \"select\",\n            \"multi-select\",\n            \"attachment\",\n            \"relation\"\n\
  \          ],\n          \"description\": \"Data type of the column\"\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether the column requires a value\"\n        },\n        \"defaultValue\": {\n          \"type\": \"string\",\n          \"description\": \"Default value for the column\"\n        },\n        \"options\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Options for select and multi-select column types\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/json-schema/boltic-table.json
tags:
- Automation
- DataSync
- Gateways
- NoCode
- Streaming
- Workflows
title: Boltic Table
---
