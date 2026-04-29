---
description: Package upload operation result for the Microsoft Edge Add-ons API
layout: schema
name: PackageUploadResult
properties_list:
- description: Upload operation identifier
  name: operationId
  type: string
- description: Operation status
  name: status
  type: string
- description: Status message
  name: message
  type: string
provider_name: Microsoft Edge
provider_slug: microsoft-edge
schema_file: json-schema/addons-api-package-upload-result-schema.json
slug: addons-api-package-upload-result
source_filename: addons-api-package-upload-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/json-schema/addons-api-package-upload-result-schema.json\",\n  \"title\": \"PackageUploadResult\",\n  \"description\": \"Package upload operation result for the Microsoft Edge Add-ons API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operationId\": {\n      \"type\": \"string\",\n      \"description\": \"Upload operation identifier\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Operation status\",\n      \"enum\": [\"InProgress\", \"Succeeded\", \"Failed\"]\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Status message\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/json-schema/addons-api-package-upload-result-schema.json
tags:
- Browser
- Chromium
- Developer Tools
- Edge
- Extensions
- Microsoft
- Progressive Web Apps
- Web Development
- WebView
title: PackageUploadResult
---
