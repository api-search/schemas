---
description: Response containing a list of workers.
layout: schema
name: List Workers Response
properties_list:
- description: ''
  name: workers
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon Deadline Cloud
provider_slug: amazon-deadline-cloud
schema_file: json-schema/list-workers-response-schema.json
slug: list-workers-response
source_filename: list-workers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deadline-cloud/json-schema/list-workers-response-schema.json\",\n  \"title\": \"List Workers Response\",\n  \"description\": \"Response containing a list of workers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workers\": {\n      \"type\": \"array\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/json-schema/list-workers-response-schema.json
tags:
- AWS
- Compute
- Media
- Rendering
- Visual Effects
title: List Workers Response
---
