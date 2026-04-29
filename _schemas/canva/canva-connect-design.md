---
description: A Canva design
layout: schema
name: Design
properties_list:
- description: The design ID
  name: id
  type: string
- description: The design title
  name: title
  type: string
- description: Unix timestamp in seconds when the design was created
  name: created_at
  type: integer
- description: Unix timestamp in seconds when the design was last updated
  name: updated_at
  type: integer
- description: The number of pages in the design
  name: page_count
  type: integer
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-design-schema.json
slug: canva-connect-design
source_filename: canva-connect-design-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Design\",\n  \"type\": \"object\",\n  \"description\": \"A Canva design\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The design ID\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The design title\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in seconds when the design was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in seconds when the design was last updated\"\n    },\n    \"page_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of pages in the design\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-design-schema.json
tags:
- Apps
- Automation
- Brand Management
- Collaboration
- Design
- Graphics
- Marketing
- Print
- Templates
- Visual Content
title: Design
---
