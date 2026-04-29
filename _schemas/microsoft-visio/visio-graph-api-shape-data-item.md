---
description: Represents a data item associated with a shape.
layout: schema
name: ShapeDataItem
properties_list:
- description: Label of the data item.
  name: label
  type: string
- description: Value of the data item.
  name: value
  type: string
- description: Format of the data item.
  name: format
  type: string
provider_name: Microsoft Visio
provider_slug: microsoft-visio
schema_file: json-schema/visio-graph-api-shape-data-item-schema.json
slug: visio-graph-api-shape-data-item
source_filename: visio-graph-api-shape-data-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/json-schema/visio-graph-api-shape-data-item-schema.json\",\n  \"title\": \"ShapeDataItem\",\n  \"description\": \"Represents a data item associated with a shape.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"label\": { \"type\": \"string\", \"description\": \"Label of the data item.\" },\n    \"value\": { \"type\": \"string\", \"description\": \"Value of the data item.\" },\n    \"format\": { \"type\": \"string\", \"description\": \"Format of the data item.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/json-schema/visio-graph-api-shape-data-item-schema.json
tags:
- Business Process
- Diagramming
- Flowcharts
- Microsoft 365
- Visualization
title: ShapeDataItem
---
