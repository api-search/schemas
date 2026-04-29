---
description: Request to create a PowerPoint presentation
layout: schema
name: PresentationRequest
properties_list:
- description: Presentation filename
  name: name
  type: string
- description: Presentation format
  name: format
  type: string
- description: Initial number of blank slides
  name: slideCount
  type: integer
provider_name: Apache POI
provider_slug: apache-poi
schema_file: json-schema/apache-poi-presentation-request-schema.json
slug: apache-poi-presentation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-presentation-request-schema.json\",\n  \"title\": \"PresentationRequest\",\n  \"description\": \"Request to create a PowerPoint presentation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Presentation filename\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PPT\",\n        \"PPTX\"\n      ],\n      \"description\": \"Presentation format\"\n    },\n    \"slideCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Initial number of blank slides\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"format\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-poi/refs/heads/main/json-schema/apache-poi-presentation-request-schema.json
tags:
- Document Processing
- Excel
- Java
- Microsoft Office
- PowerPoint
- Word
- Apache
- Open Source
title: PresentationRequest
---
