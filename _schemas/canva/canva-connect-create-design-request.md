---
description: Request body for creating a new design
layout: schema
name: CreateDesignRequest
properties_list:
- description: An image asset ID to insert into the design
  name: asset_id
  type: string
- description: The design title (1-255 characters)
  name: title
  type: string
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-create-design-request-schema.json
slug: canva-connect-create-design-request
source_filename: canva-connect-create-design-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateDesignRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new design\",\n  \"properties\": {\n    \"asset_id\": {\n      \"type\": \"string\",\n      \"description\": \"An image asset ID to insert into the design\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The design title (1-255 characters)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-create-design-request-schema.json
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
title: CreateDesignRequest
---
