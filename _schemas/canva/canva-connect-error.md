---
description: An error response
layout: schema
name: Error
properties_list:
- description: Machine-readable error code
  name: code
  type: string
- description: Human-readable error message
  name: message
  type: string
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-error-schema.json
slug: canva-connect-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"An error response\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Machine-readable error code\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-error-schema.json
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
title: Error
---
