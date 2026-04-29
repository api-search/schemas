---
description: A custom design type with specific dimensions
layout: schema
name: CustomDesignType
properties_list:
- description: ''
  name: type
  type: string
- description: Width in pixels (40-8000)
  name: width
  type: integer
- description: Height in pixels (40-8000)
  name: height
  type: integer
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-custom-design-type-schema.json
slug: canva-connect-custom-design-type
source_filename: canva-connect-custom-design-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CustomDesignType\",\n  \"type\": \"object\",\n  \"description\": \"A custom design type with specific dimensions\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"Width in pixels (40-8000)\"\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"Height in pixels (40-8000)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-custom-design-type-schema.json
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
title: CustomDesignType
---
