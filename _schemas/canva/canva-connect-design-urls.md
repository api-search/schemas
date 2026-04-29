---
description: Temporary URLs for accessing a design (expire after 30 days)
layout: schema
name: DesignUrls
properties_list:
- description: URL to edit the design (expires in 30 days)
  name: edit_url
  type: string
- description: URL to view the design (expires in 30 days)
  name: view_url
  type: string
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-design-urls-schema.json
slug: canva-connect-design-urls
source_filename: canva-connect-design-urls-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DesignUrls\",\n  \"type\": \"object\",\n  \"description\": \"Temporary URLs for accessing a design (expire after 30 days)\",\n  \"properties\": {\n    \"edit_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to edit the design (expires in 30 days)\"\n    },\n    \"view_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to view the design (expires in 30 days)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-design-urls-schema.json
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
title: DesignUrls
---
