---
description: Standard error response from the Data Lifecycle Manager API.
layout: schema
name: Error
properties_list:
- description: ''
  name: message
  type: string
- description: ''
  name: code
  type: string
- description: ''
  name: requestId
  type: string
provider_name: Amazon Data Lifecycle Manager
provider_slug: amazon-data-lifecycle-manager
schema_file: json-schema/error-schema.json
slug: error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-lifecycle-manager/json-schema/error-schema.json\",\n  \"title\": \"Error\",\n  \"description\": \"Standard error response from the Data Lifecycle Manager API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"code\": {\n      \"type\": \"string\"\n    },\n    \"requestId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-lifecycle-manager/refs/heads/main/json-schema/error-schema.json
tags:
- AWS
- Backup
- EBS Snapshots
- Lifecycle Management
- Storage
- Automation
- Compliance
title: Error
---
