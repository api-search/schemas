---
description: Represents a hyperlink associated with a shape.
layout: schema
name: VisioHyperlink
properties_list:
- description: Unique identifier for the hyperlink.
  name: id
  type: string
- description: The URL target of the hyperlink.
  name: address
  type: string
- description: Description of the hyperlink.
  name: description
  type: string
- description: Sub-address target within the document.
  name: subAddress
  type: string
provider_name: Microsoft Visio
provider_slug: microsoft-visio
schema_file: json-schema/visio-graph-api-visio-hyperlink-schema.json
slug: visio-graph-api-visio-hyperlink
source_filename: visio-graph-api-visio-hyperlink-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/json-schema/visio-graph-api-visio-hyperlink-schema.json\",\n  \"title\": \"VisioHyperlink\",\n  \"description\": \"Represents a hyperlink associated with a shape.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique identifier for the hyperlink.\" },\n    \"address\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"The URL target of the hyperlink.\" },\n    \"description\": { \"type\": \"string\", \"description\": \"Description of the hyperlink.\" },\n    \"subAddress\": { \"type\": \"string\", \"description\": \"Sub-address target within the document.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/json-schema/visio-graph-api-visio-hyperlink-schema.json
tags:
- Business Process
- Diagramming
- Flowcharts
- Microsoft 365
- Visualization
title: VisioHyperlink
---
