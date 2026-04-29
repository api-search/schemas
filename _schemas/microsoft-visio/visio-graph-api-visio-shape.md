---
description: Represents a shape on a Visio page.
layout: schema
name: VisioShape
properties_list:
- description: Unique identifier for the shape.
  name: id
  type: string
- description: The name of the shape.
  name: name
  type: string
- description: The text content of the shape.
  name: text
  type: string
- description: The shape type.
  name: type
  type: string
provider_name: Microsoft Visio
provider_slug: microsoft-visio
schema_file: json-schema/visio-graph-api-visio-shape-schema.json
slug: visio-graph-api-visio-shape
source_filename: visio-graph-api-visio-shape-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/json-schema/visio-graph-api-visio-shape-schema.json\",\n  \"title\": \"VisioShape\",\n  \"description\": \"Represents a shape on a Visio page.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique identifier for the shape.\" },\n    \"name\": { \"type\": \"string\", \"description\": \"The name of the shape.\" },\n    \"text\": { \"type\": \"string\", \"description\": \"The text content of the shape.\" },\n    \"type\": { \"type\": \"string\", \"description\": \"The shape type.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/json-schema/visio-graph-api-visio-shape-schema.json
tags:
- Business Process
- Diagramming
- Flowcharts
- Microsoft 365
- Visualization
title: VisioShape
---
