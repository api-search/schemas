---
description: A Canva brand template (requires Enterprise)
layout: schema
name: BrandTemplate
properties_list:
- description: The brand template ID
  name: id
  type: string
- description: The brand template title
  name: title
  type: string
- description: URL to view the brand template
  name: view_url
  type: string
- description: URL to create a design from the brand template
  name: create_url
  type: string
- description: Unix timestamp in seconds when the template was created
  name: created_at
  type: integer
- description: Unix timestamp in seconds when the template was last updated
  name: updated_at
  type: integer
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-brand-template-schema.json
slug: canva-connect-brand-template
source_filename: canva-connect-brand-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BrandTemplate\",\n  \"type\": \"object\",\n  \"description\": \"A Canva brand template (requires Enterprise)\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The brand template ID\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The brand template title\"\n    },\n    \"view_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to view the brand template\"\n    },\n    \"create_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to create a design from the brand template\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in seconds when the template was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in seconds when the template was last updated\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-brand-template-schema.json
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
title: BrandTemplate
---
