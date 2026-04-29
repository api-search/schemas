---
description: PowerPoint slide
layout: schema
name: Slide
properties_list:
- description: Slide index (0-based)
  name: index
  type: integer
- description: Slide title text
  name: title
  type: string
- description: ''
  name: shapes
  type: array
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-slide-schema.json
slug: apache-poi-slide
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-slide-schema.json\",\n  \"title\": \"Slide\",\n  \"description\": \"PowerPoint slide\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"Slide index (0-based)\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Slide title text\"\n    },\n    \"shapes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Shape\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-slide-schema.json
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: Slide
---
