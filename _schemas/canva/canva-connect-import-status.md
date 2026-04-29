---
description: The import status of an asset (deprecated)
layout: schema
name: ImportStatus
properties_list:
- description: The current import state
  name: state
  type: string
- description: Error details if the import failed
  name: error
  type: object
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-import-status-schema.json
slug: canva-connect-import-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImportStatus\",\n  \"type\": \"object\",\n  \"description\": \"The import status of an asset (deprecated)\",\n  \"properties\": {\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current import state\"\n    },\n    \"error\": {\n      \"type\": \"object\",\n      \"description\": \"Error details if the import failed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-import-status-schema.json
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
title: ImportStatus
---
