---
description: A graph of lineage nodes and edges
layout: schema
name: LineageGraph
properties_list:
- description: ''
  name: nodes
  type: array
- description: ''
  name: edges
  type: array
provider_name: Alation
provider_slug: alation
schema_file: json-schema/alation-alation-lineage-lineage-graph-schema.json
slug: alation-alation-lineage-lineage-graph
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-lineage-lineage-graph-schema.json\",\n  \"title\": \"LineageGraph\",\n  \"description\": \"A graph of lineage nodes and edges\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nodes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"edges\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-lineage-lineage-graph-schema.json
tags:
- Data Catalog
- Data Governance
- Data Intelligence
- Data Lineage
- Data Quality
- Business Glossary
- Metadata Management
- AI
title: LineageGraph
---
