---
description: PowerPoint presentation
layout: schema
name: Presentation
properties_list:
- description: Presentation identifier
  name: id
  type: string
- description: Presentation filename
  name: name
  type: string
- description: Presentation format
  name: format
  type: string
- description: ''
  name: slides
  type: array
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-presentation-schema.json
slug: apache-poi-presentation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-presentation-schema.json\",\n  \"title\": \"Presentation\",\n  \"description\": \"PowerPoint presentation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Presentation identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Presentation filename\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PPT\",\n        \"PPTX\"\n      ],\n      \"description\": \"Presentation format\"\n    },\n    \"slides\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Slide\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-presentation-schema.json
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: Presentation
---
