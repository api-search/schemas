---
description: Shape on a PowerPoint slide
layout: schema
name: Shape
properties_list:
- description: Shape identifier
  name: id
  type: integer
- description: Shape name
  name: name
  type: string
- description: Shape type (TextBox, Picture, Table, etc.)
  name: type
  type: string
- description: Text content of the shape
  name: text
  type: string
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-shape-schema.json
slug: apache-poi-shape
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-shape-schema.json\",\n  \"title\": \"Shape\",\n  \"description\": \"Shape on a PowerPoint slide\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Shape identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Shape name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Shape type (TextBox, Picture, Table, etc.)\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Text content of the shape\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-shape-schema.json
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: Shape
---
