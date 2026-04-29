---
description: Data lineage graph for a dataset
layout: schema
name: LineageGraph
properties_list:
- description: Dataset identifier
  name: datasetId
  type: string
- description: Dataset name
  name: datasetName
  type: string
- description: Upstream data sources
  name: upstream
  type: array
- description: Downstream data consumers
  name: downstream
  type: array
provider_name: Acceldata
provider_slug: acceldata
schema_file: json-schema/adoc-api-lineage-graph-schema.json
slug: adoc-api-lineage-graph
source_filename: adoc-api-lineage-graph-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://acceldata.io/schemas/lineage-graph.json\",\n  \"title\": \"LineageGraph\",\n  \"type\": \"object\",\n  \"description\": \"Data lineage graph for a dataset\",\n  \"properties\": {\n    \"datasetId\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset identifier\"\n    },\n    \"datasetName\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset name\"\n    },\n    \"upstream\": {\n      \"type\": \"array\",\n      \"description\": \"Upstream data sources\",\n      \"items\": {\n        \"$ref\": \"lineage-node.json\"\n      }\n    },\n    \"downstream\": {\n      \"type\": \"array\",\n      \"description\": \"Downstream data consumers\",\n      \"items\": {\n        \"$ref\": \"lineage-node.json\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/json-schema/adoc-api-lineage-graph-schema.json
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
title: LineageGraph
---
