---
description: Standard error response from the Deadline Cloud API.
layout: schema
name: Error
properties_list:
- description: ''
  name: message
  type: string
- description: ''
  name: code
  type: string
provider_name: Amazon Deadline Cloud
provider_slug: amazon-deadline-cloud
schema_file: json-schema/error-schema.json
slug: error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deadline-cloud/json-schema/error-schema.json\",\n  \"title\": \"Error\",\n  \"description\": \"Standard error response from the Deadline Cloud API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"code\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/json-schema/error-schema.json
tags:
- AWS
- Compute
- Media
- Rendering
- Visual Effects
title: Error
---
