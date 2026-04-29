---
description: Standard error response from the DataSync API.
layout: schema
name: Error
properties_list:
- description: ''
  name: message
  type: string
- description: ''
  name: errorCode
  type: string
provider_name: Amazon DataSync
provider_slug: amazon-datasync
schema_file: json-schema/error-schema.json
slug: error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datasync/json-schema/error-schema.json\",\n  \"title\": \"Error\",\n  \"description\": \"Standard error response from the DataSync API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"errorCode\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datasync/refs/heads/main/json-schema/error-schema.json
tags:
- AWS
- Data Transfer
- Migration
- Storage
- Automation
- Hybrid Cloud
title: Error
---
