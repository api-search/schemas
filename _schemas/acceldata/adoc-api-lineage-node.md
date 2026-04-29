---
description: A node in the data lineage graph
layout: schema
name: LineageNode
properties_list:
- description: Dataset or table identifier
  name: id
  type: string
- description: Dataset or table name
  name: name
  type: string
- description: Source platform
  name: source
  type: string
provider_name: Acceldata
provider_slug: acceldata
schema_file: json-schema/adoc-api-lineage-node-schema.json
slug: adoc-api-lineage-node
source_filename: adoc-api-lineage-node-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://acceldata.io/schemas/lineage-node.json\",\n  \"title\": \"LineageNode\",\n  \"type\": \"object\",\n  \"description\": \"A node in the data lineage graph\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset or table identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset or table name\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source platform\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/json-schema/adoc-api-lineage-node-schema.json
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
title: LineageNode
---
