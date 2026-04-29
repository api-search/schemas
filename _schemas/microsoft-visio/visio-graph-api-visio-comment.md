---
description: Represents a comment on a shape.
layout: schema
name: VisioComment
properties_list:
- description: Unique identifier for the comment.
  name: id
  type: string
- description: The comment text.
  name: text
  type: string
- description: The author of the comment.
  name: author
  type: string
- description: When the comment was created.
  name: date
  type: string
provider_name: Microsoft Visio
provider_slug: microsoft-visio
schema_file: json-schema/visio-graph-api-visio-comment-schema.json
slug: visio-graph-api-visio-comment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/json-schema/visio-graph-api-visio-comment-schema.json\",\n  \"title\": \"VisioComment\",\n  \"description\": \"Represents a comment on a shape.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique identifier for the comment.\" },\n    \"text\": { \"type\": \"string\", \"description\": \"The comment text.\" },\n    \"author\": { \"type\": \"string\", \"description\": \"The author of the comment.\" },\n    \"date\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"When the comment was created.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/json-schema/visio-graph-api-visio-comment-schema.json
tags:
- Business Process
- Diagramming
- Flowcharts
- Microsoft 365
- Visualization
title: VisioComment
---
